<template>
  <div>
    <HelloWorld title="slot">
      <p>これは親のテンプレートのslotです。</p>
    </HelloWorld>
    <hr>
    <HelloWorld2>
      <template v-slot:slot1>
        <div>
          slot1です。
        </div>
      </template>
      <template v-slot:slot2>
        <div>
          slot2です。
        </div>
      </template>
      <template v-slot:slot3>
        <div>
          slot3です。
        </div>
      </template>
    </HelloWorld2>
    <hr>
    <HelloWorld3>
      <template #slot1>
        <div>
          slot1です。
        </div>
      </template>
      <template #slot2>
        <div>
          slot2です。
        </div>
      </template>
      <template #slot3>
        <div>
          slot3です。
        </div>
      </template>
    </HelloWorld3>

  </div>
</template>

<script>
import HelloWorld1 from './components/HelloWorld1.vue'
import HelloWorld2 from './components/HelloWorld2.vue'
import HelloWorld3 from './components/HelloWorld3.vue'

export default {
  name: 'App',
  components: {
    HelloWorld1,
    HelloWorld2,
    HelloWorld3
  }
}
</script>
