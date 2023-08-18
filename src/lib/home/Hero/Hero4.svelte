<script>
  let hero = {
    img: "https://images.pexels.com/photos/12810665/pexels-photo-12810665.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
    title: "Life is Short, Build Stuff that Matters",
    subtext: "Create Amazing Content based on Svelte and SvelteKit",
    btn1: "Download",
    btn2: "Write Your Today",
  };
</script>

<div class="bg-gray-900">
  <div class="relative isolate overflow-hidden pt-14">
    <img
      src={hero.img}
      alt="Background"
      class="absolute inset-0 -z-10 h-full w-full object-cover opacity-60"
    />
    <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
      <div class="hidden sm:mb-8 sm:flex sm:justify-center">
        <div
          class="relative rounded-full px-3 py-1 text-sm leading-6 text-gray-300/90 ring-1 ring-white/10 hover:ring-white/20"
        >
          Announcing our next round of funding. <a
            href="/"
            class="font-semibold text-white"
            ><span class="absolute inset-0" aria-hidden="true" />Read more
            <span aria-hidden="true">&rarr;</span></a
          >
        </div>
      </div>
      <div class="text-center">
        <h1 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">
          {hero.title}
        </h1>
        <p class="mt-6 text-lg leading-8 text-gray-200">
          {hero.subtext}
        </p>
        <div
          class="mt-10 flex items-center justify-center md:gap-x-6 flex-wrap gap-3"
        >
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border-transparent transition-all duration-100 flex gap-2 justify-center items-center text-sm font-semibold leading-6 bg-white text-gray-900 hover:bg-zinc-100"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="1.6"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-arrow-down-to-line"
              ><path d="M12 17V3" /><path d="m6 11 6 6 6-6" /><path
                d="M19 21H5"
              /></svg
            >
            {hero.btn1}
          </a>
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-white border border-slate-50 bg-[#000F2987] hover:bg-[#000F29]"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="1.6"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-pencil-line"
              ><path d="M12 20h9" /><path
                d="M16.5 3.5a2.12 2.12 0 0 1 3 3L7 19l-4 1 1-4Z"
              /><path d="m15 5 3 3" /></svg
            >
            {hero.btn2}
          </a>
        </div>
      </div>
    </div>
  </div>
</div>
