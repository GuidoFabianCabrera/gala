<template>
  <div class="section_games">
    <div class="section_games__container custom_container">
      <h3 class="section_games__title">Games</h3>

      <hr class="section_games__separator" />

      <div class="section_games__list">
        <div
          class="section_games__item"
          v-for="(item, i) in this.games"
          :key="i"
        >
          <v-img :aspect-ratio="16 / 9" :src="item" alt="game image" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      games: [
        "/images/game01.png",
        "/images/game02.png",
        "/images/game03.png",
        "/images/game04.jpg",
        "/images/game05.png",
        "/images/game06.png",
        "/images/game07.jpg",
        "/images/game08.png"
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

// -----Section Games
.section_games {
  margin-top: 48px;
  cursor: pointer;

  &__container {
    // max-width: 1183px;
    margin: auto;
  }

  &__title {
    font-size: 24px;
  }

  &__separator {
    margin-bottom: 24px;
    border: 1px solid rgb(56, 58, 69);
  }

  &__list {
    display: grid;
    grid-template-columns: 1;
    grid-gap: 24px;
    padding: 12px 0;

    @include breakpoint(sm) {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
    }

    @include breakpoint(xl) {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
    }
  }

  &__item {
    width: 100%;
    height: 100%;
    box-shadow: 1px 2px 14px 0 rgba(0, 0, 0, 0.15);
  }
}
</style>
