<script>
export default {
    name: "InfoCompany"
}
</script>

<template>
    <section>
        <div class="container">
            <div>
                <fa icon="fa-solid fa-clock" />
                Open Hours Man - Sat - 9:00 - 18:00
            </div>

            <div class="info">
                <div>
                    <fa icon="fa-solid fa-phone" />
                    +1 (305) 1234-5678
                </div>
                <div>
                    <fa icon="fa-solid fa-envelope" />
                    hello@example.com
                </div>

                <div class="social">
                    <fa icon="fa-brands fa-facebook-f" />
                    <fa icon="fa-brands fa-twitter" />
                    <fa icon="fa-brands fa-linkedin-in" />
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

section {
    background-color: #21333e;
    height: $height-header;
    width: 100%;
    font-size: 12px;
    color: $light-text-color;

    .container {
        @include d-flex(space-between, center);
    }

    .info {
        @include d-flex(space-evenly, center);
        gap: 15px;

        .social {
            @include d-flex(space-evenly, center);
            gap: 30px;
        }
    }
}
</style>
