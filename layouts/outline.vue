<script setup lang="ts">

const props = defineProps({
    class: {
        type: String,
    },
})

</script>
<template>
    <div class="slidev-layout slidev-layout-left outline w-full h-full" :class="props.class">
        <slot />
    </div>
</template>