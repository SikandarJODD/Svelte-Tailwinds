<script>
  import Box from "$lib/home/Box.svelte";
  import Nav1 from "$lib/home/navbars/Nav1.svelte";
  import Nav2 from "$lib/home/navbars/Nav2.svelte";
  import Nav3 from "$lib/home/navbars/Nav3.svelte";
  import Nav4 from "$lib/home/navbars/Nav4.svelte";
  import Nav5 from "$lib/home/navbars/Nav5.svelte";
  import Nav6 from "$lib/home/navbars/Nav6.svelte";
  import Nav7 from "$lib/home/navbars/Nav7.svelte";
  let allnavData = [
    {
      name: "Simple Dark Navbar",
      component: Nav1,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav1.svelte",
      badgetags: [
        "Responsive",
        "Profile",
        "Left Menu Bar",
      ],
    },
    {
      name: "Simple Dark",
      component: Nav2,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav2.svelte",
      badgetags: [
        "Responsive",
        "Right Menu Bar",
      ],
    },
    {
      name: "Simple Light",
      component: Nav3,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav3.svelte",
      badgetags: [
        "Responsive",
        "Profile",
        "Light",
      ],
    },
    {
      name: "Simple Light with New Design",
      component: Nav4,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav4.svelte",
      badgetags: ["Responsive", "Profile", "Light"],
    },
    {
      name: "Simple Right Menu Bar",
      component: Nav5,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/navbars/Nav5.svelte",
      badgetags: ["Responsive", "Profile", "Light"],
    },
  ];
</script>

<div>
  <h1 class="text-3xl font-bold md:my-3">Navbars</h1>
  <p class="mt-2">
    Change <code class="bg-gray-200 p-1 rounded-md px-2">justify-start</code> to for Alignment
    of Nav Items to <strong>Center</strong> or <strong>End</strong>.
  </p>
</div>
{#each allnavData as item}
  <Box name={item.name} badgetags={item.badgetags} code={item.code}>
    <svelte:component this={item.component} />
  </Box>
{/each}
