<script lang="ts">
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  import { Sky, Stars,OrbitControls   } from '@threlte/extras'
  

  useTask((delta) => {
  })
</script>

<Sky elevation={-2} />


<T.PerspectiveCamera
  makeDefault
  fov={50}
>
  <OrbitControls enableDamping />
</T.PerspectiveCamera>
<T.DirectionalLight
  position={[0, 10, 10]}
  castShadow
/>

<City/>