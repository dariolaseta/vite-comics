<template>
    <footer>
        <nav class="container">
                <div class="first-block">
                    <div id="dc-comics">
                        <h2>DC COMICS</h2>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
        
                    <div id="shop">
                        <h2>SHOP</h2>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>
    
                <div class="second-block">
                    <div id="dc">
                        <h2>DC</h2>
                        <ul>
                            <li>Terms of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
        
                    <div id="sites">
                        <h2>SITES</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
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
                    padding: .2rem 0;
                    color: #6e7069;
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