<template>
  <v-app app>
    <LayoutToolbar />
    <v-main>
      <Nuxt />
    </v-main>
    <LayoutFooter />
    <LayoutNavigation />
  </v-app>
</template>

<script>
import LayoutToolbar from "@/components/Layouts/Toolbar";
import LayoutNavigation from "@/components/Layouts/Navigation";
import LayoutFooter from "@/components/Layouts/Footer";
export default {
  components: {
    LayoutToolbar,
    LayoutNavigation,
    LayoutFooter
  }
};
</script>
