<script>
export default {
    name: "FeaturesCard"
}
</script>

<template>
    <div class="card">
        <div class="icon">
            <fa icon="fa-solid fa-user-group" />
        </div>
        <h3>
            Human Capital
        </h3>
        <p>
            Humanizing business: Harness the power of technology to improve the way people work.
        </p>
    </div>

    <div class="card">
        <div class="icon">
            <fa icon="fa-solid fa-chart-pie" />
        </div>
        <h3>
            Core Business
        </h3>
        <p>
            It takes innovative approaches to transform, modernize, and run existing platforms.
        </p>
    </div>

    <div class="card">
        <div class="icon">
            <fa icon="fa-solid fa-gauge-high" />
        </div>
        <h3>
            Performance
        </h3>
        <p>
            Archieving maximum impact and value from investments in finance and supply chain.
        </p>
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

.card {
    height: 250px;
    width: 280px;
    background-color: white;
    padding: 30px;

    .icon {
        background-color: #daeced;
        color: $primary-color;
        border-radius: 50%;
        display: inline-block;
        font-size: 22px;
        width: 50px;
        height: 50px;
        @include d-flex(center, center)
    }

    h3 {
        font-size: 20px;
        color: #202427;
        margin: 20px 0;
    }

    p {
        color: darkgray;
        font-size: 14px;
    }
}
</style>