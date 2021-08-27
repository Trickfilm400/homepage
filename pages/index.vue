<template>
  <div class='w-100 h-100'>
    <Header />
    <div class='flex justify-center flex-wrap '>
      <div>
        <ProfileSection />
        <ProjectList />
      </div>
    </div>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'
import ProfileSection from '~/components/ProfileSection.vue'
import Header from '~/components/Header.vue'
import ProjectList from '~/components/ProjectList.vue'

export default Vue.extend({
  components: { ProjectList, Header, ProfileSection }
})
</script>


<style>
body {
  background-color: #121212;
}

</style>
