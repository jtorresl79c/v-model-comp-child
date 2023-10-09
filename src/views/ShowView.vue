<template>
    <div>
        <p>ShowView</p>

        <h1>v-model in child Examples</h1>

        <form action="" class="mt-5">
            <div class="mt-2">
                <p>Name: {{ name }}</p>
            </div>

            <div>
                <InputText placeholder="Name" v-model="name"/>
                <InputCheckbox pla />
                <label for="checkbox" class="form-check-label">Email me news and offers</label>
                <p>Newsletter: {{ newsLetter }}</p>
            </div>
        </form>


        <RouterView/>
    </div>
</template>
  
<script>
import { RouterLink, RouterView } from 'vue-router'
import InputText from '../components/InputText.vue';
import InputCheckbox from '../components/InputCheckbox.vue';
  
export default {
    provide: {
        mints: 'cloud'
    },
    data() {
        return {
            name: '',
            newsLetter: false
        };
    },
    components: { InputText, InputCheckbox }
}
</script>
  
<style scoped>

</style>