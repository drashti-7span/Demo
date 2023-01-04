<template>
    <div>
        <h1>Child component</h1>
        <h3>{{name}}</h3>
    </div>
</template>
<script>
export default {
    name:'TheChild',
    props:'[name]'
}
</script>