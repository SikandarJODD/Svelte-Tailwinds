<script>
  import Box from "$lib/home/Box.svelte";
  import Side1 from "./side1.svelte";

  let allnavData = [
    {
      name: "Simple Dark Navbar",
      component: Side1,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav1.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
  ];
</script>

<div>
  <h1 class="text-3xl font-bold md:my-3">Side Bars</h1>
  <p class="mt-2">
    Change <code class="bg-gray-200 p-1 rounded-md px-2">justify-start</code> to
    for Alignment of Nav Items to <strong>Center</strong> or
    <strong>End</strong>.
  </p>
</div>
{#each allnavData as item}
  <Box name={item.name} badgetags={item.badgetags} code={item.code}>
    <svelte:component this={item.component} />
  </Box>
{/each}
