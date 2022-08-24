<template>
    <footer>
        <ul>
            <h3 class="list-title">DC COMICS</h3>
            <li v-for="(link, index) in links" :key="index">
                <a href="link.url" :class="link.active?'active':'' ">{{link.text}}</a>
            </li>
        </ul>

        <ul>
            <h3 class="list-title">SHOP</h3>
            <li v-for="(shop, index) in shops" :key="index">
                <a href="shop.url">{{shop.text}}</a>
            </li>
        </ul>

        <ul>
            <h3 class="list-title">DC</h3>
            <li v-for="(dc, index) in dcs" :key="index">
                <a href="dc.url">{{dc.text}}</a>
            </li>
        </ul>

        <ul>
            <h3 class="list-title">SITES</h3>
            <li v-for="(site, index) in sites" :key="index">
                <a href="site.url">{{site.text}}</a>
            </li>
        </ul>
    </footer>
</template>

<script>
export default {
    name: "MyFooter",

    data(){
        return{
            links:[
                {
                    text: 'CHARACTERS',
                    url: '#',
                },
                {
                    text: 'COMICS',
                    url: '#',
                },
                {
                    text: 'MOVIES',
                    url: '#',
                },
                {
                    text: 'TV',
                    url: '#',
                },
                {
                    text: 'GAMES',
                    url: '#',
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                },
                {
                    text: 'VIDEO',
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
            
        }
    }
}


</script>

<style>

</style>