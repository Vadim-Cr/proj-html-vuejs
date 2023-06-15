<script>
import socialIcons from '.././socialIcons.vue';

export default {
    name: "bottomFooter",
    components: {
        socialIcons
    },
    data() {
        return {
            copyright: '<i class="fa-regular fa-copyright"></i> Copyright 2012-2020',
            navFooter: ['Avada Theme by Theme Fusion',
                'All Rights Reserved',
                'Powered By WordPress']
        }
    }
}
</script>
<template>
    <div class="copyRContainer">
        <div class="copyRPresentation">
            <div class="copyRPresentationLeft">
                <h2>CALL OUR EXPERTS TODAY 1.800.555.6789</h2>
                <div class="leftCopy">
                    <div v-html="copyright" class="copyR"> </div>
                    <ul>
                        <li v-for="(item, index) in navFooter" :key="index">
                            {{ item }}
                        </li>
                    </ul>
                </div>
            </div>
            <div class="copyRPresentationRight">
                <socialIcons />
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;
@use '../style/partials/mixins.scss' as *;
@use '../style/general.scss' as *;

.copyRContainer {
    background-color: $tertiary;
    height: 20rem;
    @include center_flex;
    border-top: 1px solid #dad9d9;

    .copyRPresentation {
        @include center_between;
        width: 70%;

        .copyRPresentationLeft {
            height: 7.5rem;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;

            .leftCopy {
                @include center_flex;
                margin-top: 2rem;

                .copyR {
                    color: $quinary;
                    margin: auto;

                    &:hover {
                        color: $primary;
                        font-weight: bold;
                        background-color: $secondary;
                        border: 2px solid $primary;
                        padding: 0.5rem;
                        cursor: pointer;
                    }
                }

                ul {
                    list-style: none;
                    @include center_flex;

                    li {
                        color: $quinary;
                        padding-left: 1rem;
                        border-left: 2px solid $quinary;
                        margin-left: 1rem;

                        &:hover {
                            color: $primary;
                            font-weight: bold;
                            background-color: $secondary;
                            border: 2px solid $primary;
                            padding: 0.5rem;
                            cursor: pointer;
                        }
                    }
                }


            }
        }

        .copyRPresentationRight {
            height: 7rem;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;

        }

    }
}
</style>

