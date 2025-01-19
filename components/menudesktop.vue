<template>
  <div class="columns mx-0 is-flex is-justify-content-center is-relative">
    <div class="column is-10">
      <div class="columns mx-0 bg-33335b is-centered is-mobile mx-0 ">
        <div class="column has-text-white">
          <div class="is-flex is-align-items-center">
            <img src="logo.png" alt="">
            <NuxtLink to="/transaction" class="is-flex is-justify-content-end is-align-items-center mr-4">
              <img src="Add.png" alt="">
              <p class="mr-1">
                ثبت تراکنش
              </p>
             
            </NuxtLink>
            <div class="is-flex is-justify-content-end is-align-items-center mr-4">
              <img src="plus.png" alt="">
              <p class="mr-1">
                تاریخچه
              </p>
              
            </div>

          </div>
        </div>
        <div class="column has-text-left has-text-white">
          <div class="is-flex is-justify-content-end is-align-items-center">
            <p class="ml-3">
              شعبه تهران
            </p>
            <img src="profile.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

    };
  },
};
</script>