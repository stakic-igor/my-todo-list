<script setup>
  import Header from './components/Header.vue';
  import SingleTask from './components/SingleTask.vue';


  const tasks = [
    { id: 1, isCompleted: false, date: '15. 7. 2025', title: 'Task 1', description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam, quibusdam.' },
    { id: 2, isCompleted: false, date: '16. 7. 2025', title: 'Task 2', description: 'Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
    { id: 3, isCompleted: true, date: '17. 7. 2025', title: 'Task 3', description: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.' },
    { id: 4, isCompleted: true, date: '18. 7. 2025', title: 'Task 4', description: 'Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.' },
    { id: 5, isCompleted: false, date: '19. 7. 2025', title: 'Task 5', description: 'Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.' }
  ];

</script>

<template>
  <Header />
 <div v-for="task in tasks" :key="task.id">
  <SingleTask 
    :id="task.id"
    :title="task.title"
    :description="task.description" 
    :date="task.date"
    :isCompleted="task.isCompleted"
    />
 </div>
</template>

<style scoped>
</style>
