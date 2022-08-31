<template>
  <div>
    <div>
      名前付きスロット
      <slot name="slot1"/>
      <slot name="slot2"/>
      <slot name="slot3"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld2',
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
