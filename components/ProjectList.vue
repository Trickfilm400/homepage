<template>
  <div class='pt-4'>
    <h1 class='text-white text-8xl text-center'>Projects</h1>
    <div class='mt-12'>
      <git-hub-card lang='ts' starscount='3' link-title='vantage-node' link-url='https://github.com/Trickfilm400/vantage-node' description='Get Data of WeatherStation "Vantage" & Vantage Pro (2)" by Davis instruments via Telnet'/>
      <git-hub-card lang='shell' starscount='0' link-title='generic-nodejs-docker' link-url='https://github.com/Trickfilm400/generic-nodejs-docker' description='A nodejs docker image to run a project without building a new docker everytime'/>
      <git-hub-card link-title='This HomePage' starscount="0" link-url='https://github.com/Trickfilm400/homepage' description='My Homepage with Nuxt.JS' lang='vue' />
      <git-hub-card lang='ts' starscount="2" link-title='senertec-dachs-msr2' link-url='https://github.com/Trickfilm400/senertec-dachs-msr2' description='SenerTec Dachs MSR2 GLT-Ethernet REST API Client' />
      <git-hub-card lang='ts' starscount="0" link-title='typescript-project-scaffolding' link-url='https://github.com/Trickfilm400/typescript-project-scaffolding' description='Create a new typescript project with everything you need to your needs customized in seconds!' />
    </div>
    <h1 class='text-white text-4xl text-center'>and a lot more...</h1>
    <h1 class='text-white text-2xl text-center'>...see them on GitHub</h1>
  </div>
</template>

<script setup lang='ts'>
import GitHubCard from '~/components/ghCard.vue'
</script>

<style scoped>

</style>