<template>
  <div>
    <input type="text" v-on:input="cssClass = $event.target.value"> 
    <p v-bind:class="cssClass">Type in a colour to change my background: {{ cssClass }}</p>
  </div>
</template>

<script>
export default {

  data() {
    return{
      cssClass: ''
      }
    }
 }
</script>


<style>
.red{
  background-color: red;
}
.blue{
  background-color: blue;
}
.green{
  background-color: green;
}
.yellow{
  background-color: yellow;
}

</style>
