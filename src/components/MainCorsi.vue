<script>
export default {
    name: 'MainCorsi',
    data() {
        return {
            corsi: [
                {
                    name: 'Ja C1',
                    backgroundImg: 'corso_JA_C1.jpg'
                },
                {
                    name: 'Ja C2',
                    backgroundImg: 'corso_JA_C2.jpg'
                },
                {
                    name: 'LO',
                    backgroundImg: 'corso_LO.jpg'
                },
                {
                    name: 'Age C1',
                    backgroundImg: 'corso_Age_C1.jpg'
                },
                {
                    name: 'Age C2',
                    backgroundImg: 'corso_Age_C2.jpg'
                },

            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section id="corsi">
        <div class="corso-container">
            <h2 class="corsi-title text-center fs-4 ">Cursos ofrecidos: tu pasaporte para el éxito en las oposiciones</h2>
            <p class="text-center">¡Bienvenido al emocionante viaje hacia tu futuro como funcionario/a con Opopreparadora! <br>
                Hemos diseñado cursos de preparación completa y flexible para que alcances tus metas profesionales en el
                sector público.</p>
            <div class="container-fluid wdt-80">
                <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3">
                    <div class="col" v-for="(corso, index) in corsi" :key="index">
                        <a href="#Modal" data-bs-toggle="modal" role="button" aria-controls="exampleModal">
                            <div class="badge ">
                                <img :src="getImagePath(corso.backgroundImg)" alt="">
                            </div>
                        </a>
                        <div class="modal fade" id="Modal" tabindex="-1" aria-labelledby="exampleModalLabel"
                            aria-hidden="true">
                            <div class="modal-dialog modal-dialog-centered modal-dialog-scrollable modal-lg">
                                <div class="modal-content">
                                    <div class="modal-header">
                                        <h1 class="modal-title fs-5" id="exampleModalLabel">Modal title</h1>
                                        <button type="button" class="btn-close" data-bs-dismiss="modal"
                                            aria-label="Close"></button>
                                    </div>
                                    <div class="modal-body">
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa eveniet, ipsam porro
                                        repudiandae dolorum exercitationem quod illum quaerat. Tenetur esse autem veritatis
                                        possimus ipsa rerum velit quibusdam doloremque, qui magni!
                                    </div>
                                    <div class="modal-footer">
                                        <button type="button" class="btn btn-secondary"
                                            data-bs-dismiss="modal">Close</button>
                                        <a href="mailto:info@opopreparadora.com" class="btn btn-primary w-25">Me
                                            interesa</a>
                                    </div>
                                </div>
                            </div>
                        </div>


                    </div>
                </div>
                <p class="text-center mt-5">Independientemente de la opción que elijas, en Opopreparadora estamos comprometidos a proporcionarte los recursos
                    y el apoyo necesarios para alcanzar el éxito en tu oposición. <br> Únete a nosotros y comienza tu viaje hacia la
                    emocionante carrera de trabajar en el sector público.
                    <br> ¡Estamos aquí para ayudarte a alcanzar tu meta!
                </p>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables/mixins' as *;

.corso-container {
    padding: 0 40px;

    a {
        height: 100%;
        display: block;
        width: 100%;

        .badge {
            width: 100%;
            height: 250px;

            img {
                @media screen and (min-width: 430px) {
                    width: 75%;
                }

                @media screen and (min-width: 540px) {
                    width: 50%;
                }

                @media screen and (min-width: 768px) {
                    width: 75%;
                }

                @media screen and (min-width: 1475px) {
                    width: 50%;
                }

                @media screen and (min-width: 2000px) {
                    width: 40%;
                }
            }
        }
    }

}</style>