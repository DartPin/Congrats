<template>
  <div class="block">
    <Header></Header>
    <Field :page="page" :melodies="melodies"></Field>
    <Footer :page="page" :melodies="melodies" @page="page = $event"></Footer>

  </div>
</template>

<script>
import Header from "../Header/Header.vue"
import Field from "../Field/Field.vue"
import Footer from "../Footer/Footer.vue"

export default {
  name: "Block",
  components:{
    Header,
    Field,
    Footer
  },
  data() {
    return {
      page: 0,
       melodies: [
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
        {
          name: "Поздравляю с днем Рождения!! желаю счастье в личной жизни!"
        },
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
        },
        {
          name: "Поздравляю с днем Рождения!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        },
        {
          name: "Happy Birthday!!!"
        }
      ],
    };
  }
};
</script>

<style src="./Block.css">

</style>
