<template>
    <header>
        <div class="logo">
            <img src="@/assets/img/dc-logo.png" alt="logo">
        </div>

        <nav>
            <ul>
                <li v-for="(nav, index) in navbars" :key="index">
                    <a :href="nav.url" :class="nav.active?'active':''">{{nav.txt}}prova</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>

export default {
    name: "MyHeader",
    Data(){
        return{
            navbar: [
            {
                txt: "CHARACTERS",
                url: "#",
                active: "false"
            },
            {
                txt: "COMICS",
                url: "#",
                active: "false"
            },
            {
                txt: "MOVIES",
                url: "#",
                active: "false"
            },
            {
                txt: "TV",
                url: "#",
                active: "false"
            },
            {
                txt: "GAMES",
                url: "#",
                active: "false"
            },
            {
                txt: "COLLECTIBLES",
                url: "#",
                active: "false"
            },
            {
                txt: "VIDEOS",
                url: "#",
                active: "false"
            },
            {
                txt: "FANS",
                url: "#",
                active: "false"
            },
            {
                txt: "NEWS",
                url: "#",
                active: "false"
            },
            {
                txt: "SHOP",
                url: "#",
                active: "false"
            },
        ]
        }
        
    }
}


</script>

<style>

</style>