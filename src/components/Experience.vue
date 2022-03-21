<template>
    <div class="flex" :class="{'flex-row-reverse':props.inverso}">
        <div>
            <slot name="imagen"></slot>
        </div>
        <div>
            <h3>
                <slot name="header">
                </slot>
            </h3>
            <p>
                <slot></slot>
            </p>
            <slot name="footer">
            </slot>
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