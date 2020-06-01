<template>
  <div class="main-layout">
    <menu-container />
    <div class="main-container">
      <router-view />
      <home-container />
    </div>
  </div>
</template>

<script>
  import MenuContainer from '@/containers/MenuContainer.vue';
  import HomeLayout from '@/containers/HomeContainer.vue'

  export default {
    components: {
      'menu-container': MenuContainer,
      'home-container': HomeContainer,
    }
  }
</script>