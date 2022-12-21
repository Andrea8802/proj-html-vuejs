<script>
import TopJumbotron from '../components/TopJumbotron.vue'
import MiddleJumbotron from '../components/MiddleJumbotron.vue'

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
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

section {
    background-image: url("../assets/img/bg-4.jpg");
    height: calc(100vh - $height-header);
    background-size: cover;

    .background {
        background-color: rgba($color: black, $alpha: 0.4);
        height: 100%;
        width: 100%;
    }


}
</style>