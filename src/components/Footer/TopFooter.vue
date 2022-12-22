<script>
import LeftTopFooter from './LeftTopFooter.vue'
import RightTopFooter from './RightTopFooter.vue'


export default {
    name: "TopFooter",
    components: {
        LeftTopFooter,
        RightTopFooter
    }
}
</script>

<template>

    <section>
        <div class="footer-cont">
            <LeftTopFooter />
            <RightTopFooter />
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-color: $bg-black;
    width: 100%;

    .footer-cont {
        @include d-flex(center, center);
        gap: 30px;
        height: 680px;
        width: 75%;
        margin: auto;
    }

}
</style>
