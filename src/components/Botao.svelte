<script lang="ts">
  export let texto: string;
  export let triplo: boolean = false;
  export let duplo: boolean = false;
  export let operacao: boolean = false;
  export let destaque: boolean = false;
  export let onClick: (valor: string) => void = () => {};
</script>

<button
  class="botao"
  on:click={() => onClick(texto)}
  class:triplo
  class:duplo
  class:operacao
  class:destaque
>
  {texto}
</button>

<style>
  .botao {
    margin: 3px;
    border: none;
    border-radius: 8px;
    background-color: var(--cor-botao);
    color: #fff;
    font-size: 1.6em;
    flex-basis: 23%;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    transition: background-color 0.2s ease;
  }

  .botao:hover {
    background-color: var(--cor-botao-hover);
  }

  .triplo {
    flex-basis: 73%;
  }

  .duplo {
    flex-basis: 48%;
  }

  .operacao {
    background-color: var(--cor-operacao);
  }

  .destaque {
    background-color: var(--cor-destaque);
  }
</style>
