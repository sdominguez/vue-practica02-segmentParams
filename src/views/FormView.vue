<!-- En esta practica enviaremos 3 parametros -->

<template>
    <v-container>
        <v-row align-content="center" justify="center">
            <v-col cols="12">
                <v-text-field v-model="nombre" label="Ingresa tu nombre"></v-text-field>
            </v-col>

            <v-col cols="12">
                <v-text-field v-model="correo" label="Ingresa tu correo"></v-text-field>
            </v-col>

            <v-col cols="12">
                <v-text-field v-model="password" label="Ingresa tu password"></v-text-field>
            </v-col>

            <v-col cols="12">
                <v-btn :to="{
                    name: 'recibeparametro',
                    params: {
                        nombre,
                        correo,
                        password
                    }
                }" color="primary">
                    Ir a la vista paso de parametros en ruta
                </v-btn>
            </v-col>
            <!--
            <v-col cols="12">
                {{ nombre }}
            </v-col>
            <v-col cols="12">
                {{ correo }}
            </v-col>
            <v-col cols="12">
                {{ password }}
            </v-col>
            -->
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: 'FormView',
    data() {
        return {
            nombre: '',
            correo: '',
            password: '',
        }
    },
}
</script>