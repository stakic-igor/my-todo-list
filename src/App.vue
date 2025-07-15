<script setup>
  import SingleTask from './components/SingleTask.vue';

</script>

<template>
 <h1>Welcome to My Todo List</h1>
 <div v-for="i in 5" :key="i">
   <SingleTask />
 </div>
</template>

<style scoped>
</style>
