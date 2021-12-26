<template>
  <div class='pt-4'>
    <h1 class='text-white text-8xl text-center'>Projects</h1>
    <div class='mt-12'>
      <git-hub-card lang='ts' starscount='2' link-title='vantage-node' link-url='https://github.com/Trickfilm400/vantage-node' description='Get Data of WeatherStation "Vantage" & Vantage Pro (2)" by Davis instruments via Telnet'/>
      <git-hub-card lang='shell' starscount='0' link-title='generic-nodejs-docker' link-url='https://github.com/Trickfilm400/generic-nodejs-docker' description='A nodejs docker image to run a project without building a new docker everytime'/>
      <git-hub-card link-title='This HomePage' link-url='https://github.com/Trickfilm400/homepage' description='My Homepage with Nuxt.JS' lang='vue' />
      <git-hub-card lang='ts' link-title='simple-dmx-control' link-url='https://github.com/Trickfilm400/simple-dmx-control' description='Simple Web-App to control lights over DMX with a Tinkerforge DMX Bricket' />
      <git-hub-card lang='ts' link-title='advent-calendar-api' link-url='https://github.com/Trickfilm400/advent-calendar-api' description='A simple and small API for any advent-caneldar-website to fetch some kind of data' />
    </div>
  </div>
</template>

<script lang='ts'>
import GitHubCard from '~/components/gitHubCard.vue'
export default {
  name: 'ProjectList',
  components: { GitHubCard },
}
</script>

<style scoped>

</style>
