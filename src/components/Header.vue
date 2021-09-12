<template>
  <div class="header bg-cover bg-center bg-no-repeat text-center">
    <nav class="container lg:pl-24 lg:pr-24 pt-6 flex items-center justify-between pl-5 pr-5">
      <div>
        <h2 class="text-white font-bold lg:text-3xl text-2xl py-3">sunnyside</h2>
      </div>
      <div class="text-white text-2xl cursor-pointer lg:hidden" @click="toggleNavbar()">
        <font-awesome-icon :icon="['fas', 'bars']" />
      </div>
      <div :class="{ hidden: !showMenu, absolute: showMenu }" class="absolute top-24 right-0 bottom-40 left-0 m-auto lg:m-0 lg:static bg-transparent lg:flex items-center z-10">
        <ul class="lg:flex lg:items-center lg:justify-between text-white font-medium lg:space-x-10 space-y-6 lg:space-y-0 lg:bg-transparent bg-yellow-300 py-8 w-80 m-auto lg:py-0 lg:w-full lg:m-0">
          <li>
            <a href="#" class="lg:hover:bg-blue-300 lg:hover:bg-opacity-80 focus:text-black lg:focus:bg-white px-7 py-3 rounded-full hover:bg-yellow-400">About</a>
          </li>
          <li>
            <a href="#" class="lg:hover:bg-blue-300 lg:hover:bg-opacity-80 focus:text-black lg:focus:bg-white px-7 py-3 rounded-full hover:bg-yellow-400">Services</a>
          </li>
          <li>
            <a href="#" class="lg:hover:bg-blue-300 lg:hover:bg-opacity-80 focus:text-black lg:focus:bg-white px-7 py-3 rounded-full hover:bg-yellow-400">Projecst</a>
          </li>
          <li>
            <a href="#" class="lg:hover:bg-blue-300 lg:hover:bg-opacity-80 focus:text-black lg:focus:bg-white px-7 py-3 rounded-full hover:bg-yellow-400">Contact</a>
          </li>
        </ul>
      </div>
    </nav>
    <div>
      <h1 class="text-white font-bold font-serif uppercase lg:text-5xl text-3xl tracking-widest mt-12">we are creatives</h1>
    </div>
    <div class="text-white text-9xl animate-bounce mt-5">
      <font-awesome-icon :icon="['fas', 'long-arrow-alt-down']"/>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleNavbar() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>

<style>
.header {
  height: 100vh;
  background-image: url(../assets/image-header.jpg);
}
</style>
