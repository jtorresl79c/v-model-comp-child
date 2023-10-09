<template>
    <div>
        <input 
            type="text"
            :value="modelValue"
            @input="$emit('update:modelValue', $event.target.value)"
            class="form-control"
            :placeholder="placeholder"
        >
    </div>
</template>

<script>
    export default {
        props: {
            modelValue: {
                type: String,
                required: true
            },
            placeholder: String,
        },
    }
</script>

<style lang="scss" scoped>

</style>