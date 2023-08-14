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
   export let code='';
</script>

<Card class="bg-gray-50 ">
  <CardHeader class="py-4 md:px-5">
    <CardTitle
      class="flex items-center gap-3 flex-wrap justify-center md:justify-start"
    >
      {name}
      <div class="hidden  gap-1 md:flex">
        {#each badgetags as item}
          <Badge variant="outline" class="border-slate-800">{item}</Badge>
        {/each}
      </div>
      <Button size="sm" href={code} target="_blank">
        Code
        <ExternalLink class="ml-2 w-4 h-4" strokeWidth="1.6px" />
      </Button>
    </CardTitle>
  </CardHeader>
  <CardContent class="p-2 m-0 md:mx-5 pb-4">
    <div class="box md:p-3">
      <slot />
    </div>
  </CardContent>
</Card>

<style>
  .box {
    border: 1px solid #ccc;
    border-radius: 5px;
  }
</style>
