<template>
    <main>
        <div class="container">
            <h1 class="margin-auto">--&gtContent goes here &lt--</h1>
        </div>
    </main>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;

    main{
        background-color: $black;
        div.container{
            @include flex();
    
            h1{
                width: 100%;
            }
        }
    }

</style>