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
                <div class="keyboard-row">
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
                <div class="keyboard-row">
                    <div class="keys enter">Enter</div>
                    <div class="keys">Z</div>
                    <div class="keys">X</div>
                    <div class="keys">C</div>
                    <div class="keys">V</div>
                    <div class="keys">B</div>
                    <div class="keys">N</div>
                    <div class="keys">M</div>
                    <div class="keys">X</div>
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

.enter{
    /* padding: 35% 50% 35% 50% !important; */
    text-align: center !important;
}

.keyboard{
    display: grid;
    grid-template-columns: 33% 33% 33%;
    margin-top: 4%;
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

.display-col2-row{
    display: grid;
    grid-template-columns: 20% 20% 20% 20% 20%;
    column-gap: 6%;
}
.display-col2{
    display: grid;
    grid-template-rows: 16% 16% 16% 16% 16% 16%;
    row-gap: 4%;
}
.board{
    display: grid;
    width: 100%;
    font-family: "Patua One"
}
.keys{
    padding: 35% 10% 35% 10%;
    background-color: #d3d6da;
    font-family: "Patua One";
    color: black;
    border-radius: 7%;
    text-align: center;
}

.display{
    display: grid;
    grid-template-columns: 41% 15% 44%;
    margin-top: -4.3%;
}

.box{
    border: solid 2px rgb(211, 211, 211);
    padding: 50%;
}

</style>
