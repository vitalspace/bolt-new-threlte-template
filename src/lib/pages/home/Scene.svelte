<script lang="ts">
  import { T, useTask } from "@threlte/core";
  import City from "./components/world/City.svelte";
  import { Sky, Stars, OrbitControls } from "@threlte/extras";

  useTask((delta) => {});
</script>

<<<<<<< HEAD
<Sky
  elevation={-5}
  turbidity={20}
  rayleigh={0.57}
  azimuth={180}
  mieCoefficient={0.038}
  mieDirectionalG={0}
  exposure={0.26}
/>
=======
<Sky elevation={-5} turbidity={20} />
>>>>>>> 929aa6818392ad65229343375bf994de655097d8

<T.PerspectiveCamera makeDefault position={[10, 5, 10]} lookAt.y={0.5}>
  <OrbitControls />
</T.PerspectiveCamera>

<T.DirectionalLight position={[0, 10, 10]} castShadow />

<City />
