<script setup>
  import QRCodeGenerator from './components/qrcodegenerator.vue';
</script>

<script>
export default {
  components: {
    QRCodeGenerator,
  },
};
</script>

<template>
  <div>
    <h1>QR Code Generator</h1>
    <QRCodeGenerator />
  </div>
</template>