<template>
  <div>
    <div class="relative pt-6 px-4 sm:px-6 ">
      <nav
        class="relative flex items-center justify-between sm:h-10 lg:justify-start"
        aria-label="Global"
      >
        <div class="flex items-center flex-grow flex-shrink-0 lg:flex-grow-0">
          <div class="flex items-center justify-between w-full md:w-auto">
            <nuxt-link to="/">
              <span class="font-black ">gotoMA</span>

            </nuxt-link>
            <div class="-mr-2 flex items-center md:hidden">
              <button
                type="button"
                class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
                aria-expanded="false"
              >
                <span class="sr-only">Open main menu</span>
                <!-- Heroicon name: outline/menu -->
                <svg
                  class="h-6 w-6"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  aria-hidden="true"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M4 6h16M4 12h16M4 18h16"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
        <div class="hidden md:block md:ml-10 md:pr-4 md:space-x-8">
          <nuxt-link to="/federalism" class="font-medium text-gray-500 hover:text-gray-900"
            >Federalism</nuxt-link
          >

          <nuxt-link to="/constitution" class="font-medium text-gray-500 hover:text-gray-900"
            >Constitution</nuxt-link
          >

          <nuxt-link to="/branches" class="font-medium text-gray-500 hover:text-gray-900"
            >Branches</nuxt-link
          >

          <nuxt-link to="/localgov" class="font-medium text-gray-500 hover:text-gray-900"
            >Local Gov</nuxt-link
          >

          <nuxt-link to="/taxes" class="font-medium text-gray-500 hover:text-gray-900"
            >Taxes</nuxt-link
          >
        </div>
      </nav>
    </div>

    <!--
          Mobile menu, show/hide based on menu open state.

          Entering: "duration-150 ease-out"
            From: "opacity-0 scale-95"
            To: "opacity-100 scale-100"
          Leaving: "duration-100 ease-in"
            From: "opacity-100 scale-100"
            To: "opacity-0 scale-95"
        -->
    <div
      class="absolute z-10 top-0 inset-x-0 p-2 transition transform origin-top-right md:hidden"
    >
      <div
        class="rounded-lg shadow-md bg-white ring-1 ring-black ring-opacity-5 overflow-hidden"
      >
        <div class="px-5 pt-4 flex items-center justify-between">
          <div>
            <img
              class="h-8 w-auto"
              src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg"
              alt=""
            />
          </div>
          <div class="-mr-2">
            <button
              type="button"
              class="bg-white rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
            >
              <span class="sr-only">Close main menu</span>
              <!-- Heroicon name: outline/x -->
              <svg
                class="h-6 w-6"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M6 18L18 6M6 6l12 12"
                />
              </svg>
            </button>
          </div>
        </div>
        <div class="px-2 pt-2 pb-3 space-y-1">
          <nuxt-link
            to="#"
            class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            >Product</nuxt-link
          >

          <nuxt-link
            to="#"
            class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            >Features</nuxt-link
          >

          <nuxt-link
            to="#"
            class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            >Marketplace</nuxt-link
          >

          <nuxt-link
            to="#"
            class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50"
            >Company</nuxt-link
          >
        </div>
        <nuxt-link
          to="#"
          class="block w-full px-5 py-3 text-center font-medium text-indigo-600 bg-gray-50 hover:bg-gray-100"
        >
          Log in
        </nuxt-link>
      </div>
    </div>
  </div>
</template>
<style scoped>
.nuxt-link-exact-active {
  @apply text-indigo-600 hover:text-indigo-500;
}
</style>