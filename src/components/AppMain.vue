<script>
export default{
    name: "AppMain",
    data() {
        return {
            components: [
            {
                image: "../../imgs/buy-comics-digital-comics.png",
                text: "DIGITAL COMICS",
            },
            {
                image: "../../imgs/buy-comics-merchandise.png",
                text: "DC MERCHANDISE",
            },
            {
                image: "../../imgs/buy-comics-subscriptions.png",
                text: "SUBSCRIPTION",
            },
            {
                image: "../../imgs/buy-comics-shop-locator.png",
                text: "COMIC SHOP LOCATOR",
            },
            {
                image: "../../imgs/buy-dc-power-visa.svg",
                text: "DC POWER VISA",
            },
            ]
        }
    }

}
</script>

<template>
    <main>
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
    outline: 1px solid black;

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
