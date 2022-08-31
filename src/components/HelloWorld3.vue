<template>
  <div>
    <div>
      名前付きスロット(v-slotを#で)
      <slot name="slot1"/>
      <slot name="slot2"/>
      <slot name="slot3"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld3',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>
