<template>
  <div class="main-container">
    <Stepper></Stepper>
  </div>
</template>

<script>
import Stepper from '@/components/Stepper'
import { mapGetters } from 'vuex'

export default {
  components: { Stepper },
  computed: {
    ...mapGetters('patients', ['currentPatient'])
  },
  created() {
    if (!this.currentPatient) {
      this.$router.push('/home')
    }
  }
}
</script>

<style scoped lang="scss"></style>
