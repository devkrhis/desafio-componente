<template>
    <div id="caixa">
        <div id="teste">
            <h1 v-if="oneValue == 0"> Usuário não Selecionado </h1>
            <strong v-else>
                <ul>
                    <li> {{ generalData.oneValue }}</li>
                    <li> {{ generalData.name }}</li>
                    <li> {{ generalData.idade }}</li>
                </ul>
            </strong>
        </div>

    </div>
    
</template>

<script>
 /* eslint-disable */
export default {
    props: {
        generalData: {
            type: Object,
        },
    }
}
</script>

<style scoped>

</style>