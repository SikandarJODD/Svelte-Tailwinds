<script>
    import Box from "$lib/home/Box.svelte";
  import Cta1 from "./cta1.svelte";
  import Cta2 from "./cta2.svelte";
  import Cta3 from "./cta3.svelte";
  import Cta4 from "./cta4.svelte";
  import Cta5 from "./cta5.svelte";
  import Cta6 from "./cta6.svelte";
  
    let allnavData = [
      {
        name: "Simple Hero",
        component: Cta1,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta1.svelte",
        badgetags: ["Dark", "Responsive"],
      },
      {
        name: "Simple Hero",
        component: Cta2,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta2.svelte",
        badgetags: ["Light", "Clean"],
      },
      {
        name: "Simple Hero",
        component: Cta3,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta3.svelte",
        badgetags: ["Image Split", "Responsive"],
      },
      {
        name: "Simple Hero",
        component: Cta4,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta4.svelte",
        badgetags: ["Smooth UI", "Responsive"],
      },
      {
        name: "Simple Hero",
        component: Cta5,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta5.svelte",
        badgetags: ["Light", "Responsive"],
      },
      {
        name: "Simple Hero",
        component: Cta6,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/cat/cta6.svelte",
        badgetags: ["Light", "Responsive"],
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
  