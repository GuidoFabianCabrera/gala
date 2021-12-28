<template>
  <div class="section_drops">
    <div class="section_drops__container custom_container">
      <h3 class="section_drops__title">Recent Drops</h3>

      <hr class="section_drops__separator" />

      <div class="section_drops__list">
        <div class="nft_card" v-for="i in 5" :key="i">
          <div class="nft_card__header">
            <div class="nft_card__rarity">
              <img
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png"
                alt="rarity image"
              />
            </div>
            <div class="nft_card__image">
              <img
                src="https://tokens.gala.games/images/ion-games/echoes-of-empire/celestial-object/auroras-edge-the-shard-of-divinity-ancient.gif"
                alt="nft_card image"
              />
            </div>
          </div>

          <div class="nft_card__body">
            <div class="nft_card__title">
              <p>Aurora's Edge - The Shard of Divinity (Ancient)</p>
            </div>
            <div class="nft_card__price">
              <img
                src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png"
                alt="coin image"
              />
              <span>1.392 m</span>
            </div>
            <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
// -----Section Drops

.section_drops {
  margin-top: 48px;

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
    grid-template-columns: repeat(5, 1fr);
    grid-gap: 9px;
  }
}


// //Nft Card//

.nft_card {
  display: flex;
  flex-direction: column;
  background: rgb(22, 22, 24);
  cursor: pointer;
  // border: 1px solid red;

  // Card header
  &__header {
    position: relative;
  }

  &__rarity {
    position: absolute;
    padding: 4px;
    right: 0;

    & img {
      width: 32px;
      height: 32px;
    }
  }

  &__image {
    width: 100%;
    height: 100%;

    img {
      width: 100%;
      height: 100%;
    }
  }

  // Card body

  &__body {
    padding: 8px;
  }

  &__title {
    & p {
      margin: 0;
      font-size: 18px;
      font-weight: 500;
    }
  }

  &__price {
    & img {
      width: 16px;
      vertical-align: middle;
    }

    // & span{
    //   vertical-align: middle;
    // }
  }

  &__subtitle {
    margin-top: 8px;

    & p {
      margin: 0;
      font-size: 14px;
    }
  }
}
</style>
