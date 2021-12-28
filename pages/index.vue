<template>
  <div class="page_home pb-15 pt-15" style="background-color:rgb(43, 43, 48);">

    <div class="custom_container--xl mx-auto">
      <v-carousel
    cycle
    height="400"
    hide-delimiter-background
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        :color="colors[i]"
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-h2">
            {{ slide }} Slide
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
    </div>


    <!-- Test -->

    <div class="custom_container--xl mx-auto">
      <v-row>
        <v-col cols="6">
          <v-card class="d-flex flex-no-wrap justify-space-between">
            <v-col cols="4" class="align-self-center">
              <v-img src="https://tokens.gala.games/compressed-images/node-laptop-founders-final.png"></v-img>
            </v-col>
            <v-col cols="8">
              <v-card-subtitle class="text-h6 pl-0">Receive rewards like GALA, limited edition NFTs and help the Gala Games ecosystem grow.</v-card-subtitle>
              <v-btn color="primary" elevation="2">Learn more</v-btn>
            </v-col>
        </v-card>
        </v-col>
        <v-col cols="6">
          <v-card class="d-flex flex-no-wrap justify-space-between">
            <v-col cols="4" class="align-self-center">
              <v-img 
              class="mx-auto"
              max-height="130"
              width="130"
              src="https://app.gala.games/_nuxt/img/Discord-Logo-White.28174a3.png"></v-img>
              <v-img 
              class="mt-n2 mx-auto"
              width="110"
              src="https://app.gala.games/_nuxt/img/discord_socialpics.a2da892.png"></v-img>
            </v-col>
            <v-col cols="8">
              <v-card-subtitle class="text-h6 pl-0">Join our vibrant community of gamers and NFT enthusiasts to learn all the latest tips and tricks.</v-card-subtitle>
              <v-btn color="primary" elevation="2">Join Discord</v-btn>
            </v-col>
          </v-card>
        </v-col>
      </v-row>
    </div>

    <!-- Test -->

    <div class="section_drops">
      <div class="section_drops__container custom_container--xl">
        <h3 class="section_drops__title">Recent Drops</h3>

        <hr class="section_drops__separator">

        <div class="section_drops__list">
          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="section_sellers">
      <div class="section_sellers__container custom_container--xl">
        <h3 class="section_sellers__title">Top Sellers</h3>

        <hr class="section_sellers__separator">

        <div class="section_sellers__list">
          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>

          <div class="nft_card">
            <div class="nft_card__header">
              <div class="nft_card__rarity">
                <img 
                src="https://tokens.gala.games/images/sandbox-games/rarity/ancient.png" 
                alt="rarity image">
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
                <p>
                  Aurora's Edge - The Shard of Divinity (Ancient)
                </p>
              </div>
              <div class="nft_card__price">
                <img src="https://app.gala.games/_nuxt/img/GALA-icon.b642e24.png" alt="coin image">
                <span>1.392 m</span>
              </div>
              <div class="nft_card__subtitle"><p>Echoes of Empire</p></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="section_games">
      <div class="section_games__container custom_container--xl">
        <h3 class="section_games__title">Games</h3>

        <hr class="section_games__separator" />

        <div class="section_games__list">
          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>

          <div class="section_games__item">
            <img
              src="https://static.gala.games/images/mirandus/mirandus_game_image_boats_docks.png"
              alt="game image"
            />
          </div>
        </div>
      </div>
    </div>

    <div class="section_banner">
      <div class="section_banner__container custom_container--xl">
        <img
          class="section_banner__image"
          src="https://static.gala.games/images/banners/the-walking-dead/twd-banner-desktop.jpg"
          alt="banner"
        />
      </div>
    </div>

    <div class="section_news">
      <div class="section_news__container custom_container--xl">
        <h3 class="section_news__title">News</h3>

        <hr class="section_news__separator">

        <div class="section_news__list">
          <div class="news_card">
            <div class="news_card__left">
              <div class="news_card__image">
                <img src="https://cdn-images-1.medium.com/max/1024/1*hAPNw7J0vnO6Swq6WCQenw.png" alt="news image">
              </div>
            </div>
            <div class="news_card__right">
              <div class="news_card__title mb-3">
                <h6>The Woes of Distributed Consensus</h6>
              </div>
              <div class="news_card__description mb-3">
                <p>TLDR: There was no hack in the VOX drop, no contract vulnerabilities, etc. There are some fundamental weaknesses in the way ETH handles randomness which were exploited by someone pointing a massive amount of hashpower to break down some of the random aspects. This is why we are building...</p>
              </div>
              <div class="news_card__footer">
                <button class="button">Read More</button>
              </div>
            </div>
          </div>
          
          <div class="news_card">
            <div class="news_card__left">
              <div class="news_card__image">
                <img src="https://cdn-images-1.medium.com/max/1024/1*hAPNw7J0vnO6Swq6WCQenw.png" alt="news image">
              </div>
            </div>
            <div class="news_card__right">
              <div class="news_card__title mb-3">
                <h6>The Woes of Distributed Consensus</h6>
              </div>
              <div class="news_card__description mb-3">
                <p>TLDR: There was no hack in the VOX drop, no contract vulnerabilities, etc. There are some fundamental weaknesses in the way ETH handles randomness which were exploited by someone pointing a massive amount of hashpower to break down some of the random aspects. This is why we are building...</p>
              </div>
              <div class="news_card__footer">
                <button class="button">Read More</button>
              </div>
            </div>
          </div>
          <div class="news_card">
            <div class="news_card__left">
              <div class="news_card__image">
                <img src="https://cdn-images-1.medium.com/max/1024/1*hAPNw7J0vnO6Swq6WCQenw.png" alt="news image">
              </div>
            </div>
            <div class="news_card__right">
              <div class="news_card__title mb-3">
                <h6>The Woes of Distributed Consensus</h6>
              </div>
              <div class="news_card__description mb-3">
                <p>TLDR: There was no hack in the VOX drop, no contract vulnerabilities, etc. There are some fundamental weaknesses in the way ETH handles randomness which were exploited by someone pointing a massive amount of hashpower to break down some of the random aspects. This is why we are building...</p>
              </div>
              <div class="news_card__footer">
                <a class="button">Read More</a>
              </div>
            </div>
          </div>
          <div class="news_card">
            <div class="news_card__left">
              <div class="news_card__image">
                <img src="https://cdn-images-1.medium.com/max/1024/1*hAPNw7J0vnO6Swq6WCQenw.png" alt="news image">
              </div>
            </div>
            <div class="news_card__right">
              <div class="news_card__title mb-3">
                <h6>The Woes of Distributed Consensus</h6>
              </div>
              <div class="news_card__description mb-3">
                <p>TLDR: There was no hack in the VOX drop, no contract vulnerabilities, etc. There are some fundamental weaknesses in the way ETH handles randomness which were exploited by someone pointing a massive amount of hashpower to break down some of the random aspects. This is why we are building...</p>
              </div>
              <div class="news_card__footer">
                <button class="button">Read More</button>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
      return {
        colors: [
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ],
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
      }
    },
};
</script>

<style lang="scss" scoped>
@import "@/assets/scss/utils";

// Button
.button{
  border-radius: 4px;
  height: 1.6em;
  padding: 0 12px;
  background-color: rgb(38, 138, 239);
  color: white;
  font-weight: 700;
}

// //Nft Card//

.nft_card {
  display: flex;
  flex-direction: column;
  background: rgb(22, 22, 24);
  cursor: pointer;
  // border: 1px solid red;

  // Card header
  &__header{
    position: relative;
  }

  &__rarity{
    position: absolute;
    padding: 4px;
    right: 0;

    & img{
    width: 32px;
    height: 32px;
    }
  }

  &__image {
    width: 100% ;
    height: 100%;

    img{
      width: 100%;
      height: 100%;
  }
  }

  // Card body

  &__body{
    padding: 8px;
  }

  &__title{
    & p{
      margin: 0;
      font-size: 18px;
      font-weight: 500;
    }
  }

  &__price {
    
    & img{
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

// //News Card//

.news_card {
  display: flex;
  flex-direction: row;
  background: rgb(22, 22, 24);
  border-radius: 4px;

  // News Card left

  &__left{
    max-width: 50%;
    // flex: 1 1 0%;
  }

  &__image{
    height: 100%;
    padding: 12px;

    & img{
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: left;
    }
  }

  // News Card Right

  &__right{
    // flex: 1 1 0%;
    max-width: 50%;
    padding: 12px;
  }

  &__title{

    & h6{
      font-size: 18px;
    }
  }

  &__description{
    
    & p {
      font-size: 14px
    }
  }

}


// -----Section Drops

.section_drops{
  margin-top: 48px;

    &__container{
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

  &__list{
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-gap: 9px;
  }
}

// -----Section Sellers

.section_sellers{
  margin-top: 48px;

  &__container{
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

  &__list{
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-gap: 9px;
  }

}

// -----Section Games


.section_games {
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
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 24px;
    padding: 12px 0;
  }

  &__item {
    width: 100%;
    height: 100%;
    min-height: 160px;
    box-shadow: 1px 2px 14px 0 rgba(0, 0, 0, 0.15);

    & img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      border-radius: 4px;
      cursor: pointer;
    }
  }
}

// -----Section Banner

.section_banner {
  margin-top: 52px;

  &__container {
    margin: auto;
    // max-width: 1183px;
  }

  &__image {
    width: 100%;
    cursor: pointer;
  }
}

// -----Section News

.section_news{
  margin-top: 48px;

    &__container{
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

  &__list{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 24px;
  }
}

</style>
