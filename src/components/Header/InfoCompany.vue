<script>
export default {
    name: "InfoCompany"
}
</script>

<template>
    <section>
        <div class="container">

            <!-- Info azienda -->
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

                <!-- Social -->
                <div class="social">
                    <fa icon="fa-brands fa-facebook-f" class="icon" />
                    <fa icon="fa-brands fa-twitter" class="icon" />
                    <fa icon="fa-brands fa-linkedin-in" class="icon" />
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
    height: 45px;
    width: 100%;
    font-size: 12px;
    color: $light-text-color;

    .container {
        @include d-flex(space-between, center);
    }

    .info {
        @include d-flex(space-evenly, center);
        gap: 15px;

        & div:hover {
            text-decoration: underline;
            cursor: pointer;
        }

        .social {
            @include d-flex(space-evenly, center);
            gap: 30px;

            & .icon:hover {
                color: $primary-color;
                cursor: pointer;
            }
        }
    }
}
</style>
