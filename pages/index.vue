<template>
  <div>
  <Header :pageInfo="siteInfo" />
    <Navigation />
    
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