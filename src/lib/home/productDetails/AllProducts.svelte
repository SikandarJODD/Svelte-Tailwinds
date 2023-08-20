<script>
    import Box from "$lib/home/Box.svelte";
  import Product1 from "./product1.svelte";
  import Product2 from "./product2.svelte";
  import Product3 from "./product3.svelte";
  import Product4 from "./product4.svelte";
    
    let allnavData = [
      {
        name: "Product Details",
        component: Product1,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/productDetails/product1.svelte",
        badgetags: [
          "Responsive",
          "Profile",
          "Left Menu Bar",
        ],
      },
      {
        name: "Product Details",
        component: Product2,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/productDetails/product2.svelte",
        badgetags: [
          "Responsive",
          "Profile",
          "Left Menu Bar",
        ],
      },
      {
        name: "Product Details",
        component: Product3,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/productDetails/product3.svelte",
        badgetags: [
          "Responsive",
          "Profile",
          "Left Menu Bar",
        ],
      },
      {
        name: "Product Details",
        component: Product4,
        code: "https://github.com/SikandarJODD/Svelte-Tailwinds/blob/master/src/lib/home/productDetails/product4.svelte",
        badgetags: [
          "Responsive",
          "Profile",
          "Left Menu Bar",
        ],
      },
    ];
  </script>
  
  <div>
    <h1 class="text-3xl font-bold md:my-3">Products Page</h1>
  </div>
  {#each allnavData as item}
    <Box name={item.name} badgetags={item.badgetags} code={item.code}>
      <svelte:component this={item.component} />
    </Box>
  {/each}
  