<template>
  <div>
    <div>
      単純なスロットで組み込み
      <slot />
      <slot>
        これは、slotで上書きされる
      </slot>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
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
