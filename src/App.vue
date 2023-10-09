<template>
    <div>
        <!-- <p>Hola mundo</p>
        <RouterLink to="/about">About</RouterLink> -->
        <div class="container">
            <RouterView/>
        </div>
    </div>
</template>

<script>
    import { RouterLink, RouterView } from 'vue-router'
    export default {
        
    }
</script>

<style lang="scss" scoped>
p{
    color: red;
}
</style>