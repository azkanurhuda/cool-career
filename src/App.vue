<template>
  <div class="main-h-full flex flex-col h-screen font-Poppins box-border">
    <NavbarVue />
    <router-view />
    <FooterVue />
  </div>
</template>

<script>
import NavbarVue from './components/Navbar.vue'
import FooterVue from './components/Footer.vue'
export default {
  components: {
    NavbarVue,
    FooterVue
  },
  setup() {
    // Create data / vars

    // Check to see if user is already logged in

    // If user does not exist, need to make app ready

    // Runs when there is a auth state change
    // if user is logged in, this will fire

    return {};
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700&display=swap");
</style>
