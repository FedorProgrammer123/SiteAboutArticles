<script setup>
</script>
<template>
    <div v-for="(el,key) in articles" v-bind:key="key" class="card" style="width: 18rem;">
        <img v-bind:src="el.picture" class="card-img-top" alt="...">
        <div class="card-body">
          <h5 class="card-title">{{ el.title }}</h5>
          <p class="card-text">{{ el.description }}</p>
          <a href="#" class="btn btn-primary">{{ el.read }}</a>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
            articles:[
                {
                    picture: 'https://itproger.com/img/news/1534765244.jpg',
                    title: 'Сравнение движков: Unreal Engine 4 против Unity 5',
                    description: 'Выбрать игровой движок дело не простое, а особо когда оба хороши. В статье мы проведём сравнение двух программ и выясним какой движок использовать именно Вам!',
                    read: 'Читать далее'
                },
                {
                    picture: 'https://itproger.com/img/news/1534137690.jpg',
                    title: '7 девушек айтишниц из фильмов и сериалов',
                    description: 'Много ли вы знаете фильмов и сериалов, где главные персонажи это девушки программисты? Мы подобрали 7 фильмов с такой категорией.',
                    read: 'Читать далее'
                },
                {
                    picture: 'https://itproger.com/img/news/1532948245.jpg',
                    title: '11 инструментов для веб разработчика',
                    description: 'Разработчики постоянно пытаются сделать свою жизнь проще или расширить собственные возможности. Мы подготовили 11 инструментов, которые это обеспечат.',
                    read: 'Читать далее'
                },
                {
                    picture: 'https://itproger.com/img/news/1534139040.jpg',
                    title: 'Что такое Deep Learning? Как работает глобальное обучение?',
                    description: 'Как работает глобальное обучение и что оно из себя представляет? В ходе статьи мы расскажет про Deep Learning и разберемся с его ключевыми понятиями.',
                    read: 'Читать далее'
                }
            ]
        }
    }
}
</script>
<style scoped>
.card:nth-child(3){
    position: relative;
    margin-left: 20em;
    margin-top: 5em;
}
.card:nth-child(4){
    position: relative;
    margin-left: 40em;
    margin-top: -25em;
}
.card:nth-child(5){
    margin-left: 20em;
    margin-top: 5em;
}
.card:nth-child(6){
    margin-left: 40em;
    margin-top: -24em;
}
.btn{
    background-color: #FFB908;
    border: 0;
    color: #000000;
    font-weight: bolder;
}
</style>