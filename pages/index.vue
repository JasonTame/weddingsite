<template>
  <div class="container flex flex-col">
    <Header />
    <Intro />
    <home-story />
    <div class="flex my-6">
      <home-nav-link></home-nav-link>
      <home-nav-link></home-nav-link>
      <home-nav-link></home-nav-link>
    </div>

    <p class="uppercase">(Yo, this is your formal invitation)</p>
  </div>
</template>

<script>
import Header from "~/components/Header.vue";
import Intro from "~/components/Intro.vue";
import HomeStory from "~/components/HomeStory.vue";
import HomeNavLink from "~/components/HomeNavLink.vue";

export default {
  components: {
    Header,
    Intro,
    HomeStory,
    HomeNavLink
  }
};
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
