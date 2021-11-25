<template>
  <header class="grid justify-items-center p-8 text-8xl bg-green-500 text-pink-200">
    <h1>{{ pageInfo.pageName }}</h1>
  </header>
</template>
<script>
export default {
  props: ["pageInfo"],
};
</script>