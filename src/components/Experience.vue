<template>
    <div class="flex w-full py-10" :class="{'flex-row-reverse':props.inverso}">
        <div class="mx-10 w-1/2">
            <slot name="imagen"></slot>
        </div>
        <div class="mx-10 my-12 w-1/2">
            <h3 class="text-xl font-bold">
                <slot name="header">
                </slot>
            </h3>
            <p class="text-xs py-4">
                <slot></slot>
            </p>
            <div class="py-5 text-[#0EE6B7] flex">
                <slot name="footer">
                </slot>
            </div>
        </div>
    </div>
</template>

<script setup>
const props = defineProps({
    inverso: Boolean
})
</script>

<style scoped>

</style>