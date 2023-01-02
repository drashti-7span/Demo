<template>
    <div>
        <h1 v-if="show">Hello from Home Components</h1>
        <!-- <h1 v-else>Hello from Home Components</h1 >  -->
        <button v-on:click="display">Toggle Element</button>
        <h2>{{date}}</h2> 
        <h2>{{msg}}</h2> 
        <button v-on:click="hello('hello call')">Call Hello Function on click</button> 
        <button v-on:mouseover="hello('hello call')">Call Hello Function mousehover</button> 
    </div>
    
</template>
<script>
export default {
    name: "Home-tut",
    props:{
        date:String,
        msg:String
    },
    methods:{
        hello(date){
            alert(date)
        },
        display()
        {
            this.show=!this.show
        }
    },
    data()
    {
        return {show:true}
    }
};
</script>