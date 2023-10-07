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
        getImagePath(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section id="corsi">
        <div class="corso-container">
            <h2 class="corsi-title text-center fs-4 ">Nuestros cursos</h2>
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
            </div>
        </div>
        <div class="prerequisiti-container wdt-80 mx-auto">
            <h2 class="text-center">Prerequisiti</h2>
            <div class="accordion accordion-flush w-75 mx-auto" id="accordionFlushExample">
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                            data-bs-target="#flush-collapseOne" aria-expanded="false" aria-controls="flush-collapseOne">
                            prerequisiti 1
                        </button>
                    </h2>
                    <div id="flush-collapseOne" class="accordion-collapse collapse" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            <ol>
                                <li>
                                    ciao
                                </li>
                            </ol>
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                            data-bs-target="#flush-collapseTwo" aria-expanded="false" aria-controls="flush-collapseTwo">
                            Prerequisiti 2
                        </button>
                    </h2>
                    <div id="flush-collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionFlushExample">
                        <div class="accordion-body">
                            <ol>
                                <li>
                                    ciao
                                </li>
                            </ol>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables/mixins' as *;

.corso-container {
    padding: 100px 40px;
    position: relative;
    @include flex(row, space-around, center);

    .corsi-title {
        position: absolute;
        left: 50%;
        top: 3%;
        transform: translateX(-50%);
    }

    a {
        height: 100%;
        display: block;
        width: 100%;

        .badge {
            width: 100%;
            height: 250px;

            img{
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
            }
        }
    }

}
</style>