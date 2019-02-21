<template>
  <div class="footer">
    <div class="btn-panel">
      <button type="button" class="btn btn-secondary prev"  v-bind:disabled="isActivePrev" :class="{ 'btn-light': isActivePrev, 'btn-secondary': !isActivePrev }" @click="prevPage()">&lt;назад</button>
      <button type="button" class="btn btn-secondary next" v-bind:disabled="!isActiveNext" :class="{ 'btn-light': !isActiveNext, 'btn-secondary': isActiveNext }" @click="nextPage()">далее&gt;</button>
      
    </div>
    
  </div>
</template>

<script>

 
export default {
  name: "Footer",
  props:["page", "melodies"],
  components:{    
  },
  data() {
    return {
      isActivePrev: true,
      isActiveNext: true
    };
  },
  methods: {
    nextPage(){
      this.page = this.page + 8;
      this.$emit("page", this.page)
      this.isActivePrev = false;
      if (this.page + 8 >= this.melodies.length){
        this.isActiveNext = false;
      }
    },
    prevPage(){
      this.page = this.page - 8;
      this.$emit("page", this.page)
      this.isActiveNext = true;
      if (this.page === 0){
        this.isActivePrev = true;
      }
    }
  }

};
</script>

<style src="./Footer.css">

</style>
