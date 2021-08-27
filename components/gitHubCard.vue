<template>
  <div class='mb-3'>
    <div style='border-color: rgba(207,207,207,0.45); border-width: 1.5px' class='border-1 rounded-md text-white w-full max-w-full'>
      <div class='h-auto w-10 inline-block pl-4 pt-4 align-text-bottom'>
        <svg aria-hidden='true' focusable='false' data-prefix='fal' data-icon='book-alt' role='img'
             xmlns='http://www.w3.org/2000/svg' viewBox='0 0 448 512' class='svg-inline--fa fa-book-alt fa-w-14 fa-3x'>
          <path fill='currentColor'
                d='M448 392V24c0-13.3-10.7-24-24-24H80C35.8 0 0 35.8 0 80v368c0 35.35 28.65 64 64 64h372c6.6 0 12-5.4 12-12v-8c0-6.6-5.4-12-12-12h-3.3c-4-20.2-3.2-49.7.4-65.8 8.7-3.6 14.9-12.2 14.9-22.2zm-43.7 88H64c-17.67 0-32-14.33-32-32s14.33-32 32-32h340.3c-2.9 18.8-3.1 43.6 0 64zm11.7-96H64c-11.72 0-22.55 3.38-32 8.88V80c0-26.5 21.5-48 48-48h336v352z'
                class=''></path>
        </svg>
      </div>
      <a class='pl-4 inline-block text-3xl text-blue-500' :href=linkUrl>{{ linkTitle }}</a>
      <p class='pl-4 pt-3 break-all pr-4'>{{ description }}</p>


      <div class='flex-wrap flex'>
        <p class='pb-4 pl-4 pt-3'>

          <span v-if='lang === "ts"' style='border-radius: 50%; background-color: #2B7489' class='w-5 h-5 inline-block align-text-bottom mr-3'></span>
          <span v-if='lang === "js"' style='border-radius: 50%; background-color: #F1E05A' class='w-5 h-5 inline-block align-text-bottom mr-3'></span>
          <span v-if='lang === "shell"' style='border-radius: 50%; background-color: #89E051' class='w-5 h-5 inline-block align-text-bottom mr-3'></span>
          {{ langMapping[lang] }}</p>
        <!-- STAR -->
        <div class='h-9 w-9 inline-block pl-4 pt-4 align-top'>
          <svg aria-hidden='true' focusable='false' data-prefix='far' data-icon='star' role='img'
               xmlns='http://www.w3.org/2000/svg' viewBox='0 0 576 512' class='svg-inline--fa fa-star fa-w-18 fa-3x'>
            <path fill='currentColor'
                  d='M528.1 171.5L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6zM388.6 312.3l23.7 138.4L288 385.4l-124.3 65.3 23.7-138.4-100.6-98 139-20.2 62.2-126 62.2 126 139 20.2-100.6 98z'
                  class=''></path>
          </svg>
        </div>
        <p class='pb-4 pl-4 pt-3'>{{ starscount }}</p>
      </div>
    </div>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'
import { Component, Prop } from 'nuxt-property-decorator'

@Component
export default class gitHubCard extends Vue {
  @Prop({required: true}) readonly linkTitle!: string;
  @Prop({required: true}) readonly linkUrl!: string;
  @Prop({required: true}) readonly description!: string;
  @Prop({required: true}) readonly lang!: "ts" | "js" | "shell";
  @Prop({default: "0"}) readonly starscount: string = "0";

  langMapping = {
    "ts": "Typescript",
    "js": "Javascript",
    "shell": "Shell",
  }
}
</script>
