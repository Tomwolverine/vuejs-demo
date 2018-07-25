<template>
    <div>
        <Card v-for="dragon in dragons" :key='dragon.id' :dragon="dragon"/>
    </div>
</template>

<script>
import Card from './Card'
export default {
    name: "CardList",
    components: { 
        Card
        },
data(){
    return {
        dragons: [  {name: "Tiamat", id: 1, imageUrl:'https://www.sciencenewsforstudents.org/sites/default/files/scald-image/860-dragon-header-iStock-494839519.gif'},
                    {name: "Smaug", id: 2, imageUrl:'https://vignette.wikia.nocookie.net/reddits-world/images/9/9a/RedDragon.jpg/revision/latest?cb=20140914212250'},
                    {name: "Puff", id:3, imageUrl:'https://www.sciencenewsforstudents.org/sites/default/files/scald-image/860-dragon-header-iStock-494839519.gif'},
                    {name: "Piro", id: 4, imageUrl:'https://i.ytimg.com/vi/P3SgpYXxqfs/maxresdefault.jpg'}
                ]
        }
    }
}
</script>

<style>

</style>
