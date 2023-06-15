<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>
    
            <nav>
                <ul>
                    <li><a href="#">CHARACTERS</a></li>
                    <li class="active"><a href="#">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    header{
        div.container{
            display: flex;
            justify-content: space-between;
            margin: 1rem auto;
            height: 100%;
        }

        div.logo{
            img{
                width: 80%;
            }
        }

        nav{
            display: flex;
            align-items: center;
            font-size: .8rem;

            ul{
                display: flex;
                
                li{
                    padding-left: 2rem;
                }

                li.active a{
                    color: $blue;
                    border-bottom: 5px solid $blue;
                    padding-bottom: 3rem;
                }
            }

            a{
                color: black;
            }
        }
    }
</style>