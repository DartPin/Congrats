<template>
  <div class="field">
    <div class="container">
      <div class="row">
        <div class="col-6" v-for="(item, index) of melodies" :key="item.id"   @click="playMusic()">
          <div class="play-icon" v-if="(index < page+8) & (index >= page) ">
            <div class="play-triangle"></div>
          </div>
          <div class="melody" v-if="(index < page+8) & (index >= page) "> <p> {{item.name}}</p> </div>          
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: "Field",
  props:["page", "melodies"],
  components:{    
  },
  data() {
    return {
     
    };
  },
  methods:{
    playMusic(){
      var audio = new Audio(); 
      audio.src = './src/components/Music/HappyBith.mp3'; 
      audio.autoplay = true;
    }
  }
};
</script>

<style src="./Field.css">

</style>
