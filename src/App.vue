<template>
  <v-app>
    <v-card width="400" class="mx-auto mt-5">
      <v-card-title >
        <h1 class="display-1">Login</h1>
      </v-card-title>
        <v-card-text>
          <v-form>
            <v-text-field
              name="username"
              label="username"
              id="id"
              prepend-icon="mdi-account-circle"
          ></v-text-field>

          <v-text-field
            name="password"
            label="password"
            id="pass"
            :type="showPassword ? 'text': 'password'"
            prepend-icon="mdi-lock"
            :append-icon="showPassword ? 'mdi-eye': 'mdi-eye-off'"
            @click:append="showPassword = !showPassword"
          ></v-text-field>

          </v-form>
        </v-card-text>
        <v-card-actions>
          <v-btn color="success">Register</v-btn>
          <v-spacer></v-spacer>
          <v-btn color="info">Login</v-btn>
        </v-card-actions>
      
    </v-card>
    
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    //HelloWorld,
  },

  data: () => ({
    showPassword: false
  }),
};
</script>
