<template>
  <div class="section_warning">
    <div class="section_warning__container custom_container mx-auto">
      <div class="section_warning__content">
        <div class="section_warning__background">
          <div class="section_warning__background_element"></div>
        </div>
        <v-img
          class="section_warning__chicken"
          src="/images/chicken.png"
          alt="chicken"
        />
        <p class="section_warning__title">Important App Update</p>
        <p class="section_warning__text">
          As we continue making strides toward the release of GalaChain, which
          will provide nearly free transactions throughout the Gala Games
          ecosystem, we have made some important updates to the Inventory
          system. Items that previously appeared in your Treasure Chest will now
          appear in your Inventory as "GC". Moving your GC items to another
          chain (ETH) will involve gas fees, as it is still the same backend
          process of minting items from your Treasure Chest. This is a
          transition towards the user experience that is envisioned once the
          GalaChain is live.
        </p>
        <v-icon class="section_warning__close">mdi-close</v-icon>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
.section_warning {
  .section_warning__content {
    position: relative;
    z-index: 10;
    padding: 20px;
    color: #161618;
    font-size: 14px;
    line-height: 17px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 1fr 1fr;
    grid-template-areas:
      "chicken title title"
      "chicken text text";
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
  }

  .section_warning__chicken {
    // display: none;
    grid-area: chicken;
  }

  .section_warning__title {
    font-weight: 700;
    margin: 0;
    grid-area: title;
  }
  .section_warning__text {
    margin: 0;
    grid-area: title;
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
