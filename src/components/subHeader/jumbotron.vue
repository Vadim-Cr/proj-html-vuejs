<script>

export default {
    name: "jumbotron",
}
</script>

<template>
    <div class="jumboContainer">
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.jumboContainer {
    height: 30rem;
    background-image: url(../../assets/img/video_law_home_preview.jpg);
}
</style>
