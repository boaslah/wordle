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

<style lang="scss" scoped>
h1{
    text-align: center;
    font-family: "Patua One"
}

.header{
    display: grid;
    grid-template-columns: 33% 33% 33%;
    border-bottom: solid 1px rgb(211, 211, 211);
    margin: -1% 0% 5% -1%;
    max-height: 70px;
}

</style>
