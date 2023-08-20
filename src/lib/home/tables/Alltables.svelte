<script>
    import Box from "$lib/home/Box.svelte";
  import Table1 from "./table1.svelte";
  import Table2 from "./table2.svelte";
  import Table3 from "./table3.svelte";
  import Table4 from "./table4.svelte";
  import Table5 from "./table5.svelte";
  
    let allnavData = [
      {
        name: "Simple Table",
        component: Table1,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/tables/table1.svelte",
        badgetags: ["Responsive", "Profile", "Left Menu Bar"],
      },
      {
        name: "Simple Table",
        component: Table2,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/tables/table1.svelte",
        badgetags: ["Responsive", "Profile", "Left Menu Bar"],
      },
      {
        name: "Simple Table",
        component: Table3,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/tables/table1.svelte",
        badgetags: ["Responsive", "Profile", "Left Menu Bar"],
      },
      {
        name: "Simple Table",
        component: Table4,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/tables/table1.svelte",
        badgetags: ["Responsive", "Profile", "Left Menu Bar"],
      },
      {
        name: "Simple Table",
        component: Table5,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/tables/table1.svelte",
        badgetags: ["Responsive", "Profile", "Left Menu Bar"],
      },
    ];
  </script>
  
  <div>
    <h1 class="text-3xl font-bold md:my-3">Tables</h1>
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
  