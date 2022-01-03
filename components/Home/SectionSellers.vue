<template>
  <div class="section_sellers">
    <div class="section_sellers__container custom_container">
      <h3 class="section_sellers__title">Top Sellers</h3>

      <hr class="section_sellers__separator" />

      <div class="section_sellers__list">
        <SharedNftCard
          v-for="(item, i) in this.nftCards"
          :key="i"
          v-bind="item"
        />
      </div>
    </div>
  </div>
</template>

<script>
import SharedNftCard from "@/components/Shared/NftCard";

export default {
  components: {
    SharedNftCard
  },
  data() {
    return {
      nftCards: [
        {
          name: "Cannon (Common Weapon)",
          cost: "342",
          game: "Spider Tanks",
          image: "images/nft06.png",
          rarityImg: "images/rarity02.png"
        },
        {
          name: "Santa's Slay (Common)",
          cost: "2,093",
          game: "Spider Tanks",
          image: "images/nft04.gif",
          rarityImg: "images/rarity02.png"
        },
        {
          name: "Human Exemplar: The Greencloaks",
          cost: "1,361",
          game: "Mirandus",
          image: "images/nft07.png",
          rarityImg: "images/rarity04.png"
        },
        {
          name: "Human Exemplar: The Weavers",
          cost: "1,256",
          game: "Mirandus",
          image: "images/nft09.png",
          rarityImg: "images/rarity04.png"
        },
        {
          name: "Bandit (Common Body)",
          cost: "243",
          game: "Spider Tanks",
          image: "images/nft08.png",
          rarityImg: "images/rarity02.png"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

// -----Section Sellers
.section_sellers {
  margin-top: 48px;

  &__container {
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
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 9px;

    @include breakpoint(sm) {
      grid-template-columns: repeat(2, 1fr);
    }
    @include breakpoint(md) {
      grid-template-columns: repeat(3, 1fr);
    }
    @include breakpoint(lg) {
      grid-template-columns: repeat(4, 1fr);
    }
    @include breakpoint(xl) {
      grid-template-columns: repeat(5, 1fr);
    }
  }
}

// @include breakpoint(xl) {
// }
</style>
