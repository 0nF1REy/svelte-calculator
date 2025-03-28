<script lang="ts">
  import Botao from "./Botao.svelte";

</script>

<div class="calculadora">
    <Botao texto="7"/>
    <Botao texto="8"/>
    <Botao texto="9"/>
</div>

<style>
    :global(body) {
        background-color: black;
    }
    :root {
        --cor-fundo: #555;
    }

    .calculadora {
        background-color: var(--cor-fundo);
        height: 220px;
        width: 150px;
        display: flex;
        flex-direction: column;
    }
</style>