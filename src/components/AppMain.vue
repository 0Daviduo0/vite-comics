<script>
export default{
    name: "AppMain",
    props: {
        components: Array,
        jumbotron: String,
        Card: Array,
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

            <div class="tag">
                CURRENT SERIES
            </div>

            <div class="comics-collection">
                <div class="comic-card" v-for="(comic, index) in Card" :key="index">
                    <div class="comic-thumbnail">
                        <img :src="comic.thumb" alt="">
                    </div>

                    <div class="comic-title">
                        {{comic.series}}
                    </div>
                    
                </div>
            </div>

            <div class="load-more">
                LOAD MORE
            </div>

        

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
        background-color: $main-color1;
        color: #fff;
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding: $general-padding;
        position: relative;
        padding-bottom: 30px;

        .tag{
            position: absolute;
            top: -25px;
            background-color: $main-color2;
            padding: 10px 20px;
            font-size: 20px;
            font-weight: 600;
        }

        .comics-collection{
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            grid-template-rows: repeat(2, 1fr);
            grid-column-gap: 20px;
            grid-row-gap: 20px;
            padding-top: 50px;
            width: 100%;
            margin-bottom: 30px;

            .comic-card{
                // outline: 1px solid black;
                height: 280px;
                width: 200px;
                display: flex;
                flex-direction: column;

                .comic-thumbnail{
                    width: 200px;
                    height: 200px;
                    overflow: hidden;

                }

                .comic-title{
                    padding-top: 20px;
                    
                }
            }

        }

        .load-more{
            background-color: $main-color2;
            margin: auto;
            padding: 10px;
            font-size: 20px;
            font-weight: 600;
            text-align: center;
            width: 250px;
        }
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
