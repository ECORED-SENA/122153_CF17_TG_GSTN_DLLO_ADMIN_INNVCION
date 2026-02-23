<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-4 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:

    .row.justify-content-center
      .col-lg-11.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis-.svg", alt="A continuación, se presenta la síntesis del componente formativo: El diagnostico empresarial se basa en la empresa-organización teniendo un análisis de información donde se pueda innovar a través de descubrir, idear y realizar/implementar, de esta manera obteniendo un valor agregado.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
