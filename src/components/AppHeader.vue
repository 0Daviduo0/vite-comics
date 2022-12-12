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
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
                    </li>
                    <li>
                        <a href="">CHARACTERS</a>
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
    height: 100px;
    outline: 1px solid black;
}

logo{
        outline: 1px solid red;
    }

</style>
