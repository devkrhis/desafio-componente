<template>
    <div id="caixa">
        <div id="teste">
            <h1 v-if="oneValue == 0"> Usuário não Selecionado </h1>
            <strong v-else>
                <ul>
                    <li> {{ oneValue }}</li>
                    <li> {{ name }}</li>
                    <li> {{ idade }}</li>
                </ul>
            </strong>
        </div>

    </div>
    
</template>

<script>
 /* eslint-disable */
export default {
    props: {
        oneValue: {
            type: Number,
        },
        name: {
            type: String,
        },
        idade: {
            type: Number
        }
    }
}
</script>

<style scoped>

</style>