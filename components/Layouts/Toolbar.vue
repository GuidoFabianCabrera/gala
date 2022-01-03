<template>
  <div class="toolbar">
    <div class="toolbar__container">
      <div class="toolbar__content">
        <div class="toolbar__left">
          <img class="toolbar__logo" src="images/toolbar.png" />
          <div class="toolbar__desktop">
            <v-btn text>About</v-btn>
            <v-btn text>Store</v-btn>
            <v-btn text>Games</v-btn>
            <v-btn text>Nodes</v-btn>
            <v-btn text>Get GALA</v-btn>
            <v-btn text>Careers</v-btn>
          </div>
        </div>

        <div class="toolbar__right">
          <div class="toolbar__discord">
            <v-img
              class="toolbar__discord_logo"
              :src="`${$router.options.base}images/discord01.png`"
              alt="image discord logo"
              aspect-ratio="1"
              width="35"
            />
            <span class="toolbar__discord_text">Join Discord</span>
          </div>
          <div class="toolbar__acount">
            <v-btn small color="primary" outlined>Register</v-btn>
            <v-btn small color="primary">Login</v-btn>
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

.toolbar__content {
  position: fixed;
  z-index: 10;
  top: 0;
  left: 0;
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 4px 16px;
  background-color: #040e1a;

  .toolbar__left {
    display: flex;
    gap: 0 15px;
    align-items: center;
  }

  .toolbar__logo {
    width: 98px;
    height: 100%;
  }

  .toolbar__desktop {
    display: none;
    @include breakpoint(xl) {
      display: block;
    }
  }

  .toolbar__right {
    display: flex;
    gap: 0 15px;
    align-items: center;
  }

  .toolbar__discord {
    display: flex;
    align-items: center;
  }

  .toolbar__discord_text {
    display: none;
    @include breakpoint(sm) {
      display: block;
    }
  }
}
</style>
