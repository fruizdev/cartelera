<template>
  <div class="uk-card uk-card-default uk-grid-collapse uk-child-width-1-2@s uk-margin" uk-grid>
      <div class="uk-card-media-left uk-cover-container">
          <img :src="actividad.RutaImg" alt="" uk-cover>
          <canvas width="600" height="400"></canvas>
      </div>
      <div>
          <div class="uk-card-body">
              <h3 class="uk-card-title"> {{ actividad.actividad }}</h3>
              <p>{{ actividad.Fecha_ini }}</p>
              <p>{{ actividad.area }}</p>
              <p>{{ actividad.Descripcion }}</p>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'ActividadCard',
  props: {
    actividad: {
      type: Object,
      required: true
    }
  }
}
</script>