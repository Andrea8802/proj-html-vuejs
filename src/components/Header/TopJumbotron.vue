<script>
export default {
    name: "TopJumbotron"
}
</script>

<template>
    <div class="top">
        <img src="../../assets/img/logo.svg" alt="Logo">
        <nav>
            <ul>
                <li>A</li>
                <li>A</li>
                <li>A</li>
                <li>A</li>
                <li>A</li>
                <li>A</li>
                <li>A</li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

.background {
    background-color: rgba($color: black, $alpha: 0.4);
    height: 100%;
    width: 100%;

    .top {
        width: 100%;
        padding-top: 20px;
        @include d-flex(space-between, center);

        img {
            width: 110px;
        }

        ul {
            list-style: none;
            @include d-flex(space-evenly, center);
            gap: 30px;
            color: white;
            font-weight: bold;
        }
    }
}
</style>