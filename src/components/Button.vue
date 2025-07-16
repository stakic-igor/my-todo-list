<script setup>

const props = defineProps({
    buttonText: String
})

</script>

<template>
    <button>
        {{ props.buttonText }}
    </button>
</template>
