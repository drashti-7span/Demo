<template>
    <div>
        <h1>DataBind component</h1>
        <h2 style="white-space:pre-line">{{ message }}</h2>
        <!-- <input type="text" v-model="message"> -->
        <textarea type="text" v-model="message"> </textarea>
    </div>
</template>

<script>
export default {
    name:'DataBind',
    data(){
        return{
            message:"Hi"
        }
    }
}
</script> 