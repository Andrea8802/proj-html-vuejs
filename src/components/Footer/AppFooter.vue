<script>
import LeftTopFooter from './LeftTopFooter.vue'
import RightTopFooter from './RightTopFooter.vue'
import BottomFooter from './BottomFooter.vue'

export default {
    name: "AppFooter",
    components: {
        BottomFooter,
        LeftTopFooter,
        RightTopFooter
    }
}
</script>

<template>

    <footer>
        <section class="top-footer">
            <LeftTopFooter />
            <RightTopFooter />
        </section>

        <BottomFooter />
    </footer>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

footer {
    background-color: $bg-black;
    width: 100%;

    .top-footer {
        @include d-flex(center, center);
        gap: 50px;
        height: 680px;
        width: 85%;
        margin: auto;
    }
}
</style>
