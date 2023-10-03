<script>
    export default{
        name: 'MainProva'
    }
</script>

<template>
    <section id="prova">
        <div class="card text-center mx-auto wdt-80">
            <div class="card-body text-white">
                <h5 class="card-title fs-1">La web que todo opositor necesita</h5>
                <div class="card-text text-start fs-3 d-flex flex-column mx-auto p-2">
                    Oposiciones disponibles en la Web:
                    <ul>
                        <li>Auxiliar Administrativo Junta de Andalucía.</li>
                        <li>Administrativo Junta de Andalucía.</li>
                        <li>LibreOffice</li>
                    </ul>
                    <p class="text-center fs-2">¡¡Pruébala GRATIS durante 2 días!!</p>
                    <a href="https://app.opopreparadora.com/login" class="btn fs-3">hacer test</a>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.card{
    background-color: black;
    .card-text{
        @media screen and (min-width: 992px) {
            width: 60%;
        }
        a{
            background-color: gold;
            color: white;
            &:hover{
                color: black;
            }
        }
    }
}
</style>