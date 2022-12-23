<script>
export default {
    name: "Process",
}
</script>

<template>

    <!-- Testo blu -->
    <div class="blue-text">
        HOW IT WORKS IN PRATICE
    </div>

    <!-- Titolo -->
    <div class="title">

        <!-- Titolo con sfondo -->
        <div class="bg-title">
            Process
        </div>
        Management
    </div>

    <!-- Testo -->
    <p class="text">
        We work with innovative methodolgies to ensure that the entire reformatting process is done from start to finish
        as planned
    </p>


    <!-- Barra con i cerchi numerati -->
    <div class="bar">
        <div class="ball-container">
            <div class="ball">
                01
            </div>
        </div>

        <div class="ball-container">
            <div class="ball">
                02
            </div>
        </div>

        <div class="ball-container">
            <div class="ball">
                03
            </div>
        </div>

        <div class="ball-container">
            <div class="ball">
                04
            </div>
        </div>

        <div class="ball-container">
            <div class="ball">
                05
            </div>
        </div>


    </div>

    <!-- Card posizionate con i cerchi numerati -->
    <div class="card-list">
        <div class="card">

            <h3>
                Collection of information
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur.
            </p>

        </div>

        <div class="card">

            <h3>
                Strategic planning
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur.
            </p>

        </div>

        <div class="card">

            <h3>
                Assignament of responsabilities
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur.
            </p>

        </div>

        <div class="card">

            <h3>
                Formatting process
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur.
            </p>

        </div>

        <div class="card">

            <h3>
                Continuity formalization
            </h3>

            <p>
                Lorem ipsum dolor sit amet consectetur.
            </p>

        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.title {
    margin: 20px 0;
}

.text {
    width: 38%;
    text-align: center;
}

.bar {
    background-color: $light-primary-color;
    height: 5px;
    width: 100%;
    margin: 50px 0 0;
    @include d-flex(center, center);

    .ball-container {
        width: calc(100% / 6);

        .ball {
            @include d-flex(center, center);
            background-color: $light-primary-color;
            color: $primary-color;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            font-weight: bold;
            font-size: 18px;
            margin: auto;
            cursor: pointer;

            &:hover {
                border: 3px solid $primary-color
            }
        }
    }
}

.card-list {
    @include d-flex(center, center);
    width: 100%;

    .card {
        @include d-flex(space-evenly, center);
        flex-direction: column;
        width: calc(100% / 6);


        h3 {
            width: 60%;
            text-align: center;
            color: $dark-text-color;
            margin: 40px 0 20px;
        }

        p {
            width: 80%;
            text-align: center;
        }

    }
}
</style>