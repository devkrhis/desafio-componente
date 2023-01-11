<template>
    <div id="AnaPerson">
        <li>{{ oneValue }} {{ name }}</li>
    </div>
    
</template>

<script>

export default {
    data(){
        return {
            oneValue: 1,
            name: 'Ana',
            idade: 31
        }
    }
    
}
</script>

<style scoped>
#AnaPerson li:hover {
    background-color: rgba(204, 190, 190, 0.815);
}

</style>