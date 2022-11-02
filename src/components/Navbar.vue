<template>
  <header>
    <nav class="bg-primary-red border-red-200 px-2 sm:px-4 py-2.5 dark:bg-primary-red">
      <div class="container flex flex-wrap justify-between items-center mx-auto">
        <a href="http://localhost:8081" class="flex items-center">
          <img src="../assets/images/logo.png" class="mr-3 h-6 sm:h-9" alt="Cool Career Logo">
          <span class="self-center text-xl font-semibold whitespace-nowrap text-white dark:text-white">Cool
            Career</span>
        </a>
        <div class="flex md:order-2">
          <router-link type="button" tag="button"
            class="text-primary-red bg-white hover:bg-secondary-red focus:ring-2 focus:outline-none focus:ring-red-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-secondary-red dark:hover:bg-white dark:focus:ring-secondary-red hover:text-white"
            :to="{ name: 'Login' }">Login</router-link>
          <button data-collapse-toggle="navbar-cta" type="button"
            class="inline-flex items-center p-2 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
            aria-controls="navbar-cta" aria-expanded="false">
            <span class="sr-only">Open main menu</span>
            <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd"
                d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                clip-rule="evenodd"></path>
            </svg>
          </button>
        </div>
        <div class="hidden justify-between items-center w-full md:flex md:w-auto md:order-1" id="navbar-cta">
          <ul
            class="flex flex-col p-4 mt-4 border border-gray-100 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0 md:bg-primary-red dark:bg-primaryred md:dark:bg-primary-red dark:border-primary-red">
            <li>
              <router-link to="/"
                class="block py-2 pr-4 pl-3 text-white bg-white rounded md:bg-transparent md:text-white md:p-0 dark:text-white"
                aria-current="page">Jobs</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>

</template>

<script>
export default {
  setup() {
    // Get user from store

    // Setup ref to router

    // Logout function

    return {};
  },
};
</script>
