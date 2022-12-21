<script>
import FeaturesCard from './FeaturesCard.vue';
export default {
    name: "AppMain",
    components: {
        FeaturesCard
    }
}
</script>

<template>
    <section class="features">
        <FeaturesCard />
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.features {
    height: 480px;
    background-color: $bg-gray;
    @include d-flex(center, center);
    gap: 25px
}
</style>