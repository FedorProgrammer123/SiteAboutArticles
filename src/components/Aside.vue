<script setup>
</script>
<template>
        <p class="fs-3 Anonces">Анонсы</p>
        <div v-for="(el,key) in asides" v-bind:key="key" class="card" style="width: 18rem;">
            <img v-bind:src="el.picture" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">{{ el.title }}</h5>
              <p class="card-text">{{ el.text }}</p>
              <a href="#" class="btn btn-primary">{{ el.readmore }}</a>
            </div>
        </div>
</template>
<script>
export default {
    data(){
        return{
            asides:[
                {
                    picture: 'https://i.ytimg.com/vi/5F3xY0zgvOA/hqdefault_live.jpg',
                    title: 'Android',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ultrices elit quis augue condimentum rhoncus. Praesent ac pharetra felis. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Maecenas at sagittis lectus. Nunc id egestas nulla, vel sagittis velit. Aenean imperdiet lorem vel justo rhoncus, nec mattis libero volutpat. Aliquam tempor, est eget pulvinar rhoncus, metus orci facilisis erat, a porttitor arcu dui eget nisl. Mauris nec iaculis nulla. Aliquam mollis arcu ullamcorper interdum varius. Nullam ac ex ut libero tincidunt laoreet ut et mauris. Curabitur consequat enim quis nisl blandit, sed lacinia odio cursus. Suspendisse iaculis ipsum et egestas imperdiet. Nam eget lacus condimentum, malesuada ligula vel, consequat risus.',
                    readmore: 'Читать далее'
                },
                {
                    picture: 'https://i.ytimg.com/vi/5F3xY0zgvOA/hqdefault_live.jpg',
                    title: 'IOS',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ultrices elit quis augue condimentum rhoncus. Praesent ac pharetra felis. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Maecenas at sagittis lectus. Nunc id egestas nulla, vel sagittis velit. Aenean imperdiet lorem vel justo rhoncus, nec mattis libero volutpat. Aliquam tempor, est eget pulvinar rhoncus, metus orci facilisis erat, a porttitor arcu dui eget nisl. Mauris nec iaculis nulla. Aliquam mollis arcu ullamcorper interdum varius. Nullam ac ex ut libero tincidunt laoreet ut et mauris. Curabitur consequat enim quis nisl blandit, sed lacinia odio cursus. Suspendisse iaculis ipsum et egestas imperdiet. Nam eget lacus condimentum, malesuada ligula vel, consequat risus.',
                    readmore: 'Читать далее'
                }
            ]
        }
    }
}
</script>
<style scoped>
.Anonces{
    margin-left: 45em;
    margin-top: -32em;
}
.card{
    margin-left: 78em;
}
</style>