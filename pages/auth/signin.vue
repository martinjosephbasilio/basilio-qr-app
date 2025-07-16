<template>
  <div class="d-flex align-center justify-center" style="height: 100vh">
    <v-card width="500">
      <h1 class="text-center my-6">Sign In</h1>
      <v-card-text>
        <v-form>
          <v-text-field outlined label="Email" prepend-inner-icon="mdi-email-outline"></v-text-field>
          <v-text-field outlined label="Password" type="password" prepend-inner-icon="mdi-lock-outline"></v-text-field>
          <v-card-actions>
            <v-btn class="mb-8" color="blue" variant="tonal" block>
              Log In
            </v-btn>
          </v-card-actions>
        </v-form>
        <div class="my-4 text-center">Or sign in with</div>
        <v-btn @click="signinWithGoogle()" class="mb-2" color="red darken-1" block>

          <v-icon left>mdi-google</v-icon>Google
        </v-btn>
      </v-card-text>

    </v-card>
  </div>
</template>

<script>
export default {
  layout: "auth",
  middleware: "guest",
  methods: {
    signinWithGoogle() {
      this.$auth.loginWith('google')
    }
  }
};

</script>
