<template>
  <h1>Simple vite app</h1>
  <p>Demo is meant to test vite building of a speech tensorflow project</p>
</template>

<script setup>
  import { onMounted } from 'vue'
  import * as tf from "@tensorflow/tfjs"
	import * as speechCommands from "@tensorflow-models/speech-commands"

  onMounted(async () => {
    const recognizer = speechCommands.create('BROWSER_FFT', 'directional4w');
    await recognizer.ensureModelLoaded();
    recognizer.listen(({ scores }) => {
      console.log(scores);
    }, {
        includeSpectrogram: false,
        probabilityThreshold: 0.75,
        invokeCallbackOnNoiseAndUnknown: true,
        overlapFactor: 0.50 // probably want between 0.5 and 0.75. More info in README
    })
  })
</script>
