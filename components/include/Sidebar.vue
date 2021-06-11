<template>
  <div>
    <div>
      <b-button v-b-toggle.sidebar-1>Toggle Sidebar</b-button>
      <b-sidebar id="sidebar-1" title="Sidebar" shadow>
        <div class="px-3 py-2">
          <p>
            Cras mattis consectetur purus sit amet fermentum. Cras justo odio,
            dapibus ac facilisis in, egestas eget quam. Morbi leo risus, porta
            ac consectetur ac, vestibulum at eros.
          </p>
          <b-img
            src="https://picsum.photos/500/500/?image=54"
            fluid
            thumbnail
          ></b-img>
        </div>
      </b-sidebar>
      <b-button v-b-toggle.sidebar-right>Toggle Sidebar</b-button>
      <b-sidebar id="sidebar-right" title="Sidebar" right shadow>
        <div class="px-3 py-2">
          <p>
            Cras mattis consectetur purus sit amet fermentum. Cras justo odio,
            dapibus ac facilisis in, egestas eget quam. Morbi leo risus, porta
            ac consectetur ac, vestibulum at eros.
          </p>
          <b-img
            src="https://picsum.photos/500/500/?image=54"
            fluid
            thumbnail
          ></b-img>
        </div>
      </b-sidebar>
    </div>
    <br>
    <div>
      <b-button v-b-toggle.sidebar-backdrop>Toggle Sidebar</b-button>

      <b-sidebar
        id="sidebar-backdrop"
        title="Sidebar with backdrop"
        :backdrop-variant="variant"
        backdrop
        shadow
      >
        <div class="px-3 py-2">
          <b-form-group label="Backdrop variant" label-for="backdrop-variant">
            <b-form-select
              id="backdrop-variant"
              v-model="variant"
              :options="variants"
            ></b-form-select>
          </b-form-group>
        </div>
      </b-sidebar>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      variant: 'dark',
      variants: [
        'transparent',
        'white',
        'light',
        'dark',
        'primary',
        'secondary',
        'success',
        'danger',
        'warning',
        'info',
      ],
    }
  },
}
</script>
