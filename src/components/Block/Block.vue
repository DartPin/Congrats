<template>
  <div class="block">
    <Header></Header>
    <Field></Field>
  </div>
</template>

<script>
import Header from "../Header/Header.vue"
import Field from "../Field/Field.vue"

export default {
  name: "Block",
  components:{
    Header,
    Field
  },
  data() {
    return {};
  }
};
</script>

<style src="./Block.css">

</style>
