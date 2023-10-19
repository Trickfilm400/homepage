<template>
  <div class='block'>
    <h1 class='text-8xl italic text-gray-300 text-center'>Trickfilm400</h1>
    <div class='pt-14'>
      <img class='w-full h-96 rounded-2xl border-black border-2' :src='"/pb.JPG"' alt='ProfilePicture'>
    </div>
    <p class='text-white text-center text-3xl pt-6'>Hey there! 👋</p>
    <p class='text-white text-center pt-6'>
      I am a somewhat professional developer and learned coding myself <br />
      I prefer backend development, because I cannot design UI's, they always look awful :D <br /> <br />
      Interested in DevOps and Developing containerized Node.js Applications in Typescript, using MongoDB / Mysql / Redis and unit-tests, <br />
      also I am a huge fan of <span class='font-bold'>Docker and Kubernetes</span><br />
      At the moment, besides developing some Node.js applications, I play around with microcontrollers (ESP32) and a bit smarthome stuff
    </p>
    <br />
    <h2 class='text-white text-center text-3xl'>Contact</h2>
    <a href='mailto: info@trickfilm400.de' class='text-gray-400 underline hover:text-green-500 ease-in-out duration-300 text-center block'>info@trickfilm400.de</a>
    <p class='text-white text-center'>Discord: @trickfilm400</p>
  </div>
</template>

<script>
export default {
  name: 'ProfileSection'
}
</script>

<style scoped>

</style>