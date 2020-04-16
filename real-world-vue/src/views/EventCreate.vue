<template>
  <div>
    <h1>Create an Event, {{user.name}}</h1>
    <p>This Event was created by {{user.id}}</p>
    <ul>
      <li v-for="cat in categories" :key="cat"> {{ cat }}</li>
    </ul>
  </div>
</template>

<script>
import {mapState} from "vuex";
export default {
  computed: 
    mapState(["user", "categories"])
  }
</script>

<style>

</style>