<template>
    <header>
        <div class="header-container">
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
    @import "../styles/general.scss";

    header{
        div.header-container{

            @include flex(row, space-between, center);
            width: 50%;
            margin: 0 auto;
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