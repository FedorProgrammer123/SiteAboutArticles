<script setup>
import cva35 from '../assets/cva35.svg'
</script>
<template>
    <div>
        <p class="display-3">3 основные сферы применения языка Python</p>
        <p class="fs-6">До начала активного изучения любого языка программирования правильно было бы задуматься о сферах его применения. Мы расскажем про 3 самые популярыне сферы применения языка Python.</p>
        <img v-bind:src="cva35" alt=""/>
        <button class="btn btn-primary">Читать далее</button>
    </div>
</template>
<style scoped>
div{
    width: 80em;
    height: 40em;
    background-color: #902929;
    margin-left: 20em;
    margin-top: 2em;
}
.display-3{
    width: 50%;
    color: #ffffff;
    padding-left: 1em;
    padding-top: 1em;
}
.fs-6{
    width: 36%;
    color: #ffffff;
    margin-left: 4em;
    margin-top: 2em;
}
img{
    margin-left: 2em;
    float: right;
    margin-top: -21.5em;
}
button{
    background-color: #CB2F3B;
    border: 0;
    margin-left: 4em;
}
</style>