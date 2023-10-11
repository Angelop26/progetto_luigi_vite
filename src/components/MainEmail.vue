<script>
export default {
    name: 'MainEmail',

    methods: {
        Email() {
            const email = document.modulo.email.value;
            const oggetto = document.modulo.oggetto.value;
            const messaggio = document.modulo.messaggio.value;
            if ((email.indexOf("@") == (-1)) || (email == "") || (email == "undefined")) {
                alert("Inserire un indirizzo email valido.");
                document.modulo.email.focus();
            }
            else if ((oggetto == "") || (oggetto == "undefined")) {
                alert("Inserire un oggetto.");
                document.modulo.oggetto.focus();
            }
            else if ((messaggio == "") || (messaggio == "undefined")) {
                alert("Inserire un messaggio.");
                document.modulo.messaggio.focus();
            }
            else {
                location.href = "mailto:" + email + "?Subject=" + oggetto + "&Body=" + messaggio;
            }
        }
    }
}
</script>

<template>
    <section id="mail">
        <div class="container text-center py-3">
            <h2 class="mb-3">Escríbenos si tienes más dudas</h2>
            <!-- <a href="mailto:info@opopreparadora.com" type="button" class="btn btn-primary fs-2">info@opopreparadora.com</a> -->
            <form name="modulo">
                Email:<br />
                <input type="text" name="email"> <br />
                Objeto:<br />
                <input type="text" name="oggetto"> <br />
                Mensaje:<br />
                <textarea name="messaggio" rows="10" cols="30"></textarea> <br />
                <input type="button" value="Envía" onClick="Email()">
            </form>
        </div>
    </section>
</template>

<style lang="scss" scoped></style>