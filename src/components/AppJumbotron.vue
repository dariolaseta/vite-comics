<template>
    <div class="jumbo">
        <img src="../assets/img/jumbotron.jpg" alt="jumbo img">
    </div>
</template>

<script>
export default {
    name: "AppJumbotron"
}
</script>

<style lang="scss" scoped>
    div.jumbo{
        height: 450px;

        img{
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: 0 2rem;
        }
    }
</style>