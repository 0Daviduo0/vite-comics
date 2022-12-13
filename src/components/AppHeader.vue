<script>
export default{
    name: "AppHeader",
    props: {
        logo: String,
        links: Array,
    }
    // data() {
    //     return {
    //         logo: '../../src/assets/dc-logo.png',
    //         links: [
    //         {
    //             text: "CHARACTERS",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "COMICS",
    //             url: "",
    //             current: true,
    //         },
    //         {
    //             text: "MOVIES",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "TV",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "GAMES",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "VIDEOS",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "FANS",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "NEWS",
    //             url: "",
    //             current: false,
    //         },
    //         {
    //             text: "SHOP",
    //             url: "",
    //             current: false,
    //         },
    //         ]
    //     }
    // }

}
</script>

<template>
    <header>

        <div class="logo">
            <img :src="logo" alt="">
        </div>

        <div class="lista">

            <nav>

                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :href=" link.url " :class="{active: link.current}"> {{ link.text }}</a>
                    </li>
                    
                </ul>

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

img{
    width: 100%;
    height: 100%;
}

header{
    display: flex;
    justify-content: space-around;
    height: 100px;
    align-items: center;
    // outline: 1px solid black;
    padding: $general-padding;

    .logo{
        width: 80px;
        // outline: 1px solid red;
    }
}

ul {
    list-style: none;
    margin: 3px;
}

li {
    display: inline;
}

    li a {
        display: inline;
        padding: 0 10px;
        text-decoration: none;
    }



</style>
