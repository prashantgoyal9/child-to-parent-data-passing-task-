<template>
    
    <TheChild :getName="getData" />
 

    
</template>
<script>

import TheChild from './TheChild.vue';
export default {
    name:"parent",
    components:{
        TheChild
 
},
data(){
    return{
        childName:''
    }
},
methods:{
        getData(name){
            this.childName=name
        }
    }
}
</script>
<style>
    *{
        margin: 0px;
        padding: 0px;
    }

</style>