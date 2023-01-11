<template>
    <div id="homePage">
        <AnaPerson/>
        <div id="controlBox">
            <h1> Teste: {{ idade }}</h1>
            <informationBlock
            :idade="idade"
            @sameAge="idade = $event"/>
        </div>
    </div>
    
</template>

<script>
/* eslint-disable */
import AnaPerson from './AnaPerson.vue';
import informationBlock from './InformationBlock.vue'
export default {
    components: {
        AnaPerson,
        informationBlock
    },
    data(){
        return {
            idade: 0
        }
    }
    
}
</script>

<style scoped>

</style>