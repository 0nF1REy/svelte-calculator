<script lang="ts">
    export let valor: string;

    $: tamanhoFonte = valor.length > 20 ? 'pequena' : `s-${valor.length}`
</script>

<div class={`tela ${tamanhoFonte}`}>
    <span>
        {valor}
    </span>
</div>

<style>
    .tela {
        display: flex;
        flex: 1;
        justify-content: flex-end;
        align-items: center;
        padding: 15px;
        font-size: 3.5rem;
        background-color: var(--cor-tela);
        color: var(--cor-texto-tela);
        overflow: hidden;
        margin: 5px;
        border-radius: 10px;
        box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.1);
    }

    .s-10 { font-size: 3rem; }
    .s-11 { font-size: 2.7rem; }
    .s-12 { font-size: 2.4rem; }
    .s-13 { font-size: 2.2rem; }
    .s-14 { font-size: 2rem; }
    .s-15 { font-size: 1.8rem; }
    .s-16 { font-size: 1.6rem; }
    .s-17 { font-size: 1.4rem; }
    .s-18 { font-size: 1.3rem; }
    .s-19 { font-size: 1.2rem; }
    .s-20 { font-size: 1.1rem; }

    .pequena { font-size: 1rem; }
</style>