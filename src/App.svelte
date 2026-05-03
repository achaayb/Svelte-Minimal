<script>
    let count = $state(0);
</script>

<main class="page">
    <section class="section">
        <h1>Svelte + Vite</h1>

        <p class="meta">Minimal Svelte Project</p>

        <button onclick={() => count++}>
            count is {count}
        </button>
    </section>
</main>

<style>
    :global(body) {
        margin: 0;
        background: #f4f1ea;
        font-family: "Times New Roman", Times, serif;
        color: #1a1a1a;
    }

    .page {
        height: 100vh;
        display: grid;
        place-items: center;
    }

    .section {
        width: min(600px, 90vw);
        padding: 48px 56px;
        border: 1px solid #222;
        background: #fffdf7;
        text-align: center;
        box-shadow: 6px 6px 0 #000;
    }

    h1 {
        font-size: 28px;
        letter-spacing: 2px;
        margin-bottom: 12px;
        text-transform: uppercase;
    }

    .meta {
        font-size: 12px;
        letter-spacing: 1px;
        margin-bottom: 32px;
        opacity: 0.7;
    }

    button {
        font-family: inherit;
        font-size: 14px;
        padding: 10px 16px;
        border: 1px solid #000;
        background: transparent;
        cursor: pointer;
        letter-spacing: 1px;
        text-transform: uppercase;
    }

    button:hover {
        background: #000;
        color: #fff;
    }
</style>
