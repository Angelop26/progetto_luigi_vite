<script>
import MainChiSiamoVue from './MainChiSiamo.vue';
import MainJumbotron from './MainJumbotron.vue';
import MainProvaVue from './MainProva.vue';
import MainQAVue from './MainQA.vue';
import MainTestimonianza from './MainTestimonianza.vue';
import MainEmail from './MainEmail.vue';
import MainCorsi from './MainCorsi.vue';
export default {
    name: 'AppMain',
    components: {
        MainJumbotron,
        MainChiSiamoVue,
        MainProvaVue,
        MainTestimonianza,
        MainQAVue,
        MainEmail,
        MainCorsi
    }
}
</script>

<template>
    <main>
        <MainJumbotron />
        <MainCorsi />
        <MainChiSiamoVue />
        <MainProvaVue />
        <MainTestimonianza />
        <MainQAVue />
        <MainEmail />
        <div class="whatsapp-link">
            <a href="https://wa.me/34681942907"><i class="fa-brands fa-square-whatsapp" style="color: #00ff40;"></i></a>
        </div>
    </main>
</template>

<style lang="scss" scoped>
section {
    padding-bottom: 10px;
    padding-top: 70px;

    @media screen and (min-width: 750px) {
        padding-top: 100px;

    }
}

.whatsapp-link {
    position: fixed;
    bottom: 130px;
    right: 0;
    padding: 1%;
    i{
        font-size: 2em;
        @media screen and (min-width: 780px){
        font-size: 3em;
            
        }
    }
}
</style>