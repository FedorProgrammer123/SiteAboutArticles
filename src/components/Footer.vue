<template>
    <footer>
        <p>{{ AllRights }} &copy;</p>
    </footer>
</template>
<script>
export default {
    data(){
        return{
            AllRights: 'Все права защищены'
        }
    }
}
</script>
<style scoped>
footer{
    width: 76em;
    height: 20em;
    border: 5px solid silver;
    background-color: #ffffff;
    margin-left: 20em;
    border-radius: 5%;
}
p{
    color: rgb(60, 255, 0);
    font-size: 2em;
    text-align: center;
    margin-top: 2em;
}
</style>