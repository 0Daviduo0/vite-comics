<script>
export default {
    name: "AppFooter",
    data() {
        return {
            menu: [
                {
                    title: "DC COMICS",
                    links: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News",
                    ]
                },
                {
                    title: "SHOP",
                    links: [
                        "Shop DC",
                        "Shop DC Collectables"
                    ]
                },
                {
                    title: "DC",
                    links: [
                        "Terms Of Use",
                        "Privacy Policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratigs",
                        "Shop Help",
                        "Contact Us",
                    ]
                },
                {
                    title: "SITES",
                    links: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa",
                    ]
                },
            ],
            socials: [
            {
                SocialIcon: "../../src/assets/footer-facebook.png",
                SocialName: "Facebook",
            },
            {
                SocialIcon: "../../src/assets/footer-twitter.png",
                SocialName: "twitter",
            },
            {
                SocialIcon: "../../src/assets/footer-youtube.png",
                SocialName: "youtube",
            },
            {
                SocialIcon: "../../src/assets/footer-pinterest.png",
                SocialName: "pinterest",
            },
            {
                SocialIcon: "../../src/assets/footer-periscope.png",
                SocialName: "periscope",
            },
            ],
        }
    }

}
</script>

<template>
    <footer>

        <div class="side-links">

            <div class="vertical">

                <div class="menu">
                <div class="title">
                    DC COMICS
                </div>

                <div class="object">
                    <ul>
                        <li>
                            <a href=""> Characters </a>
                        </li>
                        <li>
                            <a href=""> Comics </a>
                        </li>
                        <li>
                            <a href=""> Movies </a>
                        </li>
                        <li>
                            <a href=""> TV </a>
                        </li>
                        <li>
                            <a href=""> Games </a>
                        </li>
                        <li>
                            <a href=""> Videos </a>
                        </li>
                        <li>
                            <a href=""> News </a>
                        </li>
                    </ul>
                </div>

                </div>
                <div class="menu">
                <div class="title">
                    SHOP
                </div>

                <div class="object">
                    <ul>
                        <li>
                            <a href=""> Shop DC </a>
                        </li>
                        <li>
                            <a href=""> Shop DC Collectables </a>
                        </li>
                    </ul>
                </div>

            </div>

            </div>

            <div class="menu">
            <div class="title">
                DC
            </div>

            <div class="object">
                <ul>
                    <li>
                        <a href=""> Terms Of Use </a>
                    </li>
                    <li>
                        <a href=""> Privacy Policy (New) </a>
                    </li>
                    <li>
                        <a href=""> Ad Choices </a>
                    </li>
                    <li>
                        <a href=""> Advertising </a>
                    </li>
                    <li>
                        <a href=""> Jobs </a>
                    </li>
                    <li>
                        <a href=""> Subcriptions </a>
                    </li>
                    <li>
                        <a href=""> Talent Workshops </a>
                    </li>
                    <li>
                        <a href=""> CPSC Certificates </a>
                    </li>
                    <li>
                        <a href=""> Ratings </a>
                    </li>
                    <li>
                        <a href=""> Shop Help </a>
                    </li>
                    <li>
                        <a href=""> Contact Us </a>
                    </li>

                </ul>
            </div>

            </div>
            <div class="menu">
            <div class="title">
                SITES
            </div>

            <div class="object">
                <ul>
                    <li>
                        <a href=""> DC </a>
                    </li>
                    <li>
                        <a href=""> MAD Magazine </a>
                    </li>
                    <li>
                        <a href=""> DC Kids </a>
                    </li>
                    <li>
                        <a href=""> DC Universe </a>
                    </li>
                    <li>
                        <a href=""> DC Power Visa </a>
                    </li>

                </ul>
            </div>

            </div>

        </div>

        <div class="dc-big-logo-img">
            <img class="big-logo" src="../../src/assets/dc-logo-bg.png" alt="">
        </div>

        

    </footer>
    <div class="account-and-socials">

        <div class="signup">

            <div class="signup-button">
                SIGN-UP NOW!
            </div>

        </div>
        <div class="socials">

            <div class="followUs">
                FOLLOW US
            </div>

            <div class="socialIcon" v-for="(social, index) in socials" :key="index">
                <img :src=" social.SocialIcon " :alt=" social.SocialName ">
            </div>

        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

footer {
    display: flex;
    height: 400px;
    background-image: url('../../src/assets/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    padding: $general-padding;
    padding-top: 80px;
    font-size: 18px;
    color: rgb(255, 255, 255);
    overflow: hidden;
    position: relative;

    .side-links{
        display: flex;
    }

        ul {
        list-style: none;
        padding: 0;
        list-style-type: none;
        }

        li a {
        text-decoration: none;
        color: #919292;
    }
}

.menu {
    padding: 0 20px;
}

.big-logo{
    position: absolute;
    right: 200px;
    bottom: -50px;
}

.account-and-socials {
    display: flex;
    justify-content: space-between;
    background-color: #303030;
    background-color: #303030;
}

.signup {
    height: 100px;
    width: 50%;
    // outline: 1px solid black;
    display: flex;
    padding: $general-padding;
    align-items: center;

    .signup-button{
        border: 3px $main-color2 solid;
        padding: 15px;
        color: #fff;
    }
}

.socials {
    padding: $general-padding;
    height: 100px;
    width: 50%;
    // outline: 1px solid black;
    display: flex;
    align-items: center;
    justify-content: right;

    .followUs{
        padding: 20px;
        color: $main-color2;
        font-size: 20px;
        font-weight: 700;
    }

    .socialIcon{
        padding: 10px;
    }
}
</style>
