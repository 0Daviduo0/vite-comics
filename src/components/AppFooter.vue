<script>
export default{
    name: "AppFooter",

}
</script>

<template>
    <footer>

    </footer>
    <div class="account-and-socials">

        <div class="signup">

        </div>
        <div class="socials">
            
        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

footer{
    display: flex;
    height: 400px;
    background-color: green;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: $general-padding;

    .account-and-socials{
        display: flex;
        justify-content: space-between;
        background-color: #303030;
        background-color: #303030;
    }
        .signup{
            height: 100px;
            width: 50%;
            outline: 1px solid black;
        }

        .socials{
            height: 100px;
            width: 50%;
            outline: 1px solid black;
        }

}

</style>
