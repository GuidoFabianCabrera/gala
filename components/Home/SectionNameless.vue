<template>
  <div class="section_nameless">
    <div class="section_nameless__container custom_container mx-auto">
      <div class="section_nameless__gala">
        <h4 class="section_nameless__title">Get a Gala Node</h4>
        <div class="section_nameless__card">
          <div class="section_nameless__left">
            <v-img
              class="section_nameless__image_gala"
              :src="`${$router.options.base}images/gala.png`"
              alt="gala pc"
            />
          </div>
          <div class="section_nameless__right">
            <div class="section_nameless__text">
              <p>
                Receive rewards like GALA, limited edition NFTs and help the
                Gala Games ecosystem grow.
              </p>
            </div>
            <button class="button">Learn More</button>
          </div>
        </div>
      </div>
      <div class="section_nameless__discord">
        <h4 class="section_nameless__title">Join Our Community</h4>
        <div class="section_nameless__card">
          <div class="section_nameless__left">
            <v-img
              class="section_nameless__image_discord"
              :src="`${$router.options.base}images/discord01.png`"
              alt="discord image"
            />
            <v-img
              class="section_nameless__image_users"
              :src="`${$router.options.base}images/discord02.png`"
              alt="users image"
            />
          </div>
          <div class="section_nameless__right">
            <div class="section_nameless__text">
              <p>
                Join our vibrant community of gamers and NFT enthusiasts to
                learn all the latest tips and tricks.
              </p>
            </div>
            <button class="button">Join Discord</button>
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

.button {
  border-radius: 4px;
  height: 1.6em;
  padding: 0 12px;
  background-color: rgb(38, 138, 239);
  color: white;
  font-weight: 700;
}

.section_nameless {
  margin-top: 30px;

  .section_nameless__container {
    display: flex;
    flex-direction: column;
    flex-grow: 10px;

    @include breakpoint(lg) {
      flex-direction: row;
      justify-content: space-between;
    }
  }

  .section_nameless__gala,
  .section_nameless__discord {
    padding: 12px 0;
    @include breakpoint(lg) {
      width: calc(50% - 12px);
    }
  }

  .section_nameless__card {
    display: flex;
    align-items: center;
    border-radius: 4px;
    background-color: rgb(22, 22, 24);
    box-shadow: 1px 2px 14px 0 rgba(0, 0, 0, 0.15);
    @include breakpoint(lg) {
      min-height: 168px;
    }
  }

  .section_nameless__title {
    margin-bottom: 8px;
    font-size: 22px;
  }

  .section_nameless__left {
    width: 100%;
    max-width: 35%;
    padding: 12px;
  }

  .section_nameless__right {
    width: 100%;
    max-width: 100%;
    padding: 12px;
  }

  .section_nameless__image_discord {
    width: 100%;
    max-width: 130px;
    margin: auto;
  }

  .section_nameless__image_users {
    width: 80%;
    max-width: 112px;
    margin: -15px auto 0 auto;
  }
}
</style>
