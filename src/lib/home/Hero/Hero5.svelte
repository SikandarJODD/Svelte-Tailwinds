<script>
	import { fade, scale } from 'svelte/transition';
  let hero = {
    headtitle: "Mission Travel",
    icon: "https://cdn-icons-png.flaticon.com/512/826/826070.png",
    imgs: [
      "https://images.pexels.com/photos/12919846/pexels-photo-12919846.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
      "https://images.pexels.com/photos/3214944/pexels-photo-3214944.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
      "https://images.pexels.com/photos/12644588/pexels-photo-12644588.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load",
      "https://images.pexels.com/photos/7880463/pexels-photo-7880463.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
    ],
    img: "https://images.pexels.com/photos/3214944/pexels-photo-3214944.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
    title: "Travel. Your money will return. Your time won’t.",
    subtext: "Twice a year, go someplace you’ve never been before.",
    subquote: "Jobs fill your pocket, but adventures fill your soul.",
    btn1: "Book Now",
    btn2: "Search Hotels",
  };
  let i = 0;
  setInterval(() => {
    i++;
    if (i == hero.imgs.length) {
      i = 0;
    }
    hero.img = hero.imgs[i];
  }, 2900);
  // src="https://images.unsplash.com/photo-1498758536662-35b82cd15e29?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2102&q=80"
</script>

<div class="relative bg-white">
  <div class="mx-auto max-w-7xl lg:grid lg:grid-cols-12 lg:gap-x-8 lg:px-8">
    <div
      class="px-6 pb-24 pt-10 sm:pb-32 lg:col-span-7 lg:px-0 lg:pb-56 lg:pt-48 xl:col-span-6"
    >
      <div class="mx-auto max-w-2xl lg:mx-0">
        <div class="flex items-center justify-center md:justify-start gap-3">
          <img class="h-11" src={hero.icon} alt="Your Company" />
          <h1 class="text-2xl md:text-3xl font-bold text-zinc-600">
            {hero.headtitle}
          </h1>
        </div>
        <div class="hidden sm:mt-32 sm:flex lg:mt-16">
          <div
            class="relative rounded-full px-3 py-1 text-sm leading-6 text-gray-500 ring-1 ring-gray-900/10 hover:ring-gray-900/20"
          >
            {hero.subquote}
            <a href="/" class="whitespace-nowrap font-semibold text-indigo-600"
              ><span class="absolute inset-0" aria-hidden="true" />Read more
              <span aria-hidden="true">&rarr;</span></a
            >
          </div>
        </div>
        <h1
          class="mt-12 text-center md:text-left text-3xl font-bold tracking-tight text-gray-900 sm:mt-10 sm:text-6xl md:mt-16"
        >
          {hero.title}
        </h1>
        <p class="mt-6 md:ml-1 text-lg leading-8 text-gray-600">
          {hero.subtext}
        </p>
        <div class="mt-10 flex items-center md:gap-x-6 flex-wrap gap-3">
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border-transparent bg-blue-600 hover:bg-blue-600/90 border border-blue-500 transition-all duration-100 flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-white"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-check-circle"
              ><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14" /><polyline
                points="22 4 12 14.01 9 11.01"
              /></svg
            >
            {hero.btn1}
          </a>
          <a
            href="/"
            class="w-full md:w-fit rounded-md px-3.5 py-2.5 border hover:bg-blue-50 border-slate-600 flex gap-2 justify-center items-center text-sm font-semibold leading-6 text-gray-900"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="20"
              height="20"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="lucide lucide-search"
              ><circle cx="11" cy="11" r="8" /><path d="m21 21-4.3-4.3" /></svg
            >
            {hero.btn2}
          </a>
        </div>
      </div>
    </div>
    <div
      class="relative lg:col-span-5 lg:-mr-8 xl:absolute xl:inset-0 xl:left-1/2 xl:mr-0"
    >
      {#key i}
        <img
        in:fade={{ duration: 1000 }}
          class="aspect-[3/2] w-full bg-gray-50 object-cover lg:absolute lg:inset-0 lg:aspect-auto lg:h-full"
          src={hero.imgs[i]}
          alt="Split Img"
        />
      {/key}
      <!-- Single Image -->
      <!-- <img
          class="aspect-[3/2] w-full bg-gray-50 object-cover lg:absolute lg:inset-0 lg:aspect-auto lg:h-full"
          src={hero.img}
          alt="Split Img"
        /> -->
    </div>
  </div>
</div>
