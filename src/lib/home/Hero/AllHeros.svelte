<script>
    import Box from "$lib/home/Box.svelte";
  import Hero1 from "./Hero1.svelte";
  import Hero2 from "./Hero2.svelte";
  import Hero3 from "./Hero3.svelte";
  import Hero4 from "./Hero4.svelte";
  import Hero5 from "./Hero5.svelte";
    let allnavData = [
      {
        name: "Simple Hero",
        component: Hero1,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Hero/Hero1.svelte",
        badgetags: ["Light", "Responsive"],
      },
      {
        name: "Dark Mode Hero",
        component: Hero2,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Hero/Hero2.svelte",
        badgetags: ["Dark", "Responsive"],
      },
      {
        name: "Simple Hero",
        component: Hero3,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Hero/Hero3.svelte",
        badgetags: ["Simple", "Responsive"],
      },
      {
        name: "Hero with Image",
        component: Hero4,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Hero/Hero4.svelte",
        badgetags: ["Image in Background", "Responsive"],
      },
      {
        name: "Hero with Split Image",
        component: Hero5,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/Hero/Hero5.svelte",
        badgetags: ["Split Image", "Responsive","Image Carousel","Single Image"],
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
  