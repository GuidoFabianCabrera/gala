<template>
  <div class="footer">
    <div class="footer__container">
      <div class="footer__content">
        <div class="footer__help">
          <p class="footer__title">HELP</p>
          <p class="footer__link">FAQs</p>
          <p class="footer__link">Contact Support</p>
        </div>

        <div class="footer__about mx-12">
          <p class="footer__title">ABOUT</p>
          <p class="footer__link">About Us</p>
          <p class="footer__link">Careers</p>
          <p class="footer__link">News</p>
          <p class="footer__link">Environmental Impact</p>
        </div>

        <div class="footer__gala">
          <p class="footer__title">GALA COIN</p>
          <p class="footer__link">Get GALA</p>
          <p class="footer__link">Smart Contact</p>
        </div>

        <div class="footer__separator"></div>

        <div class="footer__social_media">
          <p class="footer__title">JOIN OUR COMMUNITY</p>
          <v-icon class="footer__icon">mdi-twitter</v-icon>
          <v-icon class="footer__icon">mdi-facebook</v-icon>
          <v-icon class="footer__icon">mdi-youtube</v-icon>
          <v-icon class="footer__icon">mdi-discord</v-icon>
        </div>

        <div class="footer__copywrite">
          <span class="footer__copywrite_text">© 2021 Gala Games</span>
          <span class="footer__copywrite_separator">•</span>
          <span class="footer__copywrite_text">Terms and Conditions</span>
          <span class="footer__copywrite_separator">•</span>
          <span class="footer__copywrite_text">Privacy Policy</span>
          <span class="footer__copywrite_separator">•</span>
          <span class="footer__copywrite_text">Launcher EULA</span>
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
.footer {
  margin-bottom: 60px;
  @include breakpoint(lg) {
    margin-bottom: 0px;
  }
  .footer__content {
    display: grid;
    grid-template-columns: auto;
    grid-template-rows: auto;
    padding: 28px 20px;
    background-color: #383a45;
    @include breakpoint(lg) {
      padding: 28px 44px;
      row-gap: 10px;
    }
  }

  .footer__help,
  .footer__about,
  .footer__gala {
    display: flex;
    flex-direction: column;
  }

  .footer__help {
    @include breakpoint(md) {
      grid-column: 1 / 1;
      grid-row: 1 / 1;
    }
  }
  .footer__about {
    grid-column: 2 / 2;
    grid-row: 1 / 1;
  }
  .footer__gala {
    grid-column: 3 / 4;
    grid-row: 1 / 1;
  }

  .footer__title {
    width: 100%;
    margin-bottom: 8px;
    font-weight: 700;
    font-size: 16px;
  }

  .footer__link {
    margin-bottom: 0;
    font-size: 13px;
    font-weight: 300;
    cursor: pointer;
    @include breakpoint(md) {
      font-size: 16px;
    }
  }

  .footer__separator {
    display: none;
    @include breakpoint(md) {
      width: 100%;
      display: block;
      min-width: 15px;
      grid-column: 4 / 6;
      grid-row: 1 / 1;
    }
  }

  .footer__social_media {
    display: flex;
    flex-wrap: wrap;
    padding-top: 24px;
    grid-column: 1 / 4;
    grid-row: 2 / 2;
    @include breakpoint(md) {
      width: fit-content;
      height: fit-content;
      margin-left: auto;
      padding-top: 0px;
      grid-column: 6 / 7;
      grid-row: 1 / 1;
    }
  }

  .footer__icon {
    margin: 15px auto 0;
    padding: 10px;
    border-radius: 50%;
    font-size: 30px;
    cursor: pointer;
    @include breakpoint(md) {
      font-size: 37px;
    }
  }

  .footer__icon:nth-child(2) {
    margin-left: 0;
    @include breakpoint(md) {
      font-size: 37px;
    }
  }

  .footer__icon:nth-child(2) {
    background-color: rgb(29, 161, 242);
  }
  .footer__icon:nth-child(3) {
    background-color: rgb(59, 89, 152);
  }
  .footer__icon:nth-child(4) {
    background-color: rgb(196, 48, 43);
  }
  .footer__icon:nth-child(5) {
    background-color: rgb(114, 137, 218);
  }

  .footer__copywrite {
    margin-top: 16px;
    grid-column: 1 / 4;
    grid-row: 3 / 3;
    color: rgb(147, 159, 168);
    font-size: 14px;
    @include breakpoint(md) {
      grid-column: 1 / 7;
      grid-row: 2 / 2;
    }
  }
  .footer__copywrite_text:first-child {
    display: inline;
  }
  .footer__copywrite_text {
    display: none;
    @include breakpoint(sm) {
      display: inline;
    }
  }
  .footer__copywrite_separator {
    display: none;
    margin: 0 15px;
    @include breakpoint(sm) {
      display: inline;
    }
  }
}
</style>
