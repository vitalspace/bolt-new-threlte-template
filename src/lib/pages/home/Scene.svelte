<script lang="ts">
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  import { Sky, Stars  } from '@threlte/extras'
  

  useTask((delta) => {
  })
</script>

 <!-- <Sky elevation={-2} /> -->

<Stars/>

<T.PerspectiveCamera
  makeDefault
  position={[10, 10, 10]}
  oncreate={(ref) => {
    ref.lookAt(0, 1, 0)
  }}
/>

<T.DirectionalLight
  position={[0, 10, 10]}
  castShadow
/>

<City/>