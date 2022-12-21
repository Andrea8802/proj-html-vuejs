<script>
export default {
    name: "Jumbotron"
}
</script>

<template>
    <section>
        <div class="background">
            <div class="container">
                <div class="logo-nav">
                    <img src="../assets/img/logo.svg" alt="Logo">
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

        .logo-nav {
            width: 100%;

            @include d-flex(between, center);

            img {
                width: 100px;
            }

            ul {
                list-style: none;
                @include d-flex(evenly, center);
                gap: 30px;
            }
        }
    }


}
</style>