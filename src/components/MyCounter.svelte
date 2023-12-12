<script>
  export let componentTitle = '';
	let count = 0;

  function onClick() {
    count++;
  }
</script>

<div class="my-container">
  <h1>{componentTitle}</h1>
	<p>Вы нажали на кнопку {count} раз</p>
  <button on:click={onClick}>Нажми на меня</button>
</div>

<style>
	.my-container {
		border: 1px solid black;
    border-radius: 10px;
    padding: 10px;
	}

</style>
