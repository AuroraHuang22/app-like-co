<template>
  <div
    :class="[
      'inline-block',
      'bg-shade-gray',
      'py-[6px]',
      'px-[20px]',
      'text-[12px]',
      'rounded-[16px]',
    ]"
  >
    {{ text }}
  </div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from 'vue-property-decorator'

@Component
export default class Tag extends Vue {
  @Prop(String) readonly text: String | undefined
}
</script>