<template>
    <div>
        <br>
        <v-container  fill-height>
            <v-row>
                <v-container>
                <v-btn
                tile
                dark
                color="orange darken-2"
                href="/appointments"
                >
                <v-icon
                dark
                left
                >
                mdi-arrow-left
                </v-icon>
                Return to Appointments
                </v-btn>
                </v-container>
            </v-row>
            <v-row>
                <v-container>
                <v-form
                    ref="form"
                >
                <v-container>
                    <v-text-field
                    v-model="date"
                    label="Fecha (dd/mm/aaaa)"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="diagnostic"
                    label="Diagnostico"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="treatment"
                    label="Tratamiento"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="weight"
                    label="Peso"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="height"
                    label="Altura"
                    required
                    ></v-text-field>
                    
                    <!--TODO: dropdown todos los pacientes-->
                    <v-text-field
                    v-model="pacient"
                    label="Paciente"
                    required
                    ></v-text-field>
                    </v-container>

                    <v-container>
                    <v-btn
                    class="ma-2"
                    color="green"
                    dark
                    >
                    Registrar
                    </v-btn>
                    </v-container>
                </v-form>
                </v-container>
            </v-row>
        </v-container>
    </div>
</template>

<script>
  export default {
    data: () => ({
      
    }),

    methods: {
      
    },
  }
</script>