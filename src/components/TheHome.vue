<template>
    <div>
        <h1 v-if="show">Hello from Home Components</h1>
        <button v-on:click="display">Toggle Element</button>
        <h2>{{date}}</h2> 
        <h2>{{msg}}</h2> 
        <button v-on:click="hello('hello call')">Call Hello Function on click</button> 
        <button v-on:mouseover="hello('hello call')">Call Hello Function mousehover</button> 
        <table border="1px">
            <tr>
                <td>ID</td>
                <td>Name</td>
                <td>Email</td>
            </tr>
            <tr v-for="item in items" :key="item.id">
                <td>{{item.id}}</td>
                <td>{{item.name}}</td>
                <td>{{item.email}}</td>
            </tr>
        </table>
    </div>
    
</template>
<script>
export default {
    name: "TheHome",
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
        return {show:true,
            items:[
            {id:1,name:'peter',email:'peter@test.com'},
            {id:2,name:'bruce',email:'bruce@test.com'},
            {id:3,name:'tony',email:'tony@test.com'},
            {id:4,name:'sam',email:'sam@test.com'},
        ]
        }
        
    }
};
</script>