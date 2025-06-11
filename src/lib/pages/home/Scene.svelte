<script lang="ts">
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  import { Sky, Stars,OrbitControls   } from '@threlte/extras'
  

  useTask((delta) => {
  })
</script>

<Sky elevation={-2} />


<T.PerspectiveCamera
  position={[0, 0, 0]}
  fov={60}
>
  <OrbitControls
    enableDamping
    target={[0, 0, 0]}
  />
</T.PerspectiveCamera>

<T.DirectionalLight
  position={[0, 10, 10]}
  castShadow
/>

<City/>