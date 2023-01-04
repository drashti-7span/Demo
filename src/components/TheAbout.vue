<template>
    <div>
        <h1>About component</h1>
        <TheUsers />
    </div>
</template>

<script>
import TheUsers from './TheUsers.vue'
export default {
    name: 'TheAbout',
    components:{
        TheUsers
    }
}
</script>