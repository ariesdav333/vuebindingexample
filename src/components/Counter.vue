<template>
  <div>
    <button class="button-colour" v-on:click="increment">Add me</button> 
    <p>Counter: {{ counter }}</p>
    <p>Clicks: {{ clicks }}</p>
  </div>
</template>

<script>
export default {

  data() {
    return{
 
      clicks: 0
      }
    },
    methods: {
      increment() {
      this.clicks++;
      }
    },
    computed: {
      counter() {
        return this.clicks * 2;
      }
    },
    
 }
</script>


<style>
.button-colour{
  background-color: aquamarine;
}

</style>
