<script lang="ts">
  import { T, useTask } from '@threlte/core'
  import City from "./components/world/City.svelte"
  import { Sky, Stars  } from '@threlte/extras'
  

  useTask((delta) => {
  })
</script>

<Sky elevation={-2} />


<T.PerspectiveCamera
  position={[0, 7, 18]}
  fov={60}
  near={1}
  far={20000}
  makeDefault
>
  <OrbitControls
    maxPolarAngle={85 * DEG2RAD}
    enableDamping
    target={[0, 2.5, 0]}
  />
</T.PerspectiveCamera>

<T.DirectionalLight
  position={[0, 10, 10]}
  castShadow
/>

<City/>