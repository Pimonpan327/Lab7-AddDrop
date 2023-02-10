<template>
  <div>MAEJO UNIVERSITY</div>
  <br>
  <v-sheet width="300" class="mx-auto">
    <v-form fast-fail @submit.prevent>
      <v-text-field
        v-model="username"
        label="username"
        :rules="firstNameRules"
      ></v-text-field>

      <v-text-field
        v-model="password"
        label="password"
        :rules="lastNameRules"
      ></v-text-field>

      <v-btn type="submit" block class="mt-2">Submit</v-btn>
    </v-form>
  </v-sheet>
</template>

<script>
  export default {
    data: () => ({
      username: '',
      firstNameRules: [
        value => {
          if (value?.length > 3) return true

          return 'username must be at least 3 characters.'
        },
      ],
      lastName: '123',
      lastNameRules: [
        value => {
          if (/[^0-9]/.test(value)) return true

          return 'password can not contain digits.'
        },
      ],
    }),
  }
</script>