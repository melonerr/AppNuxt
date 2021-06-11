<template>
    <div>
      <div>
        <b-button @click="makeToast()" class="mb-2">Default</b-button>
        <b-button variant="primary" @click="makeToast('primary')" class="mb-2">Primary</b-button>
        <b-button variant="secondary" @click="makeToast('secondary')" class="mb-2">Secondary</b-button>
        <b-button variant="danger" @click="makeToast('danger')" class="mb-2">Danger</b-button>
        <b-button variant="warning" @click="makeToast('warning')" class="mb-2">Warning</b-button>
        <b-button variant="success" @click="makeToast('success')" class="mb-2">Success</b-button>
        <b-button variant="info" @click="makeToast('info')" class="mb-2">Info</b-button>
      </div>
      <hr/>
      <br/>
      <div>
        <b-button @click="$bvToast.show('my-toast')">Show toast</b-button>
        <b-toast id="my-toast" variant="warning" solid>
          <template #toast-title>
            <div class="d-flex flex-grow-1 align-items-baseline">
              <b-img blank blank-color="#ff5555" class="mr-2" width="12" height="12"></b-img>
              <strong class="mr-auto">Notice!</strong>
              <small class="text-muted mr-2">3 seconds ago</small>
            </div>
          </template>
          This is the content of the toast.
          It is short and to the point.
        </b-toast>
      </div>
      <hr/>
      <br/>
    </div>
</template>

<script>
  export default {
    methods: {
      makeToast(variant = null) {
        this.$bvToast.toast('Toast body content', {
          title: `Variant ${variant || 'default'}`,
          variant: variant,
          solid: true
        })
      }
    }
  }
</script>