<template>
    <div>
        <input 
            type="checkbox" 
            id="checkbox" 
            class="form-check-input" 
            :checked="modelValue" 
            @change="$emit('update:modelValue')"/>
    </div>
</template>

<script>
    export default {
        name: 'InputCheckbox',
        props: {
            modelValue: {
                type: Boolean,
                required: true
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>