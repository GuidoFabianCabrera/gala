<template>
  <div class="page_home pb-15 pt-15" style="background-color: rgb(43, 43, 48)">
    <!-- <HomeSectionCarousel /> -->

    <!-- <HomeSectionWarning /> -->

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
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
</style>
