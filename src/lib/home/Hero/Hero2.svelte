<script>
  let herosec = {
    title: "Build Better Websites",
    subtitle: "Customize Web",
    subtext:
      "Boost Your Conversion Rate With Our Tailwind Components. 100% Free To Use!",
    btn1: "Database",
    btn2: "Create Content",
  };
</script>

<section class="bg-gray-900 text-white">
  <div
    class="mx-auto max-w-screen-xl px-4 py-32 lg:flex lg:h-screen lg:items-center"
  >
    <div class="mx-auto max-w-3xl text-center">
      <h1
        class="bg-gradient-to-r from-green-300 via-blue-500 to-purple-600 bg-clip-text text-3xl font-extrabold text-transparent sm:text-5xl"
      >
        {herosec.title}

        <span class="sm:block"> {herosec.subtitle}</span>
      </h1>

      <p class="mx-auto mt-4 max-w-xl sm:text-xl/relaxed">
        {herosec.subtext}
      </p>

      <div class="mt-8 flex flex-wrap justify-center gap-4">
        <a
          class=" flex gap-2 items-center justify-center w-full rounded border border-blue-600 bg-blue-600 px-12 py-3 text-sm font-medium text-white hover:bg-transparent hover:text-white focus:outline-none focus:ring active:text-opacity-75 sm:w-auto"
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
            class="lucide lucide-database-zap"
            ><ellipse cx="12" cy="5" rx="9" ry="3" /><path
              d="M3 5V19A9 3 0 0 0 15 21.84"
            /><path d="M21 5V8" /><path d="M21 12L18 17H22L19 22" /><path
              d="M3 12A9 3 0 0 0 14.59 14.87"
            /></svg
          >
          {herosec.btn1}
        </a>

        <a
          class="flex gap-2 items-center justify-center w-full rounded border border-blue-600 px-12 py-3 text-sm font-medium text-white hover:bg-blue-600 focus:outline-none focus:ring active:bg-blue-500 sm:w-auto"
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
            class="lucide lucide-plus-circle"
            ><circle cx="12" cy="12" r="10" /><path d="M8 12h8" /><path
              d="M12 8v8"
            /></svg
          >
          {herosec.btn2}
        </a>
      </div>
    </div>
  </div>
</section>
