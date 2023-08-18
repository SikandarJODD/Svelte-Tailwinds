<script>
  let herosec = {
    title: "Life is Short, Build Stuff that Matters",
    subtext: "Create Amazing Content based on Svelte and SvelteKit",
    btn1: "Download",
    btn2: "Write Your Today",
  };
</script>

<div class="bg-white bg">
  <div class="relative isolate px-6 pt-14 lg:px-8">
    <div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-56">
      <div class="hidden sm:mb-8 sm:flex sm:justify-center">
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
        <div
          class="mt-10 flex items-center justify-center md:gap-x-6 flex-wrap gap-3"
        >
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border-transparent bg-gray-800 hover:bg-gray-800/90 border border-gray-800 transition-all duration-100 flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-white"
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
  </div>
</div>

<style>
  .bg {
    background-color: hsla(0, 100%, 99%, 1);
    background-image: radial-gradient(
        at 81% 5%,
        hsla(189, 100%, 69%, 1) 0px,
        transparent 50%
      ),
      radial-gradient(at 3% 3%, hsla(355, 100%, 93%, 1) 0px, transparent 50%),
      radial-gradient(at 86% 60%, hsla(339, 94%, 87%, 1) 0px, transparent 50%),
      radial-gradient(at 14% 85%, hsla(155, 92%, 82%, 1) 0px, transparent 50%),
      radial-gradient(at 88% 75%, hsla(167, 94%, 78%, 1) 0px, transparent 50%),
      radial-gradient(at 37% 80%, hsla(343, 91%, 69%, 1) 0px, transparent 50%);
  }

  @media (max-width: 640px) {
    .bg {
      background: rgb(181, 231, 254);
      background: linear-gradient(
        180deg,
        rgba(181, 231, 254, 1) 16%,
        rgba(255, 235, 242, 1) 93%
      );
    }
  }
</style>
