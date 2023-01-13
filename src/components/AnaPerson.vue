<template>
    <div id="AnaPerson">
        <div id="collectionButtons">
            <table>
                <tr>
                    <td> #ID </td>
                    <td> Nome </td>
                </tr>
                <tr>
                    <td> <button type="button" @click="primaryKey()"> 1 </button> </td>
                    <td> <button type="button" @click="primaryKey()"> Ana</button></td>
                </tr>
                <tr>
                    <td> <button type="button" @click="secondKey()"> 2 </button> </td>
                    <td> <button type="button" @click="secondKey()"> Carlos</button></td>
                </tr>
                <tr>
                    <td> <button type="button" @click="thirdKey()"> 3 </button> </td>
                    <td> <button type="button" @click="thirdKey()"> Daniel</button></td>
                </tr>
                <tr>
                    <td> <button type="button" @click="bedroomKey"> 4 </button> </td>
                    <td> <button type="button" @click="bedroomKey"> Ema</button></td>
                </tr>
                <tr>
                    <td> <button type="button" @click="fifthKey"> 5 </button> </td>
                    <td> <button type="button" @click="fifthKey"> Lia</button></td>
                </tr>
            </table>
        </div>
    </div>
    
</template>

<script>
/* eslint-disable */
export default {
    props: ['idade'],
    data(){
        return {
            generalData: {
                oneValue: 1,
                name: 'Ana',
                idade: 31,
            },


        }
    },
    methods: {
        primaryKey(){
            this.generalData.oneValue = 1,
            this.generalData.name = 'Ana',
            this.generalData.idade = 31
            this.$emit('sameAll', this.generalData) // passa o objeto inteiro.
        },
        secondKey(){
            this.generalData.oneValue = 2,
            this.generalData.name = 'Carlos',
            this.generalData.idade = 22
            this.$emit('sameAll', this.generalData)
        },
        thirdKey(){
            this.generalData.oneValue = 3,
            this.generalData.name = 'Daniel',
            this.generalData.idade = 40
            this.$emit('sameAll', this.generalData)
        },  
        bedroomKey(){
            this.oneValue = 4,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Ema',
            this.$emit('sameName', this.name)
            this.idade = 17
            this.$emit('sameAge', this.idade)
        },
        fifthKey(){
            this.oneValue = 5,
            this.$emit('sameNumber', this.oneValue)
            this.name = 'Lia',
            this.$emit('sameName', this.name)
            this.idade = 28
            this.$emit('sameAge', this.idade)
        }
    }
}
</script>

<style scoped>

table {
    border: 10px;
}

#AnaPerson li:hover {
    background-color: rgba(204, 190, 190, 0.815);
}

#collectionButtons {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

#collectionButtons button {
    border: none;
    background-color: white;
}

li {
    list-style-type: none;
    margin: 10px
}

</style>