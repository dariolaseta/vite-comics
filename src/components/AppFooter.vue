<template>
    <footer>
        <nav class="container">
                <div class="first-block">
                    <div id="dc-comics">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li v-for="item in dcComics">
                                <a href="#">{{item}}</a>
                            </li>
                        </ul>
                    </div>
        
                    <div id="shop">
                        <h2>SHOP</h2>
                        <ul>
                            <li v-for="item in shops">
                                <a href="#">{{item}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
    
                <div class="second-block">
                    <div id="dc">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="item in dc">
                                <a href="#">{{item}}</a>
                            </li>
                        </ul>
                    </div>
        
                    <div id="sites">
                        <h2>SITES</h2>
                        <ul>
                            <li v-for="item in sites">
                                <a href="#">{{item}}</a>
                            </li>
                        </ul>
                    </div>
    
                </div>

                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
                </div>
        </nav>

        <div class="bottom-footer">
            <div class="container">
                <button>SIGN-UP NOW!</button>

                <div class="socials">
                    <ul>
                        <li><a href="#">FOLLOW US</a></li>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook logo"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter logo"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube logo"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest logo"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope logo"></a></li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="bottom-bar"></div>
    </footer>
</template>

<script>
export default {
    name: "AppFooter",
    data() {
        return {
            dcComics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shops: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dc: [
                "Terme of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPCS Certificates",
                "Ratings",
                "Shop Help",
                "Contact us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    footer{
        background-image: url("../assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;

        nav.container{
            display: flex;
            padding: 2rem 0;
            height: 100%;

            ul{
                padding: 1rem 0;

                li{
                    a{
                        color: #6e7069;
                    }
                    padding: .2rem 0;
                }
            }

            div.first-block{
                padding-right: 3rem;

                div#shop{
                    padding-bottom: 1rem;
                }
            }

            div.second-block{
                display: flex;
                
                div#dc{
                    padding-right: 3rem;
                }
            }

            div.logo{
                img{
                    position: relative;
                    top: -60px;
                    left: 300px;
                }
            }
        }

        div.bottom-footer{
            background-color: #303030;

            div.container{

                @include flex(row, space-between, center);

                button{
                    background: none;
                    border: 2px solid $blue;
                    padding: 1rem 1.5rem;
                    color: white;
                    font-size: 1rem;
                    cursor: pointer;
                }

                div.socials{
                    ul{
                        display: flex;
                        align-items: center;

                        li{
                            padding-left: 1rem;
                        }
                    }

                    a{
                        color: $blue;
                        font-size: 1.5rem;
                    }
                }
            }
        }

        div.bottom-bar{
            height: 50px;
            background-color: $black;
        }
    }
</style>