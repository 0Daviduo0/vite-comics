<script>
export default{
    name: "AppMain",
    props: {
        components: Array,
        jumbotron: String,
        comics: Array,
    }
    // data() {
    //     return {
    //         components: [
    //         {
    //             image: "../../src/assets/buy-comics-digital-comics.png",
    //             text: "DIGITAL COMICS",
    //         },
    //         {
    //             image: "../../src/assets/buy-comics-merchandise.png",
    //             text: "DC MERCHANDISE",
    //         },
    //         {
    //             image: "../../src/assets/buy-comics-subscriptions.png",
    //             text: "SUBSCRIPTION",
    //         },
    //         {
    //             image: "../../src/assets/buy-comics-shop-locator.png",
    //             text: "COMIC SHOP LOCATOR",
    //         },
    //         {
    //             image: "../../src/assets/buy-dc-power-visa.svg",
    //             text: "DC POWER VISA",
    //         },
    //         ],
            
    //     }
    // }

}
</script>

<template>
    <main>
        <div class="jumbotron">
            
        </div>
        <div class="content">

        --> Content goes here &lt--

        </div>
        <div class="rapid_components">

        <div class="component" v-for="(component, index) in components" :key="index">

            <img :src="component.image" alt="">
            <div class="title"> {{ component.text }} </div>

        </div>

        </div>

    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

main{
    display: flex;
    flex-direction: column;
    // outline: 1px solid black;

    .jumbotron{
        height: 500px;
        color: #fff;
        display: flex;
        align-items: center;
        // Da fixara con "jumbotron" in App.vue usando prop
        background-image: url("../../src/assets/jumbotron.jpg");
        background-repeat: no-repeat;
    }

    .content {
        height: 150px;
        background-color: $main-color1;
        color: #fff;
        display: flex;
        align-items: center;
        padding: $general-padding;
    }
    .rapid_components {
        height: 150px;
        background-color: $main-color2;
        display: flex;
        justify-content: center;

        .component{
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 50px;
        }

            img{
                height: 70px;
            }

            .title{
                color: #fff;
                margin-left: 20px;
            }
    }
}


</style>
