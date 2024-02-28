<script setup lang="ts">
const props = defineProps({
    image: {
        type: String,
    },
    // class: {
    //   type: String,
    // },  
    // backgroundSize: {
    //   type: String,
    //   default: 'cover',
    // },  
})
</script>
<template>
    <div class="slidev-layout w-full h-full">
        <slot />
        <div class="two-columns grid grid-cols-2 text-justify pt-5">
            <div class="col-left">
                <img :src="image" />
                <slot name="left" />
            </div>
            <div class="col-right">
                <slot name="right" />
            </div>
        </div>
    </div>
</template>