<template>
  <div class="page_home">
    <HomeSectionCarousel />

    <HomeSectionWarning v-on:test="updateShowWarning" v-show="!this.close" />

    <HomeSectionNameless />

    <HomeSectionDrops />

    <HomeSectionSellers />

    <HomeSectionGames />

    <HomeSectionBanner />

    <HomeSectionNews />
  </div>
</template>

<script>
import HomeSectionCarousel from "@/components/Home/SectionCarousel";
import HomeSectionWarning from "@/components/Home/SectionWarning";
import HomeSectionNameless from "@/components/Home/SectionNameless";
import HomeSectionDrops from "@/components/Home/SectionDrops";
import HomeSectionSellers from "@/components/Home/SectionSellers";
import HomeSectionGames from "@/components/Home/SectionGames";
import HomeSectionBanner from "@/components/Home/SectionBanner";
import HomeSectionNews from "@/components/Home/SectionNews";

export default {
  components: {
    HomeSectionCarousel,
    HomeSectionWarning,
    HomeSectionNameless,
    HomeSectionDrops,
    HomeSectionSellers,
    HomeSectionGames,
    HomeSectionBanner,
    HomeSectionNews
  },
  data() {
    return {
      close: false
    };
  },
  methods: {
    updateShowWarning(a) {
      this.close = true;
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
.page_home {
  margin-top: 60px;
  background-color: rgb(43, 43, 48);
}
</style>
