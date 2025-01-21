<template>
  <div class="columns mx-0 is-flex is-justify-content-center is-relative">
    <div class="column is-10">
      <nav class="navbar bg-33335b mt-15px">
        <div class="navbar-brand">
          <a class="navbar-item">
            <img src="logo.png" alt="">
          </a>
          <a 
            role="button" 
            class="navbar-burger" 
            aria-label="menu" 
            aria-expanded="false" 
            :class="{ 'is-active': isMenuOpen }" 
            @click="toggleMenu"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>
        <div 
          id="navbarBasicExample" 
          class="navbar-menu" 
          :class="{ 'is-active': isMenuOpen }"
        >
          <div class="navbar-end is-align-items-center mr-mobile-20px">
            <NuxtLink to="/transaction" class="has-text-white mr-desktop">
              <div class="is-flex">
                <img src="Add.png" alt="" class="ml-1">
                <p>
                  ثبت تراکنش
                </p>          
              </div>
            </NuxtLink>

            <NuxtLink to="/history" class="has-text-white mr-desktop">
              <div class="is-flex">
                <img src="plus.png" alt="" class="ml-1">
                <p>
                  تاریخچه
                </p>          
              </div>
            </NuxtLink>
          </div>

          <div class="navbar-start mr-mobile-20px">
            <div class="is-flex is-align-items-center has-text-white ml-5">
              <p>
                شعبه تهران
              </p>
              <NuxtLink to="/login">
                <img src="profile.png" alt="" class="mr-3 pt-2 w-35px">
              </NuxtLink>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false, 
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen; 
    },
  },
};
</script>

<style scoped>

@media (max-width: 1024px) {
  .navbar-menu.is-active {
    background-color: rgba(51,51,91,0.58039); 
  }
}
</style>
