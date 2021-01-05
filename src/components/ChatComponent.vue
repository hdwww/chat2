<template>
    <div class="chat">
        <h1>여기는 채팅이 보이는 곳 입니다.</h1>
        <div class="input">
            <input type="text" value="text 입력">
            <button>Input</button>
        </div>
        <input-component></input-component>
    </div>
</template>

<script>

import InputComponent from './InputComponent';

    export default{
        name:'ChatComponent', 
        components:{
            'input-component' : InputComponent
        }
    }
</script>

<style scoped>
    .chat{
        display: grid;
        grid-template-rows: 1fr 80px;
    }
    .input{
        display: table;
        margin: 0px auto;
    }
    input{
        width: 500px;
        height: 35px;
        border-color: black;
        border-radius: 10px;
    }
    button{
        width: 50px;
        height: 40px;
        margin-left: 20px;
        border-radius: 10px;
        border-color: black;
        background-color: white;
    }
</style>>
