<template>
  <div class="container mx-auto my-auto px-2 py-5">
    <div class=" flex flex-1 items-center justify-center">
      <div class="rounded-lg sm:border-2 px-4 lg:px-24 py-16 lg:max-w-xl sm:max-w-md w-full text-center">
        <form class="text-center">
          <h1 class="font-bold tracking-wider text-2xl mb-8 w-full text-gray-600">
            Sign in
          </h1>
          <div class="py-2 text-left">
            <input type="email"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700 "
              placeholder="Email" />
          </div>
          <div class="py-2 text-left">
            <input type="password"
              class="bg-gray-200 border-2 border-gray-100 focus:outline-none bg-gray-100 block w-full py-2 px-4 rounded-lg focus:border-gray-700 "
              placeholder="Password" />
          </div>
          <div class="py-2">
            <button type="submit"
              class="border-2 border-red-100 focus:outline-none bg-primary-red text-white text-xl font-bold tracking-wider block w-full p-2 rounded-lg focus:border-red-700 hover:bg-red-700">
              Sign In
            </button>
          </div>
        </form>
        <div class="text-center mt-10">
          <span class="text-base">
            Don't have an account?
          </span>
          <router-link class="font-light text-md  text-base text-primary-red underline font-semibold hover:text-red-700"
            :to="{ name: 'Register' }">Create
            Account</router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "login",
  setup() {
    // Create data / vars

    // Login function

    return {};
  },
};
</script>
