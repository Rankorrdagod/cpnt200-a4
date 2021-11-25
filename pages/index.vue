<template>
  <div>
    <Navigation />
    <Header :pageInfo="siteInfo" />
    <Home :pageInfo="siteInfo" />
    <Footer :pageInfo="siteInfo" />
  </div>
</template>
<script>
export default {
  data() {
    return {
      siteInfo: {
        pageName: "Kitten Zone",
        author: "Evan Burton",
        image: "images/three-kits.jpg",
      },
    };
  },
};
</script>