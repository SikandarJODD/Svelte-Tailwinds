<script>
  let herosec = {
    title: "Svelte Tailwind Components",
    subtitle: "Increase Conversion.",
    subtext:
      "Boost Your Conversion Rate With Our Tailwind Components. 100% Free To Use!",
    btn1: "Dashboard",
    btn2: "Products",
  };
</script>

<section class="bg-gray-50">
  <div
    class="mx-auto max-w-screen-xl px-4 py-32 lg:flex lg:h-screen lg:items-center"
  >
    <div class="mx-auto max-w-3xl text-center">
      <h1 class="text-3xl font-extrabold sm:text-5xl">
        {herosec.title}
        <strong class="font-extrabold text-blue-600 sm:block">
          {herosec.subtitle}
        </strong>
      </h1>

      <p class="mt-4 sm:text-xl/relaxed text-gray-600 font-light  ">
        {herosec.subtext} 
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-4">
        <a
          class="flex gap-2 justify-center items-center w-full border-transparent rounded bg-blue-600 px-12 py-3 text-sm font-medium text-white shadow hover:bg-blue-700 focus:outline-none focus:ring active:bg-blue-500 sm:w-auto"
          href="/"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="1.6"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-layout"
            ><rect width="18" height="18" x="3" y="3" rx="2" ry="2" /><line
              x1="3"
              x2="21"
              y1="9"
              y2="9"
            /><line x1="9" x2="9" y1="21" y2="9" /></svg
          >
          {herosec.btn1}
        </a>

        <a
          class="flex justify-center gap-2 items-center w-full rounded px-12 py-3 text-sm font-medium border border-slate-600 hover:border-transparent shadow hover:text-white hover:bg-blue-700 focus:outline-none focus:ring active:text-blue-500 sm:w-auto"
          href="/"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="1.6"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="lucide lucide-box"
            ><path
              d="M21 8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16Z"
            /><path d="m3.3 7 8.7 5 8.7-5" /><path d="M12 22V12" /></svg
          >
          {herosec.btn2}
        </a>
      </div>
    </div>
  </div>
</section>
