<template>
  <div class="menu-container">
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/home'}"
      @click="clickMenu('home')"
    >
    Home
    </div>
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/config'}"
      @click="clickMenu('config')"
    >
    Config
    </div>
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/rootchain'}"
      @click="clickMenu('rootchain')"
    >
    RootChain Setup
    </div>
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/operator'}"
      @click="clickMenu('operator')"
    >
    Operator Setup
    </div>
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/usernnode'}"
      @click="clickMenu('operator')"
    >
    Usernode Setup  
    </div>
    <div
      class="menu-title-container"
      :class="{ 'menu-selected': $route.path === '/stake'}"
      @click="clickMenu('stake')"
    >
    Stake/Unstake Tester
    </div>
  </div>
</template>

<script>
  export default {
    methods: {
      clickMenu (path) {
        if (`/${path}` === this.$route.path) {
          return ;
        }
        this.$router.push(`/${path}`).catch(err => {});
      },
    },
  };
</script>

<style scoped>

</style>