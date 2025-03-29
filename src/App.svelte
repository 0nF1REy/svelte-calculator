<script lang="ts">
  import Calculadora from "./components/Calculadora.svelte";

  let numeroMagico = 13
</script>

<main>
	{#if numeroMagico === 13}
		<Calculadora />
	{:else}
		<h1>Falso</h1>
	{/if}
</main>

<style>
  :global(body) {
    background-color: #222;
    color: #fff;
    font-family: sans-serif;
  }

  :root {
    --cor-fundo: #333;
    --cor-botao: #444;
    --cor-botao-hover: #555;
    --cor-operacao: #f90;
    --cor-destaque: #d33;
    --cor-tela: #eee;
    --cor-texto-tela: #222;
  }

  main {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
</style>
