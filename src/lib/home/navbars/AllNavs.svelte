<script>
  import Box from "$lib/home/Box.svelte";
  import Nav1 from "$lib/home/navbars/Nav1.svelte";
  import Nav2 from "$lib/home/navbars/Nav2.svelte";
  let allnavData = [
    {
      name: "Simple Navbar",
      component: Nav1,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/94f07c568206d611efeca2c8d827bdc1ac164e08/src/lib/home/navbars/Nav1.svelte",
      badgetags: ["Dark", "Responsive", "Profile"],
    },
    {
      name: "Simple Dark",
      component: Nav2,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/94f07c568206d611efeca2c8d827bdc1ac164e08/src/lib/home/navbars/Nav2.svelte",
      badgetags: ["Responsive", "Profile", "Simple"],
    },
  ];
</script>

<div>
  <h1 class="text-3xl font-bold md:my-3">Navbars</h1>
</div>
{#each allnavData as item}
  <Box {...item} >
    <svelte:component this={item.component} />
  </Box>
{/each}
