<template>
  <header class="grid justify-items-center p-8 text-6xl bg-green-500">
    <h1>{{ pageInfo.pageName }}</h1>
  </header>
</template>
<script>
export default {
  props: ["pageInfo"],
};
</script>