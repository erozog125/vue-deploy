<script>
  export default {
    data: () => ({
      valid: true,
      checkbox: false,
    }),
  }
</script>

<template>
      <v-checkbox
        v-model="checkbox"
        :rules="[v => !!v || 'Para continuar debes aceptar']"
        label="He leído y acepto la Politica de privacidad y los terminos y condiciones"
        required
      ></v-checkbox>
      <v-btn type="submit" class="mt-2 sizebtn" color="SecondaryCyan">Enviar</v-btn>
</template>
<style>
  .sizebtn {
    width: 200px;
  }
</style>