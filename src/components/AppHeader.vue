<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            navTitles: [
                {
                    href: "#corsi",
                    title: "Nuestros cursos"
                },
                {
                    href: "#chisiamo",
                    title: "Quienes somos"
                },
                {
                    href: "#prova",
                    title: "Acceso Web Test"
                },
                {
                    href: "#testimonials",
                    title: "Opiniones"
                },
                {
                    href: "#Q&A",
                    title: "Preguntas frequentes"
                },
                {
                    href: "#mail",
                    title: "Contactanos"
                },

            ]
        }
    }
}
</script>

<template>
    <header>
        <nav class="navbar navbar-expand-lg ">
            <div class="container-fluid ">
                <a class="navbar-brand text-white" href="#">
                    <img src="../assets/img/opopreparadora_img_white_preview_rev_1.png" alt="Logo"
                        class="d-inline-block align-text-center">
                    Opopreparadora
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar"
                    aria-controls="offcanvasNavbar" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon "></span>
                </button>
                <div class="offcanvas offcanvas-end bg-black" tabindex="-1" id="offcanvasNavbar"
                    aria-labelledby="offcanvasNavbarLabel">
                    <div class="offcanvas-header bg-light">
                        <h5 class="offcanvas-title" id="offcanvasNavbarLabel">Opopreparadora</h5>
                        <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                    </div>
                    <div class="offcanvas-body">
                        <div class="row row-cols-1 row-cols-lg-6 align-items-lg-center">
                            <div class="col" v-for="title, index in navTitles" :key="index">
                                <a :href="title.href">{{ title.title }}</a>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/variables/mixins' as *;

header {
    background-color: black;
    position: fixed;
    z-index: 999;
    width: 100%;
    height: 60px;

    @media screen and (min-width: 750px) {
        height: 80px;
    }

    .container-fluid {
        align-items: flex-start;

        @media screen and (min-width: 992px) {
            align-items: flex-end;
        }

        @media screen and (min-width: 1830px) {
            align-items: baseline;
        }

        .navbar-brand {
            width: 20%;
            font-size: .8rem;

            @media screen and (min-width: 600px) {
                font-size: 1.2rem;
            }

            img {
                width: 75%;

                @media screen and (min-width: 750px) {
                    width: 60%;
                    height: 60px;
                }

                @media screen and (min-width: 1400px) {
                    width: 45%;
                }
            }

        }

        .navbar-toggler {
            background-color: white;
            font-size: .8rem;
            padding: .2rem .5rem;
            margin-top: 6px;

            @media screen and (min-width: 750px) {
                font-size: 1.2rem;
                margin-top: 14px;
            }
        }

        .offcanvas.offcanvas-end {
            width: 55%;

            .offcanvas-body {
                justify-content: space-around;

                .row {
                    width: 75%;

                    .col {
                        margin-bottom: 1rem;

                        a:hover {
                            color: gold;
                            border-bottom: 5px solid gold;
                        }
                    }
                }
            }
        }
    }
}
</style>