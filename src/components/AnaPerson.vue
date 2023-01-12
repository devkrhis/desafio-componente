<template>
    <div id="AnaPerson">
        <h1> Usuário não Selecionado </h1>
        <div>
            <li> <button type="button" @click="primaryKey"> 1 Ana</button> </li>
            <li> <button type="button" @click="secondKey"> 2 Carlos</button> </li>
            <li> <button type="button" @click="thirdKey"> 3 Daniel</button> </li>
            <li> <button type="button" @click="bedroomKey"> 4 Ema</button> </li>
            <li> <button type="button" @click="fifthKey"> 5 Lia</button> </li>
        </div>
    </div>
    
</template>

<script>
/* eslint-disable */
export default {
    props: ['idade'],
    data(){
        return {
            oneValue: 1,
            name: 'Ana',
            idade: 31,
        }
    },
    methods: {
        primaryKey(){
            this.oneValue = 1,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Ana',
            this.$emit('sameName', this.name)
            this.idade = 31
            this.$emit('sameAge', this.idade)
        },
        secondKey(){
            this.oneValue = 2,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Carlos',
            this.$emit('sameName', this.name)
            this.idade = 31
            this.$emit('sameAge', this.idade)
        },
        thirdKey(){
            this.oneValue = 3,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Daniel',
            this.$emit('sameName', this.name)
            this.idade = 31
            this.$emit('sameAge', this.idade)
        },  
        bedroomKey(){
            this.oneValue = 4,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Ema',
            this.$emit('sameName', this.name)
            this.idade = 31
            this.$emit('sameAge', this.idade)
        },
        fifthKey(){
            this.oneValue = 5,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Lia',
            this.$emit('sameName', this.name)
            this.idade = 31
            this.$emit('sameAge', this.idade)
        }
    }
}
</script>

<style scoped>
#AnaPerson li:hover {
    background-color: rgba(204, 190, 190, 0.815);
}

</style>