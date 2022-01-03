<template>
  <div class="section_carousel custom_container mx-auto">
    <v-carousel
      class="section_carousel__mobile"
      cycle
      height="auto"
      hide-delimiter-background
      hide-delimiters
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-img
          :src="`${$router.options.base}${slide.image}`"
          :aspect-ratio="500 / 748.466"
        >
          <div class="section_carousel__content">
            <span class="section_carousel__text">{{ slide.text }}</span>
            <p class="section_carousel__description">
              {{ slide.description }}
            </p>
            <v-btn
              v-show="slide.buttonOutlined"
              color="white"
              elevation="2"
              small
              height="22"
              outlined
              class="section_carousel__button"
              >{{ slide.buttonOutlined }}</v-btn
            >
            <v-btn
              v-show="slide.button"
              color="primary"
              elevation="2"
              small
              height="22"
              class="section_carousel__button"
              >{{ slide.button }}</v-btn
            >
          </div>
        </v-img>
      </v-carousel-item>
    </v-carousel>

    <!-- Desktop version -->

    <v-carousel
      class="section_carousel__desktop"
      cycle
      height="auto"
      hide-delimiter-background
      hide-delimiters
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-img :src="`${$router.options.base}${slide.imageDesktop}`" contain>
          <div class="section_carousel__content">
            <span class="section_carousel__text">{{ slide.text }}</span>
            <p
              class="section_carousel__description"
              :style="{
                color: slide.text == 'STAKE YOUR CLAIM' ? '#000' : ''
              }"
            >
              {{ slide.description }}
            </p>
            <v-btn
              v-show="slide.buttonOutlined"
              color="white"
              elevation="2"
              height="22"
              outlined
              class="section_carousel__button"
              >{{ slide.buttonOutlined }}</v-btn
            >
            <v-btn
              v-show="slide.button"
              color="primary"
              elevation="2"
              height="22"
              class="section_carousel__button"
              >{{ slide.button }}</v-btn
            >
          </div>
        </v-img>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slides: [
        {
          image: "images/carousel01.jpg",
          imageDesktop: "images/carouselDesktop01.jpg",
          text: "JOIN NOW!",
          description:
            "Join before 2022 for an EOE Profile Pic NFT! All new members receive the Town Star Express Depot, eligible for P2E rewards. Plus leaks, exclusives and more!",
          button: "Learn More"
        },
        {
          image: "images/carousel02.jpg",
          imageDesktop: "images/carouselDesktop02.jpg",
          text: "STAKE YOUR CLAIM",
          description:
            "Get out in front of the hordes by grabbing a Dead Claim today. When the land rush begins, the best places will be yours for the taking.",
          button: "ON SALE NOW"
        },
        {
          image: "images/carousel03.jpg",
          imageDesktop: "images/carouselDesktop03.jpg",
          text: "Now Available",
          description:
            "Explore the blue yonder with a Boat, or create a safe haven for seafaring vessels with a Dock. Be ready for your great voyage!",
          button: "Set Sail"
        },
        {
          image: "images/carousel04.jpg",
          imageDesktop: "images/carouselDesktop04.png",
          text: "Live Land Drop!",
          description:
            "Legacy's Land sale is live! Grab a slice of London, one of the world's top economic hubs. Design, make, trade and compete to earn!",
          button: "BUY NOW!"
        },
        {
          image: "images/carousel05.jpg",
          imageDesktop: "images/carouselDesktop05.jpg",
          text: "On Sale Now",
          description:
            "Claim your own piece of galactic property in round 3 of the presale, Aurora's Edge... But hurry, supplies and time are limited!",
          button: "VIEW CLAIMS"
        },
        {
          image: "images/carousel06.jpg",
          imageDesktop: "images/carouselDesktop06.jpg",
          text: "SIGN UP TODAY!",
          description:
            "Gala is a new type of gaming platform, partially owned and operated by its players. Earn Gala tokens by playing and use them to decide the future of the game!",
          buttonOutlined: "SIGN UP!"
        },
        {
          image: "images/carousel07.jpg",
          imageDesktop: "images/carouselDesktop07.jpg",
          text: "Be a Baron!",
          description:
            "Be a Baron! Get rewards from the battles played in your arena!",
          button: "TANK STORE"
        },
        {
          image: "images/carousel08.jpg",
          imageDesktop: "images/carouselDesktop08.jpg",
          text: "NEW WEBSITE",
          description:
            "Place NFTs in your town. Complete Daily Challenges. Earn TownCoin. Welcome to Play-to-Earn. First Season is free for everyone!",
          button: "PLAY TO EARN",
          buttonOutlined: "LEARN MORE"
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

.section_carousel {
  padding-top: 40px;
  .section_carousel__mobile {
    @include breakpoint(sm) {
      display: none;
    }
  }

  .section_carousel__desktop {
    display: none;
    @include breakpoint(sm) {
      display: block;
    }
  }

  .section_carousel__content {
    position: absolute;
    bottom: 0;
    padding: 25px 15px;
    text-align: center;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0.6), #000);
    @include breakpoint(sm) {
      left: 4vw;
      bottom: 4vw;
      width: 40vw;
      text-align: left;
      background: none;
      padding: 0;
    }
  }
  .section_carousel__text {
    position: absolute;
    top: -18px;
    left: -1px;
    padding: 0 12px;
    font-size: 12px;
    font-weight: 700;
    color: #0f0c04;
    background-color: rgb(240, 202, 63);
    @include breakpoint(md) {
      font-size: 16px;
    }
  }

  .section_carousel__description {
    font-size: 14px;
    @include breakpoint(sm) {
      margin: 9px 0 3px;
    }
    @include breakpoint(md) {
      margin-top: 15px;
      font-size: 16px;
    }
  }

  .section_carousel__button {
    font-weight: 700;
    @include breakpoint(md) {
      padding: 15px 35px;
    }
  }
}
</style>
