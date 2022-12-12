<script>
export default{
    name: "AppMain",

}
</script>

<template>
    <main>
        <div class="content">

        --> Content goes here &lt--

        </div>
        <div class="rapid_components">

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
    }
}


</style>
