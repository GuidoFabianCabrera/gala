<template>
  <div class="section_warning">
    <div class="section_warning__container custom_container mx-auto">
      <div class="section_warning__content">
        <div class="section_warning__background">
          <div class="section_warning__background_element"></div>
        </div>

        <div class="section_warning__left">
          <v-img
            class="section_warning__chicken"
            :src="`${$router.options.base}images/chicken.png`"
            alt="chicken"
            max-width="150"
            contain
          />
        </div>

        <div class="section_warning__right">
          <p class="section_warning__title">Important App Update</p>

          <p class="section_warning__text">
            As we continue making strides toward the release of GalaChain, which
            will provide nearly free transactions throughout the Gala Games
            ecosystem, we have made some important updates to the Inventory
            system. Items that previously appeared in your Treasure Chest will
            now appear in your Inventory as "GC". Moving your GC items to
            another chain (ETH) will involve gas fees, as it is still the same
            backend process of minting items from your Treasure Chest. This is a
            transition towards the user experience that is envisioned once the
            GalaChain is live.
          </p>
        </div>
        <v-icon v-on:click="test" class="section_warning__close"
          >mdi-close</v-icon
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    test() {
      this.$emit("test", true);
    }
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
.section_warning {
  margin-top: 40px;

  .section_warning__content {
    position: relative;
    z-index: 2;
    padding: 20px;
    color: #161618;
    font-size: 14px;
    line-height: 17px;
    display: flex;
    @include breakpoint(sm) {
      font-size: 16px;
      line-height: 21px;
    }
  }

  .section_warning__background {
    overflow: hidden;
    border-right: 5px solid #ce6c21;
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
  }

  .section_warning__background_element {
    position: relative;
    right: -4px;
    width: 100%;
    height: 100%;
    background: transparent linear-gradient(97deg, #f7a728, #dfb013) 0 0
      no-repeat padding-box;
    border: 5px solid #ce6c21;
    z-index: -1;
    @include breakpoint(sm) {
      transform: skewX(-29deg);
      transform-origin: bottom left;
    }
  }

  .section_warning__left {
    display: none;
    width: 25%;
    @include breakpoint(sm) {
      display: block;
      align-self: flex-end;
    }
  }

  // .section_warning__chicken {
  // display: none;
  // width: calc(25% - 29px);
  // }

  .section_warning__right {
    padding-left: 18px;
  }

  .section_warning__title {
    font-weight: 700;
    margin: 0;
  }
  .section_warning__text {
    margin: 0;
  }
  .section_warning__close {
    position: absolute;
    right: 12px;
    top: 12px;
    background: hsla(0, 0%, 43.9%, 0.3);
    border-radius: 50%;
  }
}
</style>
