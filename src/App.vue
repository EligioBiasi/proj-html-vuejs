<script>
import AppFooter from "./components/AppFooter.vue";
import AppMain from "./components/AppMain.vue";
import AppHeader from "./components/AppHeader.vue";

export default {
    components:{
      AppMain,
      AppHeader,
      AppFooter,
    }
  }

</script>

<template>
  <AppHeader />
  <AppMain />
  <AppMain />
</template>

<style lang="scss">
 @import './styles/General.scss';
</style>
