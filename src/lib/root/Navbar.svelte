<script>
  import { fade, slide } from "svelte/transition";
  import { Menu, X } from "lucide-svelte";
  import { page } from "$app/stores";
  import Logo from "$lib/images/logo.png";
  let nav = {
    title: "Svelte Tailwinds",
    img: Logo,
    listnavs: [
      {
        name: "Home",
        link: "/",
      },
      {
        name: "Components",
        link: "/c",
      },
      {
        name: "About",
        link: "/about",
      },
    ],
  };
  $: isActive = $page.route.id;

  let isMenu = false;
  let isMobileMenu = false;
</script>

<nav class="bg-gray-800  border-b border-slate-500">
  <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
    <div class="relative flex h-16 items-center justify-between">
      <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
        <!-- Mobile menu button-->
        <button
          type="button"
          class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white outline-none"
          aria-controls="mobile-menu"
          aria-expanded="false"
          on:click={() => (isMobileMenu = !isMobileMenu)}
        >
          <span class="absolute -inset-0.5" />
          <Menu class={isMobileMenu ? "hidden" : "block"} />
          <X class={isMobileMenu ? "block" : "hidden"} />
        </button>
      </div>
      <div
        class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start"
      >
        <div class="flex flex-shrink-0 items-center">
          <img class="h-8 w-auto" src={nav.img} alt="Your Company" />
          <a href="/">
            <h1 class="ml-1 text-lg md:text-2xl text-white font-semibold">
              Svelte Tailwind
            </h1></a
          >
        </div>
        <div class="hidden sm:ml-6 sm:block w-full">
          <div class="flex space-x-4 justify-center">
            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->

            {#each nav.listnavs as item}
              <a
                href={item.link}
                class="{isActive === item.link
                  ? 'bg-gray-900 text-white hover:text-blue-100'
                  : 'text-gray-300 hover:bg-gray-700 hover:text-white'} rounded-md px-3 py-2 text-sm font-medium"
                >{item.name}</a
              >
            {/each}
          </div>
        </div>
      </div>
      <div
        class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0"
      >
        <!-- <button
          type="button"
          class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
        >
          <span class="absolute -inset-1.5" />
          <span class="sr-only">View notifications</span>
          <svg
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            aria-hidden="true"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"
            />
          </svg>
        </button> -->

        <!-- Profile dropdown -->
        <div class="relative ml-3">
          <div>
            <button
              type="button"
              class="relative flex rounded-full bg-gray-800 text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
              id="user-menu-button"
              aria-expanded="false"
              aria-haspopup="true"
              on:click={() => (isMenu = !isMenu)}
            >
              <span class="absolute -inset-1.5" />
              <span class="sr-only">Open user menu</span>
              <img
                class="h-8 w-8 rounded-full"
                src="https://i.pinimg.com/564x/f2/5f/91/f25f91130d2b6f2dc7b2c8833f4d2113.jpg"
                alt=""
              />
            </button>
          </div>

          <!--
              Dropdown menu, show/hide based on menu state.
  
              Entering: "transition ease-out duration-100"
                From: "transform opacity-0 scale-95"
                To: "transform opacity-100 scale-100"
              Leaving: "transition ease-in duration-75"
                From: "transform opacity-100 scale-100"
                To: "transform opacity-0 scale-95"
            -->
          <div
            class="{isMenu
              ? 'transform opacity-100 scale-100'
              : 'hidden transform opacity-0 scale-95'} transition ease-out duration-100 absolute right-0 z-10 mt-2 w-48 origin-top-right rounded-md bg-white py-1 shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none"
            role="menu"
            aria-orientation="vertical"
            aria-labelledby="user-menu-button"
            tabindex="-1"
          >
            <!-- Active: "bg-gray-100", Not Active: "" -->
            <a
              href="/"
              class="block px-4 py-2 text-sm text-gray-700"
              role="menuitem"
              tabindex="-1"
              id="user-menu-item-0"
              >Build By <code class="text-blue-500">Sikandar.S.Bhide</code></a
            >
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Mobile menu, show/hide based on menu state. -->
  <div
    class="sm:hidden {isMobileMenu
      ? 'visible'
      : 'hidden'} transition-all duration-150"
    id="mobile-menu"
  >
    <div class="space-y-1 px-2 pb-3 pt-2">
      <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->

      {#each nav.listnavs as item}
        <a
          href={item.link}
          class="{isActive === item.link
            ? 'bg-gray-900 text-white'
            : 'text-gray-300 hover:bg-gray-700 hover:text-white'}  block rounded-md px-3 py-2 text-base font-medium"
          >{item.name}</a
        >
      {/each}
    </div>
  </div>
</nav>
