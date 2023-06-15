<template>
    <footer>
        <nav class="container margin-auto">
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
        </nav>
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

        @include flex();
        nav.container{
            display: flex;
            margin-top: 2rem;
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
            }

            div.second-block{
                display: flex;

                div#dc{
                    padding-right: 3rem;
                }
            }
        }
    }
</style>