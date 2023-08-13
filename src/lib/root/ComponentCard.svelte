<!-- Component Solo Card -->

<script>
  export let title = "UI/UX Review Check";
  /**
   * @type {any}
   */
  export let content;
</script>

<div
  class="m-4 border-2 border-gray-900 relative w-full sm:w-fit flex flex-col rounded-xl bg-white bg-clip-border text-gray-700 shadowclass hover:scale-105 transition-all duration-250 hover:bg-cyan-400"
>
  <div class="p-6">
    <h5
      class="mb-2 block font-sans text-xl md:text-2xl font-bold text-gray-800"
    >
      {title}
    </h5>
    <div class="block font-sans text-base leading-relaxed">
      <ul>
        {#each content as item, index}
          <li>
            {index + 1}.
            <a
              href={item.link}
              class="hover:text-gray-900 text-gray-600 hover:underline-offset-2 hover:underline transition-all duration-200"
            >
              {item.nv}
            </a>
          </li>
        {/each}
      </ul>
    </div>
  </div>
</div>

<style>
  
  .shadowclass:hover {
    transform: translate(-4px, -4px);
    box-shadow: 4px 4px rgb(0, 18, 22);
  }
</style>
