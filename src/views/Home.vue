<template>
  <div class="home">
    <d-player class="player" :options="options" ref="player"></d-player>
  </div>
</template>

<script>
import VueDPlayer from 'vue-dplayer'
import 'vue-dplayer/dist/vue-dplayer.css'
export default {
  data(){
    return{
      options:{
        video:{
          url:'./video/1.flv',
          type:'flv'
        }
      }
    }
  },
  components: {
    'd-player': VueDPlayer,
  },

}
</script>

<style scoped>
.home{
  width: 60%;
  margin: auto;
}
</style>
