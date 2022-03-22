<template>
    <div class="bg-[#171A1B] rounded-md border-solid border-2 border-[#4A4A4A] w-full h-min md:h-72 pb-14 mb-5">
        <div class="flex justify-between p-3">
            <div class="flex space-x-3">
                <a href="#" class="nav-dot block w-4 h-4 rounded-full bg-[#FFBD2E]"></a>
                <a href="#" class="nav-dot block w-4 h-4 rounded-full bg-[#FF5F56]"></a>
                <a href="#" class="nav-dot block w-4 h-4 rounded-full bg-[#27C93F]"></a>
            </div>
            <div v-if="props.url" class="bg-[#202226] rounded-md px-24">
                <h5>Matias.Castillo.com</h5>
            </div>
            <div></div>
        </div>
        <slot></slot>
    </div>
</template>

<script setup>
const props = defineProps({
    url: Boolean
})
</script>

<style scoped>

</style>