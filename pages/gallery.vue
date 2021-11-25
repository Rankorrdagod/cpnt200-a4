<template>
  <div>
  <Header :pageInfo="siteInfo" :galleries="galleries" />
    <Navigation />
    
    <main class="flex justify-evenly gap-x-16 gap-y-16 flex-wrap p-16 bg-pink-200">
      <Gallery :pageInfo="siteInfo" v-for="gallery in galleries" :key="gallery.id" :info="gallery" />
    </main>
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
        
      },
galleries: [
        {
          title: "Kittens Sleeping",
          description: "Two kittens sleeping on a hot day out in the sun.",
          credit: "luxstorm",
          image: "images/sleepy-kits.jpg",
        },
         {
          title: "Serene Kitten",
          description: "A serene kitten enjoying his day and contemplating his life choices.",
          credit: "luxstorm",
          image: "images/serene-kit.webp",
        },
         {
          title: "Blue Eyes White Kitten",
          description: "I summon my Blue Eyes White Kitten dealing 3000 dmg to your life!",
          credit: "luxstorm",
          image: "images/white-kit.webp",
        },
        {
          title: "Fence Kitten",
          description: "Just a wee little kitten sitting on a fence on a cloudy day.",
          credit: "luxstorm",
          image: "images/little-kit.jpg",
        },


      ],
    };
  },
};
</script>