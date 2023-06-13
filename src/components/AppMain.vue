<script>
import companyPresentation from './subMain/companyPresentation.vue';
import vision from './subMain/vision.vue';
import askExpert from './subMain/askExpert.vue';
import teamResponse from './subMain/teamResponse.vue';

export default {
    name: "AppMain",
    components: {
        companyPresentation,
        vision,
        askExpert,
        teamResponse

    }
}


</script>

<template>
    <div class="containerMain">
        <companyPresentation />
        <vision />
        <askExpert />
        <teamResponse />


    </div>
</template>

<style lang="scss" scoped>
@use '../components/style/partials/variables' as *;
@use '../components/style/general.scss' as *;

.containerMain {
    min-height: 10rem;
    margin-top: 28rem;
    width: 100%;
    background-color: $secondary;
}
</style>
