<script>
  import Box from "$lib/home/Box.svelte";
  import Banner1 from "./banner1.svelte";
  import Banner2 from "./banner2.svelte";
  import Banner3 from "./banner3.svelte";
  import Banner4 from "./banner4.svelte";
  import Banner5 from "./banner5.svelte";
  import Banner6 from "./banner6.svelte";

  let allnavData = [
    {
      name: "Simple Light Banner",
      component: Banner1,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner1.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
    {
      name: "Simple Dark",
      component: Banner2,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner2.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },

    {
      name: "Bottom Aligned",
      component: Banner3,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner3.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
    {
      name: "Floating Bottom",
      component: Banner4,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner4.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
    {
      name: "Background Glow",
      component: Banner6,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner6.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
    {
      name: "Floating Bottom Center",
      component: Banner5,
      code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Banner/banner5.svelte",
      badgetags: ["Responsive", "Profile", "Left Menu Bar"],
    },
  ];
</script>

<div>
  <h1 class="text-3xl font-bold md:my-3">Banners</h1>
  <p class="mt-2">
    Just Comment out the Top and Bottom part to see the <strong>Effects</strong>
  </p>
</div>
{#each allnavData as item}
  <Box name={item.name} badgetags={item.badgetags} code={item.code}>
    <svelte:component this={item.component} />
  </Box>
{/each}
