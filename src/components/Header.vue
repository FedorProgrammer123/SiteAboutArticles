<script setup>
import LogoVue from '../assets/logo-waveform-svgrepo-com.svg'
</script>
<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
          <a class="navbar-brand" href="#"><img v-bind:src="LogoVue"></a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">ItProger<br/>Blog</a>
              </li>
            </ul>
            <form class="d-flex" role="search">
              <input class="form-control me-2" type="search" placeholder="Поиск">
              <button v-on:mouseleave="changeColor()" v-bind:style="color" class="btn btn-outline-success" type="submit">{{ home }}</button>
              <button v-on:mouseleave="changeColorArticles()" v-bind:style="colorArticles" class="btn btn-outline-success" type="submit">{{ articles }}</button>
              <button v-on:mouseleave="changeColorContacts()" v-bind:style="colorContacts" class="btn btn-outline-success" type="submit">{{ contacts }}</button>
            </form>
          </div>
        </div>
      </nav>
</template>
<script>
export default {
    data(){
        return{
            color: '',
            colorArticles: '',
            colorContacts: '',
            home: 'Главная',
            articles: 'Статья',
            contacts: 'Контакты'
        }
    },
    methods:{
      changeColor(){
        this.color = 'color:red'
      },
      changeColorArticles(){
        this.colorArticles = 'color:blue'
      },
      changeColorContacts(){
        this.colorContacts = 'color:#34eb64'
      }
    },
    components:{
      LogoVue
    }
}
</script>
<style scoped>
img{
    width: 2em;
}
img:hover{
  transform: rotate(360deg);
  transition: all 5s ease-in-out;
}
nav{
    width: 80em;
    background-color: #FFFFFF;
    margin-left: 20em;
    margin-top: 2em;
}
.form-control{
    margin-right: 25px;
}
</style>