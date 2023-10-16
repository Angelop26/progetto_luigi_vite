<script>
export default {
    name: 'MainCorsi',
    data() {
        return {
            corsi: [
                {
                    name: 'JA C1, Administrativo de la Junta de Andalucía. ',
                    backgroundImg: 'corso_JA_C1.jpg',
                    option_1: {
                        title: "Opción 1: Clases grabadas por argumento + Seguimiento + Tutoría Online.",
                        text: "Este paquete integral está diseñado para brindarte una preparación completa y personalizada. Con este plan, tendrás acceso a:",
                        list: ["Clases grabadas por argumento: Hemos creado lecciones en video cuidadosamente estructuradas para cada tema.. Puedes ver estas clases cuantas veces quieras, para asegurarte de entender a fondo cada concepto.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "75€/mes"
                    },
                    option_2: {
                        title: "Opción 2: Seguimiento.",
                        list: ["Si prefieres un enfoque más independiente, con la opción de seguimiento tendrás las respuestas a todas las preguntas que te surjan durante el estudio y orientación sobre cómo organizar tu estudio.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "55€/mes"
                    }
                },
                {
                    name: 'JA C2',
                    backgroundImg: 'corso_JA_C2.jpg',
                    option_1: {
                        title: "Opción 1: Clases grabadas por argumento + Seguimiento + Tutoría Online.",
                        text: "Este paquete integral está diseñado para brindarte una preparación completa y personalizada. Con este plan, tendrás acceso a:",
                        list: ["Clases grabadas por argumento: Hemos creado lecciones en video cuidadosamente estructuradas para cada tema.. Puedes ver estas clases cuantas veces quieras, para asegurarte de entender a fondo cada concepto.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "75€/mes"
                    },
                    option_2: {
                        title: "Opción 2: Seguimiento.",
                        list: ["Si prefieres un enfoque más independiente, con la opción de seguimiento tendrás las respuestas a todas las preguntas que te surjan durante el estudio y orientación sobre cómo organizar tu estudio.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "55€/mes"
                    }
                },
                {
                    name: 'LO',
                    backgroundImg: 'corso_LO.jpg',
                    option_1: {
                        title: "Opción 1: Clases grabadas por argumento + Seguimiento + Tutoría Online.",
                        text: "Este paquete integral está diseñado para brindarte una preparación completa y personalizada. Con este plan, tendrás acceso a:",
                        list: ["Clases grabadas por argumento: Hemos creado lecciones en video cuidadosamente estructuradas para cada tema.. Puedes ver estas clases cuantas veces quieras, para asegurarte de entender a fondo cada concepto.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "75€/mes"
                    },
                    option_2: {
                        title: "Opción 2: Seguimiento.",
                        list: ["Si prefieres un enfoque más independiente, con la opción de seguimiento tendrás las respuestas a todas las preguntas que te surjan durante el estudio y orientación sobre cómo organizar tu estudio.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "55€/mes"
                    }
                },
                {
                    name: 'AGE C1',
                    backgroundImg: 'corso_Age_C1.jpg',
                    option_1: {
                        title: "Opción 1: Clases grabadas por argumento + Seguimiento + Tutoría Online.",
                        text: "Este paquete integral está diseñado para brindarte una preparación completa y personalizada. Con este plan, tendrás acceso a:",
                        list: ["Clases grabadas por argumento: Hemos creado lecciones en video cuidadosamente estructuradas para cada tema.. Puedes ver estas clases cuantas veces quieras, para asegurarte de entender a fondo cada concepto.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "75€/mes"
                    },
                    option_2: {
                        title: "Opción 2: Seguimiento.",
                        list: ["Si prefieres un enfoque más independiente, con la opción de seguimiento tendrás las respuestas a todas las preguntas que te surjan durante el estudio y orientación sobre cómo organizar tu estudio.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "55€/mes"
                    }
                },
                {
                    name: 'AGE C2',
                    backgroundImg: 'corso_Age_C2.jpg',
                    option_1: {
                        title: "Opción 1: Clases grabadas por argumento + Seguimiento + Tutoría Online.",
                        text: "Este paquete integral está diseñado para brindarte una preparación completa y personalizada. Con este plan, tendrás acceso a:",
                        list: ["Clases grabadas por argumento: Hemos creado lecciones en video cuidadosamente estructuradas para cada tema.. Puedes ver estas clases cuantas veces quieras, para asegurarte de entender a fondo cada concepto.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Seguimiento individualizado: Estamos a tu disposición para aclarar tus dudas y proporcionar orientación personalizada. Te ayudaremos a establecer un plan de estudio efectivo y te guiaremos en tu progreso, asegurándonos que estés listo para afrontar el examen con confianza.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "75€/mes"
                    },
                    option_2: {
                        title: "Opción 2: Seguimiento.",
                        list: ["Si prefieres un enfoque más independiente, con la opción de seguimiento tendrás las respuestas a todas las preguntas que te surjan durante el estudio y orientación sobre cómo organizar tu estudio.", "Temario y esquemas de cada tema: los cuales se facilitarán semanalmente en base a la programación de estudio.", "Web: para realizar los test de todo el temario.", "Actualizaciones: del temario y sobre la oposición."],
                        price: "55€/mes"
                    }
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
            <p class="text-center">¡Bienvenido al emocionante viaje hacia tu futuro como funcionario/a con Opopreparadora!
                <br>
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
                                        <h1 class="modal-title fs-5" id="exampleModalLabel">{{ corso.name }}</h1>
                                        <button type="button" class="btn-close" data-bs-dismiss="modal"
                                            aria-label="Close"></button>
                                    </div>
                                    <div class="modal-body px-5">
                                        <div>
                                            <h4>{{ corso.option_1.title }}</h4>
                                            <p>{{ corso.option_1.text }}</p>
                                            <ul class="option-list">
                                                <li v-for="item, index in corso.option_1.list" :key="index">{{ item }}</li>
                                            </ul>
                                            <div class="d-flex justify-content-end">
                                                <span class="price text-end badge text-bg-warning mb-5">{{ corso.option_1.price }}</span>
                                            </div>
                                        </div>
                                        <div>
                                            <h4>{{ corso.option_2.title }}</h4>
                                            <p>{{ corso.option_2.text }}</p>
                                            <ul class="option-list">
                                                <li v-for="item, index in corso.option_2.list" :key="index">{{ item }}</li>
                                            </ul>
                                            <div class="d-flex justify-content-end">
                                                <span class="price text-end badge text-bg-warning">{{ corso.option_2.price }}</span>
                                            </div>
                                        </div>
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
                <p class="text-center mt-5">Independientemente de la opción que elijas, en Opopreparadora estamos
                    comprometidos a proporcionarte los recursos
                    y el apoyo necesarios para alcanzar el éxito en tu oposición. <br> Únete a nosotros y comienza tu viaje
                    hacia la
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

    .modal-body {
        .option-list {
            list-style-type: disc;
        }
        .price{
            margin-right: 0%;
        }
    }

}</style>