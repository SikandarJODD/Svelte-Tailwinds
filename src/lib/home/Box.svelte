<script>
  import { ExternalLink } from "lucide-svelte";
  import { Button } from "$components/ui/button";
  import { Badge } from "$components/ui/badge";
  import {
    Card,
    CardContent,
    CardHeader,
    CardTitle,
  } from "$components/ui/card";

  export let name = "";
  /**
   * @type {any}
   */
  export let badgetags;
  export let code = "";
</script>

  <Card class="bg-gray-50 my-5 border-slate-400">
    <CardHeader class="py-4 md:px-5">
      <CardTitle
        class="flex items-center gap-3 flex-wrap justify-center md:justify-start"
      >
        <h1 class="text-xl font-bold md:text-2xl">
          {name}
        </h1>
        <div class="hidden gap-1 md:flex">
          {#each badgetags as item}
            <Badge
              variant="outline"
              class="px-3 py-1  border-slate-800 hover:bg-gray-800 hover:text-white cursor-pointer"
              >{item}</Badge
            >
          {/each}
        </div>
        <Button size="sm" href={code} target="_blank">
          Code
          <ExternalLink class="ml-2 w-4 h-4" strokeWidth="1.6px" />
        </Button>
      </CardTitle>
    </CardHeader>
    <CardContent class="p-2 m-0 md:mx-5 pb-4">
      <div class="box md:p-3 overflow-hidden">
        <slot />
      </div>
    </CardContent>
  </Card>

<style>
  .box {
    border: 1px solid #b1b1b1;
    border-radius: 5px;
    background: #0b0a0a0b;
  }
 
</style>
