<script setup>

const props = defineProps({
    buttonText: String
})

</script>

<template>
    <button class="bg-gray-800 text-white py-2 px-4 rounded cursor-pointer ">
        {{ props.buttonText }}
    </button>
</template>
