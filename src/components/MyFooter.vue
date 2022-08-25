<template>
    <footer>
        <div class="container">
            <div class="ul-container">
                <ul>
                <h3 class="list-title">DC COMICS</h3>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>

            <ul>
                <h3 class="list-title">SHOP</h3>
                <li v-for="(shop, index) in shops" :key="index">
                    <a :href="shop.url">{{shop.text}}</a>
                </li>
            </ul>

            <ul>
                <h3 class="list-title">DC</h3>
                <li v-for="(dc, index) in dcs" :key="index">
                    <a :href="dc.url">{{dc.text}}</a>
                </li>
            </ul>

            <ul>
                <h3 class="list-title">SITES</h3>
                <li v-for="(site, index) in sites" :key="index">
                    <a :href="site.url">{{site.text}}</a>
                </li>
            </ul>
            </div>

            <img src="../assets/img/dc-logo-bg.png" alt="logo">
        </div>

        

        <div class="footer-bottom">
            <div class="bottom-container">
                <button>SIGN-UP NOW!</button>
                <div class="socials">
                    
                    <h3>FOLLOW US</h3>
                    
                    <ul>
                        <li>
                            <img v-for="(icons, index) in socials" :key="index" :src='icons.icon' alt="social">
                        </li>
                    </ul>
                </div>
            </div>
            
        </div>
    </footer>
</template>

<script>
export default {
    name: "MyFooter",

    data(){
        return{
            links:[
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'TV',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                },
                {
                    text: 'FANS',
                    url: '#',
                },
                {
                    text: 'NEWS',
                    url: '#',
                },
                {
                    text: 'SHOP',
                    url: '#',
                },
            ],
            shops:[
                {
                    text: 'shop DC',
                    url: '#',
                },
                {
                    text: 'shop DC Collectibles',
                    url: '#',
                },
            ],
            dcs:[
                {
                    text: 'Terms Of Use',
                    url: '#',
                },
                {
                    text: 'Privacy Polici(New)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                },
                {
                    text: 'Talent Workshops',
                    url: '#',
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Heelp',
                    url: '#',
                },
                {
                    text: 'Contact Us',
                    url: '#',
                },
            ],
            sites:[
                {
                    text: 'DC',
                    url: '#',
                },
                {
                    text: 'MAD Magazine',
                    url: '#',
                },
                {
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                },
            ],
            socials:[
                {
                    icon: '../assets/img/footer-facebook.png'
                },
                {
                    icon: '../assets/img/footer-facebook.png'
                },
                {
                    icon: '../assets/img/footer-facebook.png'
                },
                {
                    icon: '../assets/img/footer-facebook.png'
                },
                {
                    icon: '../assets/img/footer-facebook.png'
                }
            ]
            
        }
    }
}


</script>

<style lang="scss">

@import '../Style/MyFooter.scss';

</style>