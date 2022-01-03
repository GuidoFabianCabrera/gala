<template>
  <div class="nft_card">
    <div class="nft_card__header">
      <div class="nft_card__rarity_container">
        <img
          class="nft_card__rarity"
          :src="`${$router.options.base}${this.rarityImg}`"
          alt="rarity image"
        />
      </div>
      <div class="nft_card__image_container">
        <img
          class="nft_card__image"
          :src="`${$router.options.base}${this.image}`"
          alt="nft_card image"
        />
      </div>
    </div>

    <div class="nft_card__body">
      <div class="nft_card__title">
        {{ this.name }}
      </div>
      <div class="nft_card__price_container">
        <img
          class="nft_card__price"
          src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png"
          alt="coin image"
        />
        <span>{{ this.cost }}</span>
      </div>
      <div class="nft_card__subtitle">
        {{ this.game }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    cost: String,
    game: String,
    image: String,
    rarityImg: String
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.nft_card {
  display: flex;
  flex-direction: column;
  background: rgb(22, 22, 24);
  cursor: pointer;

  // Card header
  &__header {
    position: relative;
  }

  &__rarity_container {
    position: absolute;
    padding: 4px;
    right: 0;
  }
  &__rarity {
    width: 32px;
    height: 32px;
  }

  &__image_container {
    width: 100%;
    height: 100%;
  }
  &__image {
    width: 100%;
    height: 100%;
  }

  // Card body

  &__body {
    height: 100%;
    display: flex;
    flex-direction: column;
    padding: 8px;
  }

  &__title {
    margin: 0;
    font-size: 18px;
    font-weight: 500;
  }

  &__price_container {
    margin-top: auto;
  }
  &__price {
    width: 16px;
    vertical-align: middle;
  }

  &__subtitle {
    margin: 8px 0 0 0;
    font-size: 14px;
  }
}
</style>
