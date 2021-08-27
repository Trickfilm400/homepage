<template>
  <div class='pt-4'>
    <h1 class='text-white text-8xl text-center'>Projects</h1>
    <div class='mt-12'>
      <git-hub-card lang='ts' stars-count='2' link-title='vantage-node' link-url='https://github.com/Trickfilm400/vantage-node' description='Get Data of WeatherStation "Vantage" & Vantage Pro (2)" by Davis instruments via Telnet'/>
      <git-hub-card lang='shell' stars-count='0' link-title='generic-nodejs-docker' link-url='https://github.com/Trickfilm400/generic-nodejs-docker' description='A nodejs docker image to run a project without building a new docker everytime'/>
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
