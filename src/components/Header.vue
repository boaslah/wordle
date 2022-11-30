<template>

    <div class="header">

        <div></div>

        <div>

            <h1>Wordle</h1>
        
        </div>

        <div></div>

    </div>
        
</template>

<script>


export default  {
    name: "Header"
}
</script>

<style scoped>
h1{
    text-align: center;
}

.header{
    display: grid;
    grid-template-columns: 33% 33% 33%;
    border-bottom: solid 2px rgb(155, 153, 153);
    margin: -1% 0% 0% -1%;
}

</style>
