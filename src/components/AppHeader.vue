<template>
    <header>
        <div class="container">
            <div class="logo">

            </div>
    
            <nav>
    
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
            height: 50px;
            width: 50px;
            background-color: red;
        }

        nav{
            height: 50px;
            width: 200px;
            background-color: red;
        }
    }
</style>