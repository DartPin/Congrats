<template>
  <div class="field">
    <div class="container">
      <div class="row">
        <div class="col-6" v-for="(item, index) of melodies" :key="item.id" v-if="(index < page+8) & (index >= page) "  @click="playMusic()">
          <div class="play-icon">
            <div class="play-triangle"></div>
          </div>
          <div class="melody"> <p> {{item.name}}</p> </div>          
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
      audio.src = '../Music/HappyBirth.mp3'; 
      audio.autoplay = true;
    }
  }
};
</script>

<style src="./Field.css">

</style>
