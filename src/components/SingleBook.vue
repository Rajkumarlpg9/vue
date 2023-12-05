<template>
    

    <div  :class="tool.Is_available ? 'blue': 'green' ">

                        <h1><b>Id:</b> {{tool.id}}</h1>
                        <h2><b>Name:</b> {{tool.Name}}</h2>
                        <h2><b>Release_Date:</b> {{tool.Release_Date}}</h2>
                        <h2><b>Technologies_used:</b> {{tool.Technologies_used}}</h2>
                        <h2><b>Purpose:</b> {{tool.Purpose}}</h2>
                        <h2><b>Version:</b> {{tool.Version}}</h2>
                        <h2><b>Is_available:</b> {{tool.Is_available}}</h2>
    </div>
</template>

<script>

export default{
    name: 'SingleBook',
    props:{
        tool: Array
    }
}
</script>

<style scoped>

.green{
    background-color: green;
}
.blue{
    background-color:#87CEEB;
}

h2{
    margin: 2px;
}

div{
    background-color: #ffb89e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>