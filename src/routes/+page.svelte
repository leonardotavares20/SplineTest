<script>
  import { Application } from "@splinetool/runtime";
  import { onMount } from "svelte";

  let canvas;
  onMount(() => {
    canvas = document.getElementById("canvas3d");
    const app = new Application(canvas);
    app.load("https://prod.spline.design/yBWnEoywvSzXwkna/scene.splinecode");
  });
</script>

<canvas id="canvas3d"></canvas>

<svelte:head>
  <script
    async
    src="https://unpkg.com/es-module-shims@1.6.3/dist/es-module-shims.js"
  ></script>
</svelte:head>
