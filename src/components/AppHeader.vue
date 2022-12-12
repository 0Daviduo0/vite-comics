<script>
export default{
    name: "AppHeader",

}
</script>

<template>
    <header>

        <div class="logo">

        </div>

        <div class="lista">

            <nav>

                <ul>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">COMICS</a>
                    </li>
                    <li>
                        <a href="">MOVIES</a>
                    </li>
                    <li>
                        <a href="">TV</a>
                    </li>
                    <li>
                        <a href="">GAMES</a>
                    </li>
                    <li>
                        <a href="">COLLECTABLES</a>
                    </li>
                    <li>
                        <a href="">VIDEOS</a>
                    </li>
                    <li>
                        <a href="">FANS</a>
                    </li>
                    <li>
                        <a href="">NEWS</a>
                    </li>
                    <li>
                        <a href="">SHOP</a>
                    </li>
                </ul>

            </nav>

        </div>

    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

header{
    display: flex;
    justify-content: space-around;
    height: 100px;
    align-items: center;
    outline: 1px solid black;
    padding: $general-padding;

    .logo{
        outline: 1px solid red;
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
        padding: 2px;
        text-decoration: none;
    }



</style>
