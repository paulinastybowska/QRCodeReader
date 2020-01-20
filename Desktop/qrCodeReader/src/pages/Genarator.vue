<template>
  <q-page class="container">
    <div class="row justify-center">
      <div class="col-12 q-pt-lg text-center text-blue-grey-9">
        <span class="text-subtitle1">
          Enter the String you want to insert into your custom QRCode.
        </span>
      </div>
      <div class="col-10 q-pt-lg">
        <q-input rounded outlined v-model="text" label="Value" />
      </div>
      <div class="col-12 q-pt-md text-center">
        <qriously :value="text" :size="230" />
      </div>
       <q-btn clickable to="/" exact class="q-mt-xl" style="background: #FF0080; color: white" size="xl" label="Read QR Code" />
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'Generator',
  data () {
    return {
      text: 'https://wzr.ug.edu.pl/glowna/'
    }
  }
}
</script>
