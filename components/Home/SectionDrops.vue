<template>
  <div class="section_drops">
    <div class="section_drops__container custom_container">
      <h3 class="section_drops__title">Recent Drops</h3>

      <hr class="section_drops__separator" />

      <div class="section_drops__list">
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
          name: "Aurora's Edge - The Shard of Divinity (Ancient)",
          cost: "1.57 m",
          game: "Echoes of Empire",
          image: "images/nft01.gif",
          rarityImg: "images/rarity01.png"
        },
        {
          name: "Aurora's Edge - The Gallows of Time (Ancient)",
          cost: "2.512 m",
          game: "Echoes of Empire",
          image: "images/nft02.gif",
          rarityImg: "images/rarity01.png"
        },
        {
          name: "Aurora's Edge - The Anvil of Gravity",
          cost: "2.198 m",
          game: "Echoes of Empire",
          image: "images/nft03.gif",
          rarityImg: "images/rarity01.png"
        },
        {
          name: "Santa's Slay (Common)",
          cost: "2,093",
          game: "Spider Tanks",
          image: "images/nft04.gif",
          rarityImg: "images/rarity02.png"
        },
        {
          name: "Dead Claim: Georgia (Epic)",
          cost: "276,950",
          game: "The Walking Dead: Empires",
          image: "images/nft05.gif",
          rarityImg: "images/rarity03.png"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";
// -----Section Drops

.section_drops {
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
</style>
