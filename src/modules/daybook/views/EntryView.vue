<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
      <span class="text-success fs-3 fw-bold">15</span>
      <span class="mx-1 fs-3 fw-bold">Julio</span>
      <span class="mx-2 fs-4 fw-light">2021</span>
    </div>
    <div>
      <button class="btn btn-danger">
        Subir foto
        <i class="fa fa-upload"></i>
      </button>
      <button class="btn btn-primary mx-2">
        Borrar
        <i class="fa fa-trash-alt"></i>
      </button>
    </div>
  </div>
  <hr />
  <div class="d-flex flex-column px-3 h-75">
    <textarea name="" placeholder="¿Qué ha pasado hoy?"></textarea>
  </div>

  <Fab icon="fa-save" />

  <img
    class="img-thumbnail"
    alt="entry-picture"
    src="https://www.xtrafondos.com/wallpapers/resized/paisaje-digital-en-atardecer-5846.jpg?s=large"
  />
</template>

<script>
import { defineAsyncComponent } from "@vue/runtime-core";
export default {
  components: {
    Fab: defineAsyncComponent(() => import("../components/Fab.vue")),
  },
};
</script>

<style lang="scss" scoped>
textarea {
  font-size: 20px;
  border: none;
  height: 100%;

  &:focus {
    outline: none;
  }
}

img {
  width: 200px;
  position: fixed;
  bottom: 150px;
  right: 20px;
  box-shadow: 0px 5px 10px rgba($color: black, $alpha: 1);
}
</style>
