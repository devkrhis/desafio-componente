<template>
    <div id="caixa">
        <ul>
            <li> {{ oneValue }}</li>
            <li> {{ name }}</li>
            <li> {{ idade }}</li>
        </ul>

    </div>
    
</template>

<script>
export default {
    props: ['oneValue', 'name', 'idade']
}
</script>

<style scoped>

</style>