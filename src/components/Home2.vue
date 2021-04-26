<template>
    <div>
        <h1 id="demo">{{name}}</h1>
    </div>
</template>

<script>
export default {
    name:'Home2',
    data(){
        return {
            name:"AK2",
        }
    },

    beforeMount()
    {
        //console.warn(this.$el)//$el represent html 
        //console.warn("before mount",document.getElementById("demo"))//null value not html rendered
        console.warn("before mount")//before html rendering called null will be outputed because html not called
    },

    mounted()
    {   
        //console.warn(this.$el)     
        console.warn("mounted",document.getElementById("demo"))//html rendered then only called for html DOM so id is given
                                                                //DOM can only be modified in 
    }

}
</script>