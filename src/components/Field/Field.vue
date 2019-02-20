<template>
  <div class="field">
    <div class="container">
      <div class="row">
        <div class="col-6" v-for="item of melodies" :key="item.id">
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
  components:{    
  },
  data() {
    return {
      melodies: [
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Поздравляю с днем Рождения!!"
        }
      ]
    };
  }
};
</script>

<style src="./Field.css">

</style>
