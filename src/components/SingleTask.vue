<script setup>
import Button from './Button.vue';

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
        <Button button-text="Delete" />
    </div>
    <h3>{{ props.title }} - {{ props.id }}</h3>
    <p>{{ props.description }}</p>
    <p>status: {{ props.isCompleted }}</p>
    <Button button-text="Mark as done" />
</template>
