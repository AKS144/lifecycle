<template>
    <div>
        <h1>{{name}}</h1>
    </div>
</template>

<script>
export default {
    name:'Home',
    data()
    {
        return {
            name:"AK",            
        }
    },

    created()
    {
        this.name="sam"
        console.warn("created",this.name)//everything will be updated inside created
    },
    
    beforeCreate()
    {

        console.warn("before")//created before component is created and
                             //no changes will be initialised in this in component
    }
}
</script>