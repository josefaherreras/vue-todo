<template>
    <div id="search-container">
        <input type="text" placeholder="Busca tarea" 
        v-model="query" v-on:input="$emit('query-change', query)">
    </div>
</template>
<script>
export default {
    name: 'Search',
    data(){
        return {
            query: ''
        }
    }
}
</script>
<style scoped>
    #search-container{
        width: 600px;
        margin: 0 auto;
    }
    input{
        padding: 10px;
        width: 100%;
        outline: none;
        border-radius: 10px;
        border: transparent;
    }
</style>