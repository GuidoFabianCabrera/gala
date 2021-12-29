<template>
  <div class="section_carousel custom_container mx-auto">
    <v-carousel cycle height="400" hide-delimiter-background>
      <v-carousel-item
        v-for="(slide, i) in slides"
        :key="i"
        :src="slide"
      ></v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slides: [
        "/images/carousel01.jpg",
        "/images/carousel02.jpg",
        "/images/carousel03.jpg",
        "/images/carousel04.png",
        "/images/carousel05.jpg",
        "/images/carousel06.jpg",
        "/images/carousel07.jpg",
        "/images/carousel08.jpg"
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
.testb {
  // border: 1px solid red;
}
</style>
