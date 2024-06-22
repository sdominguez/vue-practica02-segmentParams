<template>
    <v-container>
        <v-row>
            <v-col>
                <v-card>
                    <v-card-title>
                        Nombre: {{ nombre }}
                    </v-card-title>
                    <v-card-title>
                        Correo: {{ correo }}
                    </v-card-title>
                    <v-card-title>
                        Contraseña: {{ password }}
                    </v-card-title>

                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    name: 'ResultView',
    props: {
        nombre: {
            type: String,
            required: true
        },
        correo: {
            type: String,
            required: true
        },
        password: {
            type: String,
            required: true
        },

    },
    data() {
        return {

        }
    },
}
</script>