<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>
        <div class="ms_ft-top">
            <div class="container text-center text-white py-4">
                <div class="mx-auto">
                    <p>AROUND THE WEB</p>
                    <div class="d-flex justify-content-center align-items-center">
                        <a href="https://www.facebook.com/people/Opopreparadora/100063451699998/" class="ms_entity">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a href="https://www.instagram.com/opopreparadora/?hl=es" class="ms_entity">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="https://www.tiktok.com/@opopreparadora" class="ms_entity">
                            <i class="fa-brands fa-tiktok"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.ms_ft-top {
    background-color: black;

    .ms_entity {
        border: 1px solid white;
        width: 50px;
        height: 50px;
        padding: 10px;
        border-radius: 30px;
    }

}
</style>