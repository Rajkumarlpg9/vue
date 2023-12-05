<template>
   
    
    <div v-for="tool of tools" :key="tool.id" >

     
       <SingleBook :tool=tool />

    </div>

</template>
<script>
import SingleBook from './SingleBook.vue'

export default {
    name: 'BookBox',
    props:{
        tools: Array
    },
    components:{
        SingleBook
    }
    
}
</script>
<style scoped>

</style>
