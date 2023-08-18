<script>
  import Button from "$lib/components/ui/button/Button.svelte";
  import { BarChart2, Layout } from "lucide-svelte";
</script>

<section class="bg-gray-900 text-white">
  <div
    class="mx-auto max-w-screen-xl px-4 py-32 lg:flex lg:h-screen lg:items-center"
  >
    <div class="mx-auto max-w-3xl text-center">
      <h1
        class="bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 bg-clip-text text-3xl font-extrabold text-transparent sm:text-5xl"
      >
        Svelte Based Components

        <span class="sm:block text-white mt-4"> Tailwind CSS </span>
      </h1>

      <p class="mx-auto mt-4 max-w-xl sm:text-xl/relaxed text-gray-400">
        A collection of Svelte components built with Tailwind CSS.
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-6">
        <Button size="lg" variant="outline" href="/c">
          <Layout strokeWidth="1.4px" class="w-7 mr-2" />
          Components</Button
        >
        <Button size="lg" variant="outline" href="/">
            <BarChart2 strokeWidth="1.4px" class="w-7 mr-2" />
            Installation</Button>
      </div>
    </div>
  </div>
</section>
