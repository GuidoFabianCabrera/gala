<template>
  <div class="section_news">
    <div class="section_news__container custom_container">
      <h3 class="section_news__title">News</h3>

      <hr class="section_news__separator" />

      <div class="section_news__list">
        <SharedNewsCard v-for="(item, i) in this.new" :key="i" v-bind="item" />
      </div>
    </div>
  </div>
</template>

<script>
import SharedNewsCard from "@/components/Shared/NewsCard";

export default {
  components: {
    SharedNewsCard
  },
  data() {
    return {
      new: [
        {
          title: "Join the Club… Gala Gold!",
          text: `Join the Club… Gala Gold TL;DR-Upgrade to Gala Gold before the end of the year to get an exclusive Echoes of Empire Profile Character Avatar… among other things. If you haven’t heard about the exclusive Gala Games membership club known as Gala Gold, we’re slightly concerned for you safety....`,
          image: "images/new01.jpeg"
        },
        {
          title: "The Woes of Distributed Consensus",
          text: `TLDR: There was no hack in the VOX drop, no contract vulnerabilities, etc. There are some fundamental weaknesses in the way ETH handles randomness which were exploited by someone pointing a massive amount of hashpower to break down some of the random aspects. This is why we are building...`,
          image: "images/new02.png"
        },
        {
          title: "Mirandus VOX-The Great Revealing",
          text: `Mirandus VOX-The Great Revealing 8888 unique Mirandus VOX have until now been nestled snug in their Boxes, but today the time of Revealing has come. Until each VOX Box is exchanged (sent to the VOX contract), the individual provably random VOX have not...`,
          image: "images/new03.png"
        },
        {
          title: "Genesis Curry Flow NFTs",
          text: `Stephen Curry of the Golden State Warriors made history last Tuesday evening when he sunk his 2974th 3-pointer, a nothing-but-net beauty that set the Madison Square Garden crowd into a roar. The lifetime 3-point record is now his, and to celebrate, Under Armour is “Changing the Game for Good”...`,
          image: "images/new04.jpg"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.section_news {
  margin-top: 48px;
  padding-bottom: 58px;

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
    grid-template-columns: 100%;
    grid-gap: 24px;

    @include breakpoint(md) {
      display: grid;
      grid-template-columns: repeat(2, calc(50% - 12px));
    }
  }
}
</style>
