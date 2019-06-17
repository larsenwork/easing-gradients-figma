<h1>Hej {name}!</h1>

<p>Count: <input type="number" bind:value={count}></p>
<button on:click={createRectangles}>Create</button>
<button on:click={cancel}>Cancel</button>

<style>
  h1 {
    color: blue;
  }
</style>

<script lang="ts">
  let count = 5
  export let name: string;

  type PluginMessage = {
    type: 'create-rectangles' | 'cancel'
    count?: number
  }

  function sendToFigma(message: PluginMessage) {
    parent.postMessage({ pluginMessage: message }, '*')
  }

  function createRectangles() {
		sendToFigma({ type: 'create-rectangles', count })
  }

	function cancel() {
    sendToFigma({ type: 'cancel' })
	}
</script>
