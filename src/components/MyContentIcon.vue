<template>

<div class="section">
    <div class="icon-container">
        <ul>
            <li v-for="(icon, index) in icons" :key="index">
                <img :src="icon.url" alt="icon">
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
                    url: '../assets/img/buy-comics-digital-comics.png',
                    text: "DIGITAL COMICS"
                },
                {   
                    url: "../assets/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {   
                    url: "../assets/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION"
                },
                {
                    url: "../assets/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"
                },
                {
                    url: "../assets/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>

<style lang="scss">

    .section{
        background-color: #0E7CEB;
        height: 100px;
        .icon-container{
            max-width: 1400px;
            margin: 0 auto;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            ul{
                display: flex;
                list-style-type: none;
                li{
                    padding: 20px;
                    span{
                        margin: 10px;
                    }
                }
            }
        }
    }

</style>