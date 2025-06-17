<script lang="ts">
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  import { Sky, Stars,OrbitControls   } from '@threlte/extras'
  

  useTask((delta) => {
  })
</script>

<Sky elevation={-5} turbidity={20} />


<T.PerspectiveCamera
  makeDefault
  position={[10, 5, 10]}
  lookAt.y={0.5}
>
  <OrbitControls />
</T.PerspectiveCamera>


<T.DirectionalLight
  position={[0, 10, 10]}
  castShadow
/>

<City/>