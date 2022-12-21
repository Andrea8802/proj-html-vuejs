<script>
export default {
    name: "Process",
}
</script>

<template>
    <div class="blue-text">
        HOW IT WORKS IN PRATICE
    </div>

    <div class="title">
        <div class="bg-title">
            Process
        </div>
        Management
    </div>

    <p class="text">
        We work with innovative methodolgies to ensure that the entire reformatting process is done from start to finish
        as planned
    </p>


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
    font-size: 40px;
    font-weight: bold;
    color: $dark-text-color;
    margin: 20px 0;
}

.text {
    color: $text-color;
    width: 38%;
    font-size: 14px;
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
            background-color: $light-primary-color;
            color: $primary-color;
            border-radius: 50%;
            padding: 10px;
            width: 40px;
            height: 40px;
            font-weight: bold;
            font-size: 18px;
            margin: auto
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
            color: $text-color;
            width: 80%;
            text-align: center;
        }

    }
}
</style>