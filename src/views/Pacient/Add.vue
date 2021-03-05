<template>
    <div>
        <br>
        <br>
        <v-container  fill-height>
            <v-row>
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
            </v-row>
            <v-row>
                <v-form
                    ref="form"
                >
                    <v-text-field
                    v-model="name"
                    label="Name"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="email"
                    required
                    ></v-text-field>

                    <v-btn
                    :disabled="!valid"
                    color="success"
                    class="mr-4"
                    @click="validate"
                    >
                    Validate
                    </v-btn>

                    <v-btn
                    color="error"
                    class="mr-4"
                    @click="reset"
                    >
                    Reset Form
                    </v-btn>

                    <v-btn
                    color="warning"
                    @click="resetValidation"
                    >
                    Reset Validation
                    </v-btn>
                </v-form>
            </v-row>
        </v-container>
    </div>
</template>

<script>
  export default {
    data: () => ({
      valid: true,
      name: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => (v && v.length <= 10) || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+\..+/.test(v) || 'E-mail must be valid',
      ],
      select: null,
      items: [
        'Item 1',
        'Item 2',
        'Item 3',
        'Item 4',
      ],
      checkbox: false,
    }),

    methods: {
      validate () {
        this.$refs.form.validate()
      },
      reset () {
        this.$refs.form.reset()
      },
      resetValidation () {
        this.$refs.form.resetValidation()
      },
    },
  }
</script>