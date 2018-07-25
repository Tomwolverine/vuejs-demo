<template>
    <div class="drimg">
        <h2>I'M {{dragon.name}}</h2>
        <h3>My ID is {{dragon.id}}</h3>
        <img class="dragpic" :src='dragon.imageUrl'>
    </div>
    
</template>

<script>
export default {
    name: "Card",
    props: ['dragon']
}
</script>

<style>
.drimg {
    border: 2px;
    border-color: red;
    background-color: aqua;
}
.dragpic {
    height: 200px;
    width: 200px;
}
</style>
