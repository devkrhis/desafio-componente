<template>
    <div id="AnaPerson">
        <li> <button type="button" @click="primaryKey"> {{ idade }} </button> </li>
    </div>
    
</template>

<script>
/* eslint-disable */
export default {
    props: ['idade','oneValue','name'],
    data(){
        return {
           // oneValue: 1,
           // name: 'Ana',
            idade: 31
        }
    },
    methods: {
        primaryKey(){
            //this.oneValue = 1,
            //this.$emit('sameNumber', this.oneValue)
            //this.name = 'Ana',
            //this.$emit('sameName', this.name)
            this.idade = 31
            // this.$emit('sameAge', this.idade)
        }
    }
}
</script>

<style scoped>
#AnaPerson li:hover {
    background-color: rgba(204, 190, 190, 0.815);
}

</style>