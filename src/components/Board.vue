<template>

    <div class="board">

        <div class="display">
            <div class="display-col1"></div>
            <div class="display-col2">
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                <div class="display-col2-row">
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                    <div class="box"></div>
                </div>
                
            </div>
            <div class="display-col3"></div>
        </div>

        <div class="keyboard">
            <div></div>
            <div class="keyboard-col2" >
                <div class="keyboard-row">
                    <div class="keys">Q</div>
                    <div class="keys">W</div>
                    <div class="keys">E</div>
                    <div class="keys">R</div>
                    <div class="keys">T</div>
                    <div class="keys">Y</div>
                    <div class="keys">U</div>
                    <div class="keys">I</div>
                    <div class="keys">O</div>
                    <div class="keys">P</div>
                </div>
                <div class="keyboard-row2">
                    <div></div>
                    <div class="keys">A</div>
                    <div class="keys">S</div>
                    <div class="keys">D</div>
                    <div class="keys">F</div>
                    <div class="keys">G</div>
                    <div class="keys">H</div>
                    <div class="keys">J</div>
                    <div class="keys">K</div>
                    <div class="keys">L</div>
                </div>
                <div class="keyboard-row3">
                    <div class="key">Enter</div>
                    <div class="keys">Z</div>
                    <div class="keys">X</div>
                    <div class="keys">C</div>
                    <div class="keys">V</div>
                    <div class="keys">B</div>
                    <div class="keys">N</div>
                    <div class="keys">M</div>
                    <div class="key"><i class="fa fa-delete-left"></i></div>
                </div>
                
            </div>
            <div></div>
        </div>

    </div>
        
</template>

<script>


export default  {
    name: "Board"
}
</script>

<style scoped>


.keys:hover{
    cursor: pointer;
}
.keyboard{
    display: grid;
    grid-template-columns: 34% 30% 39%;
    margin-top: 3%;
}
.keyboard-col2{
    display: grid;
    grid-template-rows:33% 33% 33%;
    row-gap: 5%;
}

.keyboard-row{
    display: grid;
    grid-template-columns: 10% 10% 10% 10% 10% 10% 10% 10% 10% 10%;
    column-gap: 1%;
    font-size: 1.25em;
    font-weight: bold;
}
.keyboard-row3{
    display: grid;
    grid-template-columns: 15% 10% 10% 10% 10% 10% 10% 10% 15%;
    column-gap: 1%;
    font-size: 1.25em;
    font-weight: bold;
}
.keyboard-row2{
    display: grid;
    grid-template-columns: 5% 10% 10% 10% 10% 10% 10% 10% 10% 10% 5%;
    column-gap: 1%;
    font-size: 1.25em;
    font-weight: bold;
}

.display-col2-row{
    display: grid;
    grid-template-columns: 20% 20% 20% 20% 20%;
    column-gap: 5%;
}
.display-col2{
    display: grid;
    grid-template-rows: 16% 16% 16% 16% 16% 16%;
    row-gap: 3%;
}
.board{
    display: grid;
    width: 100%;
    font-family: "Patua One"
}
.keys{
    padding: 35%;
    background-color: #d3d6da;
    font-family: "Patua One";
    color: black;
    border-radius: 7%;
    text-align: center;
}
.key{
    /* padding: 15%; */
    background-color: #d3d6da;
    font-family: "Patua One";
    color: black;
    border-radius: 7%;
    text-align: center;
    padding-top: 25%;
}

.display{
    display: grid;
    grid-template-columns: 41% 15% 44%;
    margin-top: -4.3%;
}

.box{
    border: solid 2px rgb(211, 211, 211);
    padding: 52%;
}

</style>
