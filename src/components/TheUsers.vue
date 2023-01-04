<template>
    <div>
        <h1 class="homestyle">Class and Style bindings</h1>
        <h1 v-bind:style="{color:colorkey}">Style bindings</h1>
        <h1 v-bind:class="{dispay:show}">class bindings with object</h1>
        <h1 v-bind:class="[aclass]">class bindings with array</h1>
        <h1 v-bind:class="[show?'yesSHow':'noSHow']">class Show</h1>
    </div>
</template>

<script>
export default {
    name: 'TheUsers',
    data(){
        return{
            show:true,
            aclass:'arrayclass',
            colorkey:'green'
        }
    }
}
</script>

<style scoped>
.homestyle{
    color: orange
}
.dispay{
    background-color: brown;
}
.arrayclass{
    background-color: cadetblue;
}
</style>