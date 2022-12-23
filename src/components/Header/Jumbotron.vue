<script>
import TopJumbotron from './TopJumbotron.vue'
import MiddleJumbotron from './MiddleJumbotron.vue'

export default {
    name: "Jumbotron",
    components: {
        TopJumbotron,
        MiddleJumbotron
    }
}
</script>

<template>
    <section>
        <div class="background">
            <div class="container">
                <TopJumbotron />
                <MiddleJumbotron />
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;

section {
    background-image: url("../../assets/img/bg-4.jpg");
    height: calc(100vh - 45px);
    background-size: cover;

    .background {
        background-color: rgba($color: $bg-black, $alpha: 0.5);
        height: 100%;
        width: 100%;
    }
}
</style>