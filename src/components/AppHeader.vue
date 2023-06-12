<script>
import NavHeader from './subHeader/navHeader.vue';
import presentation_smItems from './subHeader/presentation_smItems.vue';
import jumbotron from './subHeader/jumbotron.vue';
export default {
    name: "AppHeader",
    components: {
        presentation_smItems,
        NavHeader,
        jumbotron
    }
}


</script>

<template>
    <div class="container">
        <presentation_smItems />
        <navHeader />
        <jumbotron />


    </div>
</template>

<style lang="scss" scoped>
@use '../components/style/partials/variables' as *;
@use '../components/style/general.scss' as *;

.container {
    border-top: 4px solid $primary;
    height: 10rem;
    width: 100%;
    background-color: $secondary;
}
</style>
