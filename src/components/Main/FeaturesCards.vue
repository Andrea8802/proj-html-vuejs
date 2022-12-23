<script>
export default {
    name: "FeaturesCards"
}
</script>

<template>
    <div class="card">

        <!-- Icona -->
        <div class="icon">
            <fa icon="fa-solid fa-user-group" />
        </div>

        <!-- Titolo -->
        <h3>
            Human Capital
        </h3>

        <!-- Testo -->
        <p>
            Humanizing business: Harness the power of technology to improve the way people work.
        </p>
    </div>

    <div class="card">

        <!-- Icona -->
        <div class="icon">
            <fa icon="fa-solid fa-chart-pie" />
        </div>

        <!-- Titolo -->
        <h3>
            Core Business
        </h3>

        <!-- Testo -->
        <p>
            It takes innovative approaches to transform, modernize, and run existing platforms.
        </p>
    </div>

    <div class="card">

        <!-- Icona -->
        <div class="icon">
            <fa icon="fa-solid fa-gauge-high" />
        </div>

        <!-- Titolo -->
        <h3>
            Performance
        </h3>

        <!-- Testo -->
        <p>
            Archieving maximum impact and value from investments in finance and supply chain.
        </p>
    </div>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/mixins' as *;
@use '../../styles/partials/variables' as *;

.card {
    height: 250px;
    width: 280px;
    background-color: white;
    padding: 30px;
    border-radius: 5px;

    &:hover {
        box-shadow: 0px 0px 30px rgba($color: $light-text-color, $alpha: 0.5);
    }

    .icon {
        background-color: $light-primary-color;
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
        color: $dark-text-color;
        margin: 20px 0;
    }

    p {
        font-size: 14px;
    }
}
</style>