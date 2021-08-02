<template>
  <div>
    <button @click="success">
      Successful Transaction
    </button>
    <button @click="fail">
      Failed Transaction
    </button>
  </div>
</template>

<script>
export default {
  methods: {
    success () {
      this.$swal('Success!', 'Transaction was successful', 'success')
    },
    fail () {
      this.$swal('Error!', 'Transaction was not successful', 'error')
    }
  }
}
</script>
