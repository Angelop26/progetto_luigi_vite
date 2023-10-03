<script>
    export default{
        name: 'MainTestimonianza',
        data(){
            return{
                intervall:null,
                indexTestimonianza: 0,
                testimonianze:[
                    {
                        name:'Kenia Arjona Dorado',
                        date:'01/2023',
                        comment:'Rocío es una estupenda preparadora, tiene muy buenos materiales, esquemas, te mantiene siempre actualizado, te motiva y apoya desde el principio hasta el final. No le importa explicarte 15 veces algo si lo necesitas. Había estudiado algunos meses por libre, pero estos 7 meses con ella me han ayudado mucho a lograr la plaza. La recomiendo mucho.'
                    },
                    {
                        name:'Sandra Castanedo Fernández',
                        date:'01/2023',
                        comment:'Estoy súper contenta con ellos. Rocío explica muy bien y de forma clara. Los temas súper completos (de los más completos que he visto en varios años), así como sus esquemas. Me he preparado la última convocatoria con Rocío y la verdad que no puedo estar más satisfecha. Además las clases las puedes ver en diferido por si no puedes verla en directo, cosa que facilita mucho el estudio también. En general su preparación es muy completa: temas, esquemas, clases, supuestos prácticos y web para hacer test.'
                    },
                    {
                        name:'Soraya Alcázar',
                        date:'04/2022',
                        comment:'Solo tengo buenas palabras para ellas. Empecé con Rocío estudiando para auxiliar administrativo de la junta y en menos de un año, aprobada!! Aun no me lo creo. Luego continúe estudiando administrativo para la AGE con María e igualmente aprobada!! Ambas son lo más, super atentas, los esquemas, los vídeos y la forma de explicar es magnífica. Estoy muy contentas con ellas, y seguiré con ellas hasta sacarme mi plaza🤞 las recomiendo porque a parte de ser un encanto, explican y reexplican hasta que se te queda grabado a fuego. Además, hacen mucho incapie en lo importante, y eso es algo que no muchas academias lo hacen de cara al examen. RECOMIENDO 100%'
                    }
                ],
            }
        },
        mounted(){
            this.autoScroll()
        },
        methods:{
            showNext(){
                this.blockAutoScroll()
                if(this.indexTestimonianza < this.testimonianze.length - 1){
                    this.indexTestimonianza++
                } else{
                    this.indexTestimonianza = 0
                }
                this.autoScroll()
            },
            showPrev(){
                this.blockAutoScroll()
                if(this.indexTestimonianza > 0){
                    this.indexTestimonianza--
                }else{
                    this.indexTestimonianza = this.testimonianze.length - 1
                }
                this.autoScroll()
            },
            autoScroll(){
                this.interval = setInterval(this.showNext, 15000)
            },
            blockAutoScroll(){
                clearInterval(this.interval)
            },          
        }
    }
</script>

<template>
   <section id="testimonials">
        <h2 class="text-center pt-3 mb-3">Ecco cosa ne pensano i nostri alunni</h2>
        <div class="carousel">
            <div class="carousel-inner mx-auto">
                <div class="carousel-item active" :class="{'active': indexTestimonianza}">
                    <p class="fs-6"> {{testimonianze[indexTestimonianza].comment}} </p>
                    <div class="ms_credit">
                        <p class="fs-6"> {{ testimonianze[indexTestimonianza].date }} </p>
                        <p class="fw-bold fs-6"> {{testimonianze[indexTestimonianza].name}} </p>
                    </div>
                </div>
            </div>
            <div class="prev" @click="showPrev()">
              <i class="fa-regular fa-circle-left fa-beat fa-lg"></i>
            </div>
            <div class="next" @click="showNext()">
              <i class="fa-regular fa-circle-right fa-beat fa-lg"></i>
            </div>
        </div>
    </section> 
</template>

<style lang="scss" scoped>
@use '../style/variables/mixins' as *;
.carousel-inner{
    width: 50%;
    height: 350px;
    @include flex(row,normal,center);
    .ms_credit{
        @include flex(row,space-between,center);
    }
}

.prev,
.next{
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;
}

.prev{
    left: 20%;
}
.next{
    right: 20%;
}
</style>