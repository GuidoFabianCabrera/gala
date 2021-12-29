<template>
  <div class="section_banner">
    <div class="section_banner__container custom_container">
      <v-img
        class="section_banner__image"
        :aspect-ratio="2 / 1"
        src="/images/bannerMobile.jpg"
        alt="banner"
      />
      <v-img
        class="section_banner__imageDesktop"
        src="/images/banner.jpg"
        alt="banner"
      />
    </div>
  </div>
</template>

<script>
export default {
  // computed: {
  //   mobile() {
  //     return this.$vuetify.breakpoint.md;
  //   }
  // }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

// -----Section Banner
.section_banner {
  margin-top: 52px;

  &__container {
    margin: auto;
  }

  &__image {
    width: 100%;
    cursor: pointer;

    @include breakpoint(md) {
      display: none;
    }
  }

  &__imageDesktop {
    width: 100%;
    cursor: pointer;
    display: none;
    @include breakpoint(md) {
      display: block;
    }
  }
}
</style>
