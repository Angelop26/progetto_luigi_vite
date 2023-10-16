<script>
export default {
    name: 'MainProva',

    data() {
        return {
            list: [
                {
                    title: "Test ilimitados y personalizados:",
                    description: "Con este servicio puedes acceder a una amplia gama de preguntas tipo test que te ayudarán a familiarizarte con el contenido del temario y el formato de tu examen. Además, puedes crear tus propios simulacros personalizados para enfocarte en las áreas que más necesitas mejorar."
                },
                {
                    title: "Estadísticas Avanzadas: ",
                    description: "Este apartado te ayudará a medir tus logros a través de gráficos intuitivos que te enseñarán los resultados de los test por cada bloque, tema, ley y por respuesta dudosa.",
                },
                {
                    title: "Comparación con otros usuarios:",
                    description: "¿Quieres saber cómo te va en comparación con otros usuarios? Con esta estadística podrás medir tu progreso en comparación con el resto de opositores. Esto te proporcionará una perspectiva valiosa sobre dónde te encuentras y te motivará a superarte constantemente.",
                },
                {
                    title: "Resultado obtenido: ",
                    description: "Después de cada test, recibirás la nota obtenida, calculada en función a las respuestas acertadas y a las erróneas, averiguando qué preguntas contestaste correctamente y en cuáles necesitas mejorar. ",
                },
                {
                    title: "Respuestas justificadas: ",
                    description: "Una vez terminado el test te facilitaremos la explicación detallada de las respuestas correctas conforme a lo que dicta la ley.",
                },
            ]
        }
    }
}
</script>

<template>
    <section id="prova">
        <h2 class="text-center">Acceso a nuestra Web de test para opositores.</h2>
        <p class="text-center">Si ya tienes un plan de estudio establecido y solo necesitas recursos extras para tu
            preparación, esta opción es perfecta para ti. Con este plan, tendrás:</p>
        <ul class="w-75 mx-auto">
            <li v-for="elem, index in list" :key="index" class="mb-2">
                <span>{{ elem.title }}</span>{{ elem.description }}
            </li>
        </ul>
        <div class="d-flex justify-content-end w-75 mx-auto mb-5">
            <span class="price text-end badge text-bg-warning">Precio &RightArrow; Mensual 5,50€ <br>
                Trimestral 13,50€ <br>
                Semestral 24€
            </span>
        </div>
        <video class="mx-auto d-block" controls>
            <source src="../assets/img/video_landing_page.mp4" type="video/mp4">
        </video>

    </section>
</template>

<style lang="scss" scoped>
ul {
    list-style-type: disc;

    span {
        font-weight: bold;
    }
}

video {
    width: 60%;

    @media screen and (min-width: 992px) {
        width: 900px;
    }
}</style>