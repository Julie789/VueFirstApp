<template>
  <div class="about">
    <h1>This is ToDo List developed by {{ their_name }} </h1>
    <p>This website is developed to learn basics of Vue Js.</p>
    <p>I implemented the different concepts of the framework</p>
    <p>including components, templating, styling, forms, animation,</p>
    <p>routing. The App is to add skills in a list-style.</p>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      their_name: this.$route.params.name
    }
  }
}
</script>

<style scoped>
  p {
    text-align:center;
    padding: 10px 0;
    color: gray;
    line-height: 10px;
    margin: 0;
  }
</style>