<template>
    <div class="jumbo">

    </div>
</template>

<script>
export default {
    name: 'Jumbo',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
    .jumbo{
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        height: 300px;
    }
</style>