<script>
export default {
    name: 'MainProva'
}
</script>

<template>
    <section id="prova">
        <video class="mx-auto d-block" controls>
            <source src="../assets/video/video_landing_page.mp4" type="video/mp4">
        </video>
    </section>
</template>

<style lang="scss" scoped>
    video{
        width: 60%;
        @media screen and (min-width: 992px) {
            width: 900px;
        }
    }
</style>