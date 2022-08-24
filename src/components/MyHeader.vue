<template>
    <header>
        <div class="logo">
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </div>

        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a href="link.url" :class="link.active?'active':'' ">{{link.text}}</a>
                </li>
            </ul>
        </nav>


    </header>
</template>

<script>

export default {
    name: "MyHeader",
    data(){
        return{
            links:[
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    text: 'VIDEO',
                    url: '#',
                    active: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: false
                },
            ]
        }
    }
}


</script>

<style lang="scss">

    @import '../Style/var.scss';
    @import '../Style/MyHeader.scss';
    @import '../Style/reset.scss';

    
</style>