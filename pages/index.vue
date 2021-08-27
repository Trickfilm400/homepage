<template>
  <div class='w-100 h-100'>
    <Header />
    <div class='flex justify-center flex-wrap '>
      <ProfileSection />
    </div>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'
import ProfileSection from '~/components/ProfileSection.vue'
import Header from '~/components/Header.vue'

export default Vue.extend({
  components: { Header, ProfileSection }
})
</script>


<style>
body {
  background-color: #121212;
}

</style>
