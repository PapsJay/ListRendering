<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <transition-group name="tweets" tag="div">
      <tweet-component />
    </transition-group>
  </div>
</template>

<script>
import TweetComponent from "./app/components/TweetComponent.vue";

export default {
  name: "App",

  components: {
    TweetComponent,
  },
};
</script>

<style lang="scss" scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#app .tweets-move {
  transition: transform 1s;
}
</style>
