<template>
    <div class="d-flex align-center justify-center" style="height: 100vh">
        <v-card width="500" >
            <h2 class="text-center my-6"> Sign In </h2>
            <v-card-text>
                <v-form>
                    <v-text-field 
                        outlined label = "Username"  type = "Username" prepend-inner-icon="mdi-email-outline"  >
                        
                        
                       
                    </v-text-field>
                    <v-text-field 
                        outlined label ="Password" type = "Password" prepend-inner-icon="mdi-lock-outline" ></v-text-field>
                       
                    
                </v-form>
            </v-card-text>
            <v-card-actions>
                <v-btn
        class="mb-8"
        color="blue"
        size="large"
        variant="tonal"
        block
      >
        Log In
      </v-btn>

            </v-card-actions>
        </v-card>
    </div>
</template>
<script>
export default{
    layout: "auth"
}
</script>