<script setup>

const props = defineProps({
    id: Number,
    date: String,
    isCompleted: Boolean,
    title: String,
    description: String
});

</script>

<template>
    <div>
        <p>{{ props.date }}</p>
        <button>delete</button>
    </div>
    <h3>{{ props.title }} - {{ props.id }}</h3>
    <p>{{ props.description }}</p>
    <p>status: {{ props.isCompleted }}</p>
    <button>Done!</button>
</template>