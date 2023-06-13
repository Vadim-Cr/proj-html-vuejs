<script>

import visionCard from '../subMain/visionCard.vue';
export default {
    name: "companyPresentation",
    data() {
        return {
            // created the array for the NAV
            visionArray: [
                {
                    icon: 'fa-solid fa-check',
                    title: 'A Global View',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    icon: 'fa-solid fa-check',
                    title: 'Expert Lawyers',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    icon: 'fa-solid fa-check',
                    title: 'Client Focus',
                    text: ' Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                },
                {
                    icon: 'fa-solid fa-check',
                    title: 'Local Knowledge',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
                }
            ]
        }
    },
    components: {
        visionCard
    }
}
</script>
<template>
    <div class="visionContainer">
        <div class="visionPresentation">
            <visionCard :visionInfo="visionArray" />
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.visionContainer {
    background-color: $tertiary;
    height: 25rem;
    @include center_flex;
    border-top: 1px solid #dad9d9;

    .visionPresentation {
        width: 70%;
        @include center_flex;
        height: 20rem;
    }
}
</style>

