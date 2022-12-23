<script>
export default {
    name: "BottomFooter"
}
</script>

<template>

    <!-- Testo -->
    <section>
        <div class="text">
            Enjoy the low price. We are tracking any intention of privacy.
        </div>

        <div class="text">
            &#169; NEXGEN is Proudly Powered by <a href="#">Codings.</a>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    @include d-flex(space-between, center);
    height: 70px;
    padding: 0 290px;
    font-size: 12px;
    background-color: #0d0d11;
    color: $light-text-color;

    a {
        color: darkcyan;
        text-decoration: underline;
    }
}
</style>
