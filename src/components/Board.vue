<template>

    <div class="board">

        <div class="display">
            <div class="display-col1"></div>
            <div class="display-col2">
                <div class="display-col2-row">
                    <div class="box" v-html="letter"></div>
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
                    <div class="keys" @click="display($event)">Q</div>
                    <div class="keys" @click="display($event)">W</div>
                    <div class="keys" @click="display($event)">E</div>
                    <div class="keys" @click="display($event)">R</div>
                    <div class="keys" @click="display($event)">T</div>
                    <div class="keys" @click="display($event)">Y</div>
                    <div class="keys" @click="display($event)">U</div>
                    <div class="keys" @click="display($event)">I</div>
                    <div class="keys" @click="display($event)">O</div>
                    <div class="keys" @click="display($event)">P</div>
                </div>
                <div class="keyboard-row2">
                    <div></div>
                    <div class="keys" @click="display($event)">A</div>
                    <div class="keys" @click="display($event)">S</div>
                    <div class="keys" @click="display($event)">D</div>
                    <div class="keys" @click="display($event)">F</div>
                    <div class="keys" @click="display($event)">G</div>
                    <div class="keys" @click="display($event)">H</div>
                    <div class="keys" @click="display($event)">J</div>
                    <div class="keys" @click="display($event)">K</div>
                    <div class="keys" @click="display($event)">L</div>
                </div>
                <div class="keyboard-row3">
                    <div class="key" @click="check()">Enter</div>
                    <div class="keys" @click="display($event)">Z</div>
                    <div class="keys" @click="display($event)">X</div>
                    <div class="keys" @click="display($event)">C</div>
                    <div class="keys" @click="display($event)">V</div>
                    <div class="keys" @click="display($event)">B</div>
                    <div class="keys" @click="display($event)">N</div>
                    <div class="keys" @click="display($event)">M</div>
                    <div class="key" @click="clear()"><i class="fa fa-delete-left"></i></div>
                </div>
                
            </div>
            <div></div>
        </div>

    </div>
        
</template>

<script>

import { ref } from 'vue'

let letter=ref("");

export default  {
    name: "Board",
    components: {question
    },
    methods:{
        display(event){question
            letter.value = event.target.innerHTML
        }
    },
    // data:{}
}
</script>

<style lang="scss" scoped>


.keys:hover{
    cursor: pointer;
}
.keyboard{
    display: grid;
    grid-template-columns: 34% 30% 35%;
    margin-top: 3%;
    width: 100%;
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
}
.keyboard-row3{
    display: grid;
    grid-template-columns: 15% 10% 10% 10% 10% 10% 10% 10% 15%;
    column-gap: 1%;
    font-size: 1.25em;
}
.keyboard-row2{
    display: grid;
    grid-template-columns: 5% 10% 10% 10% 10% 10% 10% 10% 10% 10% 5%;
    column-gap: 1%;
    font-size: 1.25em;
    width: 100%;
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


@media only screen and (max-width: 600px) {
    .keyboard{
        display: grid;
        grid-template-columns: 0% 90% 0%;
        margin-top: 4%;
        width: 100%;
    }

    .display{
        display: grid;
        grid-template-columns: 25% 50% 25%;
        margin-top: -4%;
        color: gray
    }

    .box{
        border: solid 2px rgb(211, 211, 211);
        padding: 50%;
    }
}

@media only screen and (max-width: 1230px) {
    .keyboard{
        display: grid;
        grid-template-columns: 30% 40% 30%;
        margin-top: 4%;
        width: 100%;
    }

    .display{
        display: grid;
        grid-template-columns: 40% 20% 40%;
        margin-top: -4%;
    }

    .box{
        border: solid 2px rgb(211, 211, 211);
        padding: 50%;
    }
}

</style>
