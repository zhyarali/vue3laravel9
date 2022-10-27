<template>
    <div>
        <button @click="add_counter">counter by one</button>
        <p>{{counter}}</p>
    </div>
</template>

<script>
import {ref} from 'vue';
export default {
    setup () {

        const counter=ref(0);

        function add_counter() {
            counter.value+=1;
        }

        return {counter,add_counter}
    }
}
</script>

<style lang="scss" scoped>

</style>
