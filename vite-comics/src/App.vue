<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppIconTopFooter from './components/AppIconTopFooter.vue'
import AppFooter from './components/AppFooter.vue'
import AppBottomFooter from './components/AppBottomFooter.vue'


export default {
  components: {
    AppHeader,
    AppMain,
    AppIconTopFooter,
    AppFooter,
    AppBottomFooter
  }
}
</script>

<template>
<div class="container-header">
  <div class="container">
    <AppHeader />
  </div>
</div>
<div class="container-main">
  <div class="container">
    <AppMain />
  </div>
</div>
<div class="container-IconTopFooter">
  <div class="container">
    <AppIconTopFooter />
  </div>
</div>
<div class="container-footer">
  <div class="container">
    <AppFooter />
  </div>
</div>
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;
@use './styles/partials/mixins.scss' as *;
</style>

