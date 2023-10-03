<script>
    export default{
        name: 'MainJumbotron'
    }
</script>

<template>
    <section>
        <div class="ms_jumbo">
            <div class="ms_jumbo-container mx-auto">
                <div class="ms_promo">
                    <p>Oposita con nosotros</p>
                    <h1>Ve a por tu plaza</h1>
                </div>
                <div class="ms_jumbo-logo d-flex">
                    <img src="../assets/img/opopreparadora_full_logo.jpg" alt="logo">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables/mixins' as *;
.ms_jumbo{
    background-image: url('../assets/img/top-view-young-redhead-male-student-preparing-university-exam_171337-10015.avif');
    background-size: cover;

    .ms_jumbo-container{
        @include flex(row,center,center);
        width: 80%;
        padding: 30px 0;
        .ms_promo{
            color: white;
            font-size: 1.5rem;
            margin-right: 2rem;
            p{
                font-weight: bolder;
                font-size: 1.4rem;
            }
            h1{
                font-size: 5rem;
            }
        }
    }
}
</style>