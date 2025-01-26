<template>
  <div v-on:click="countClicks">
    <h2>{{ name }}</h2>  
    <p>{{ message }}</p>
    <p id="red">You have clicked me {{ clicks }} times.</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Mangoes',
      message: 'I like Mangoes',
      clicks: 0
    }
  }
}
</script>

<style>
  #app > div {
    border: dashed black 1px;
    display: inline-block;
    width: 120px;
    margin: 10px;
    padding: 10px;
    background-color: lightyellow;
  }
  #app > div:hover {
    cursor: pointer;
  }
</style>