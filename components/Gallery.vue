<template>
  <div>
    <figure>
      <div class="text-pink-600 text-center bg-black" v-html="`<h3>${info.title}</h3>`"></div>
      <nuxt-img :src="info.image" sizes="sm:300px md:400px lg:500px" />
      <figcaption class="text-center bg-black text-pink-600"v-text="info.description" />
      <p class="bg-black text-pink-600 text-center" v-text="info.credit" />
    </figure>
  </div>
</template>
<script>
export default {
  props: ["pageInfo", "info"],
};
</script>