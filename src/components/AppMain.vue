<template>
    <div class="container">
        <h1>--&gtContent goes here &lt--</h1>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    @import "../styles/general.scss";

    div.container{
        @include flex();

        h1{
            margin: 0 auto;
            width: 50%;
        }
    }

</style>