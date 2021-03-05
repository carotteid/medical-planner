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
                href="/pacients"
                >
                <v-icon
                dark
                left
                >
                mdi-arrow-left
                </v-icon>
                Return to Pacients
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
                    v-model="name"
                    label="Nombre"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="ap_p"
                    label="Apellido paterno"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="ap_m"
                    label="Apellido materno"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="dir"
                    label="Dirección"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="tel"
                    label="Teléfono"
                    required
                    ></v-text-field>
                    
                    <v-text-field
                    v-model="nac"
                    label="Fecha de nacimiento (dd/mm/aaaa)"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="sexo"
                    label="Sexo"
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