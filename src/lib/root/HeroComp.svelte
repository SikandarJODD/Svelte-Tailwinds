<script>
  import ComponentCard from "./ComponentCard.svelte";
  let comptitles = [
    {
      id: 1,
      name: "Navbar",
      subs: [
        {
          nv: "Simple Navbar",
          link: "/",
        },
        {
          nv: "Simple Navbar with Sign In",
          link: "/",
        },
        {
          nv: "Simple Navbar Profile ",
          link: "/",
        },
      ],
    },
    {
      id: 2,
      name: "Hero",
      subs: [
        {
          nv: "Simple Hero",
          link: "/",
        },
        {
          nv: "Image in Right",
          link: "/",
        },
        {
          nv: "Hero with  Buttons",
          link: "/",
        },
      ],
    },
    {
      id: 3,
      name: "CTA Sections",
      subs: [
        {
          nv: "Dark panel with App Screenshot",
          link: "/",
        },
        {
          nv: "Simple Stacked CTA",
          link: "/",
        },
        {
          nv: "Centered on Dark panel",
          link: "/",
        },
        {
          nv: "Simple Centered ",
          link: "/",
        },
        {
          nv: "Simple Justify on Light Brand ",
          link: "/",
        },
        {
          nv: "Two columns with photo on dark ",
          link: "/",
        },
      ],
    },
    {
      id: 4,
      name: "Stats",
      subs: [
        {
          nv: "Simple Stats",
          link: "/",
        },
        {
          nv: "Simple on Dark",
          link: "/",
        },
        {
          nv: "Simple Grid",
          link: "/",
        },
        {
          nv: "Simple Grid on Dark",
          link: "/",
        },
      ],
    },
    {
      id: 5,
      name: "Tables",
      subs: [
        {
          nv: "Simple Tables",
          link: "/",
        },
        {
          nv: "Simple on Dark",
          link: "/",
        },
        {
          nv: "Simple in card",
          link: "/",
        },
      ],
    },
    {
      id: 6,
      name: "Sign-in and Registration",
      subs: [
        {
          nv: "Simple",
          link: "/",
        },
        {
          nv: "Simple on Dark",
          link: "/",
        },
        {
          nv: "Split Screen",
          link: "/",
        },
        {
          nv: "Simple with SuperForms",
          link: "/",
        },
      ],
    },
    {
      id: 6,
      name: "Hero",
      subs: [
        {
          nv: "Simple Hero",
          link: "/",
        },
        {
          nv: "Image in Right",
          link: "/",
        },
        {
          nv: "Hero with  Buttons",
          link: "/",
        },
      ],
    },
  ];
</script>

<div class="box">
  {#each comptitles as item}
    <ComponentCard title={item.name} content={item.subs} />
  {/each}
</div>

<style>
  .box {
    background: #ffe75d;
    padding: 20px 5%;
    display: flex;
    flex-wrap: wrap;
  }
</style>
