<template>
    <div id="homePage">
        <hr>
        <AnaPerson 
        :idade="idade" 
        @sameAge="idade = $event"

        @sameName="name = $event"
        :name="name"

        :oneValue="oneValue"
        @sameNumber="oneValue = $event"/>

        <div id="controlBox">
            <informationBlock 
            :idade="idade" 
            @sameAge="idade = $event"

            @sameName="name = $event"
            :name="name"

            :oneValue="oneValue"
            @sameNumber="oneValue = $event"/>
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
            oneValue: 1,
            name: 'Ana',
            idade: 31
        }
    },
    methods: {
        alterarIdade(){
            this.idade = 100
        }
    }
    
}
</script>

<style scoped>

</style>