<template>
  <div>
    <v-expansion-panels v-model="panel" multiple>
      <v-expansion-panel
        title="Foo"
        text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
        value="foo"
      ></v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<script>

import { onMounted, onUnmounted } from 'vue'

export default {
    data () {
      return {
        panel: [],
      }
    },
    methods: {
      all () {
        this.panel = ['foo', 'bar', 'baz']
      },
      none () {
        this.panel = []
      },
    },
  }


  setup (props){
    const handleClick = () => {
  console.log('Clicou no botão!')
}

onMounted(() => {
  const showMore = document.querySelector('#show-more')
  showMore.addEventListener('click', handleClick)
})

onUnmounted(() => {
  const showMore = document.querySelector('#show-more')
  showMore.removeEventListener('click', handleClick)
})

  return handleClick
  }
</script>
