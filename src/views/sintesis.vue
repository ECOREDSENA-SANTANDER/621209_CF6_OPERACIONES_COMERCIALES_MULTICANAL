<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      p Atender al cliente en el #[em retail] es crucial para el éxito de cualquier negocio. La experiencia del cliente puede influir directamente en la fidelización y en la reputación de la empresa. Por lo anterior es fundamental implementar estrategias, que mejoren la satisfacción del cliente y que fomenten la lealtad y, en última instancia, aumenten el éxito de la organización.
      p.mb-5 A continuación, se presenta el diagrama que representa el resumen de las temáticas que están desarrolladas en el componente formativo:
  
      .row.justify-content-center
        .col-lg-12.mb-5
          figure
            img(src="@/assets/curso/sintesis.svg", alt="La sintesis organiza cinco componentes fundamentales: conceptos básicos del servicio al cliente, procesos de atención en el entorno comercial, técnicas de servicio orientadas a la comunicación y la interacción efectiva, protocolos institucionales relacionados con la atención y la cortesía, y mecanismos para evaluar la satisfacción del cliente mediante herramientas de seguimiento, gestión de PQRS y registro de información. Estos elementos se articulan para fortalecer la calidad del servicio y la experiencia del cliente en los establecimientos comerciales.")
        .col-auto
          a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
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
