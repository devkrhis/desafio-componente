<template>
    <div id="homePage">
        <hr>
        <AnaPerson 
        @sameAll="receber" 
        />
        

        <hr>
        <informationBlock 
        :idade="idade" 
        @sameAge="idade = $event"

        @sameName="name = $event"
        :name="name"

        :oneValue="oneValue"
        @sameNumber="oneValue = $event"/>
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
            generalData: {
                oneValue: 0,
                name: 'Ana',
                idade: 31,
            },
        }
    },
    methods: {
        alterarIdade(){
            this.idade = 100
        },
        receber(param){ // ele joga o general inteiro dentro do param
            console.log(param)
            param.oneValue
            param.name
            param.idade
            
        }
    }
    
}
</script>

<style scoped>

</style>