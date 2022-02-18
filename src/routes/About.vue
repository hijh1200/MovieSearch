<template>
  <div class="about">
    <div class="name"> {{ name }} </div>
    <div>{{email}}</div>
    <div>{{phone}}</div>
  </div>
</template>

<script>
import { mapState } from 'vuex'
export default {
  
  computed: {
    ...mapState('about', [
      'name',
      'email',
      'phone'
    ])
  },
  
}
</script>

<style lang="scss" scoped>
.about {
  text-align: center;
  .name {
    font-size: 40px;
    font-family: "Oswald", sans-serif;
    margin-bottom: 20px;
  }
}
</style>