<template>
  <div class="news_card">
    <div class="news_card__left">
      <div class="news_card__imageContainer">
        <v-img
          position="left"
          aspect-ratio="1"
          class="news_card__image"
          :src="`${$router.options.base}${this.image}`"
          alt="news image"
        />
      </div>
    </div>
    <div class="news_card__right">
      <h6 class="news_card__title mb-3">
        {{ this.title }}
      </h6>
      <p class="news_card__description mb-3">
        {{ this.text }}
      </p>
      <div class="news_card__footer">
        <button class="button">Read More</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    text: String,
    image: String
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.button {
  border-radius: 4px;
  height: 1.6em;
  padding: 0 12px;
  background-color: rgb(38, 138, 239);
  color: white;
  font-weight: 700;
}

.news_card {
  display: flex;
  flex-direction: column;
  background: rgb(22, 22, 24);
  border-radius: 4px;
  box-shadow: 1px 2px 14px 0 rgba(0, 0, 0, 0.15);

  @include breakpoint(sm) {
    flex-direction: row;
  }
  @include breakpoint(md) {
    flex-direction: column;
  }
  @include breakpoint(lg) {
    flex-direction: row;
  }

  // News Card left

  &__left {
    width: 100%;
    padding: 12px;

    @include breakpoint(sm) {
      max-width: 50%;
    }
    @include breakpoint(md) {
      max-width: 100%;
    }
    @include breakpoint(lg) {
      max-width: 50%;
    }
  }

  &__imageContainer {
    height: 100%;
  }

  // &__image {
  // }

  // News Card Right

  &__right {
    padding: 12px;
    width: 100%;

    @include breakpoint(sm) {
      max-width: 50%;
    }
    @include breakpoint(md) {
      max-width: 100%;
    }
    @include breakpoint(lg) {
      max-width: 50%;
    }
  }

  &__title {
    font-size: 18px;
  }

  &__description {
    font-size: 14px;
  }
}
</style>
