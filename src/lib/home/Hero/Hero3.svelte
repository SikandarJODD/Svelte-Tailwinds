<script>
  let herosec = {
    title: "Life is Short, Build Stuff that Matters",
    subtext: "Create Amazing Content based on Svelte and SvelteKit",
    btn1: "Download",
    btn2: "Write Your Today",
  };
</script>

<div class="bg-white">
  <div class="relative isolate px-6 pt-14 lg:px-8">
    <div
      class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80"
      aria-hidden="true"
    >
      <div
        class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-30 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]"
        style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)"
      />
    </div>
    <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
      <div class="hidden sm:mb-8 sm:flex  sm:justify-center">
        <div
          class="relative rounded-full px-3 py-1 text-sm leading-6 text-gray-600 ring-1 ring-gray-900/10 hover:ring-gray-900/20"
        >
          Download Free Svelte Tailwind Templates <a
            href="/"
            class="font-semibold text-indigo-600"
            ><span class="absolute inset-0" aria-hidden="true" />Read more
            <span aria-hidden="true">&rarr;</span></a
          >
        </div>
      </div>
      <div class="text-center">
        <h1 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">
          {herosec.title}
        </h1>
        <p class="mt-6 text-lg leading-8 text-gray-600">{herosec.subtext}</p>
        <div class="mt-10 flex items-center justify-center md:gap-x-6 flex-wrap gap-3">
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border-transparent bg-gray-800 hover:bg-gray-800/90  border border-gray-800 transition-all duration-100  flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-white"
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
            {herosec.btn1}
          </a>
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border hover:bg-zinc-200 border-slate-600 flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-gray-900"
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
            {herosec.btn2}
          </a>
        </div>
      </div>
    </div>
    <div
      class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]"
      aria-hidden="true"
    >
      <div
        class="relative left-[calc(50%+3rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-30 sm:left-[calc(50%+36rem)] sm:w-[72.1875rem]"
        style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)"
      />
    </div>
  </div>
</div>
