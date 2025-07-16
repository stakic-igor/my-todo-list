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
    <div class="flex flex-row">
        <p class="text-sm text-gray-500">{{ props.date }}</p>
        <Button button-text="Delete" />
    </div>
    <h3 class="text-xl">{{ props.title }} - {{ props.id }}</h3>
    <p>{{ props.description }}</p>
    <p>status: {{ props.isCompleted }}</p>
    <Button button-text="Mark as done" />
</template>
