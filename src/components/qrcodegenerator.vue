<script>
import QrcodeVue from 'qrcode.vue';

export default {
  components: {
    QrcodeVue,
  },
  data() {
    return {
      qrCodeData: '',
      size: 200,
    };
  },
};
</script>

<template>
  <div id="qrdiv">
    <input v-model="qrCodeData" placeholder="Enter link" />
    <qrcode-vue id="qrcode" :value="qrCodeData" :size="size" level="Q" />
  </div>
</template>

<style>
  #qrdiv {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1em;
  }
  input {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 20px;
    width: 20em;
    text-align: center;
  }
  #qrcode {
    border: solid #fff 4px;
  }
</style>