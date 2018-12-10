<template>
  <div id="app">
    <title-bar></title-bar>
    <quien-pago></quien-pago>
    <quienes-estan></quienes-estan>
  </div>
</template>

<script>
import TitleBar from './components/TitleBar'
import QuienPago from './components/QuienPago'
import QuienesEstan from './components/QuienesEstan'

export default {
  name: 'app',
  components:{
    TitleBar,
    QuienPago,
    QuienesEstan
  }
}
</script>

<style>
body, html{
  background-color: #273c75 !important;
  color: white !important;
  font-family: regulator-nova, sans-serif !important;
}
</style>
