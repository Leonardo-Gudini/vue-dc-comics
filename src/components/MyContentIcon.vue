<template>

<div class="section">
    <div class="icon-container">
        <ul>
            <li v-for="(icon, index) in icons" :key="index">
                <img :src="require('../assets/img/' + icon.url)" alt="icon">
                <span>{{icon.text}}</span>
            </li>
        </ul>
    </div>
</div>
  
</template>

<script>
export default {
    name: "MyContentIcon",

    data(){
        return{
            icons:[
                {
                    url: 'buy-comics-digital-comics.png',
                    text: "DIGITAL COMICS"
                },
                {   
                    url: "buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {   
                    url: "buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION"
                },
                {
                    url: "buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"
                },
                {
                    url: "buy-dc-power-visa.svg",
                    text: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>

<style lang="scss">

    @import "@/Style/var.scss";
    @import "@/Style/MyContentIcon.scss"

</style>