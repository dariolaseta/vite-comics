<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="dc logo">
            </div>
    
            <nav>
                <ul>
                    <li v-for="link in links">
                        <a href="#">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "AppHeader",
    data(){
        return{
            links:[
            {
                    text: "CHARACTERS",
                },
                {
                    text: "COMICS",
                },
                {
                    text: "MOVIES",
                },
                {
                    text: "TV",
                },
                {
                    text: "GAMES",
                },
                {
                    text: "COLLECTIBLES",
                },
                {
                    text: "VIDEOS",
                },
                {
                    text: "FANS",
                },
                {
                    text: "NEWS",
                },
                {
                    text: "SHOP",
                },
            ]
        }
    }
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