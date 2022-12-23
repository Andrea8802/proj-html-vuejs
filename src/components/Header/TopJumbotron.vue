<script>
export default {
    name: "TopJumbotron",
    data() {
        return {
            linkNav: [
                {
                    name: "HOME",
                    link: "#",
                    active: false
                },

                {
                    name: "ABOUT",
                    link: "#",
                    active: false
                },

                {
                    name: "PROJECTS",
                    link: "#",
                    active: false
                },

                {
                    name: "PROCESS",
                    link: "#",
                    active: true
                },

                {
                    name: "TESTIMONIALS",
                    link: "#",
                    active: false
                },
            ]
        }
    },
    methods: {
        itemClicked(item) {
            // azzerare item active
            this.linkNav.forEach(element => element.active ? element.active = false : "");

            // Assegnare stato active
            item.active = true;
        }
    }
}
</script>

<template>
    <div class="top">

        <!-- Logo -->
        <a href="#">
            <img src="../../assets/img/logo.svg" alt="Logo">
        </a>

        <!-- Links nav -->
        <nav>
            <ul>

                <!-- Links -->
                <li v-for="(item, index) in linkNav" :info="item" :key="index">
                    <a :href="item.link" :class="item.active ? 'item-selected' : ''" @click="itemClicked(item)">
                        {{ item.name }}
                    </a>
                </li>

                <!-- Icona profilo -->
                <li>
                    <fa icon="fa-solid fa-user" class="profile" />
                </li>

                <!-- Bottone -->
                <li>
                    <a href="#" class="button solid">
                        GET IN TOUCH
                    </a>
                </li>
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

            li {
                font-size: 14px;
            }

            a {
                color: white;

                &:hover {
                    color: $primary-color;
                }
            }

            .item-selected {
                color: $primary-color;
            }
        }

        .profile {
            color: white;
            font-size: 18px;
            cursor: pointer;

            &:hover {
                color: $primary-color;
            }
        }

    }
}
</style>