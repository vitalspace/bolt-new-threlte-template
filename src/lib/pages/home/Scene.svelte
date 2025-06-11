<script>
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  
  

  useTask((delta) => {
  })
</script>

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