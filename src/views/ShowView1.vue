<template>
    <div>
        <p>ShowView</p>

        <h1>v-model in child Examples</h1>

        <form action="" class="mt-5">

            <div class="mt-2">
                <input v-model="name" type="text" name="" id="" class="form-control" placeholder="Name">
                <p>Name: {{ name }}</p>
            </div>

            <div class="mt-5">
                <input type="checkbox" id="checkbox" class="form-check-input" v-model="newsLetter" />
                <label for="checkbox" class="form-check-label">Email me news and offers</label>
                <p>Newsletter: {{ newsLetter }}</p>
            </div>

        </form>


        <RouterView/>
    </div>
</template>
  
<script>
import { RouterLink, RouterView } from 'vue-router'
  
export default {
    provide: {
        mints: 'cloud'
    },
    data() {
        return {
            name: '',
            newsLetter: false
        }
    },

}
</script>
  
<style scoped>

</style>