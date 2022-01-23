<article>
    <div role="presentation" class="image">
        <slot name="image"></slot>
    </div>
    <h2>
        <slot name="header"></slot>
    </h2>
    <slot></slot>
</article>

<style>
    .image {
        font-size: 100px;
    }

    article {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    h2 {
        font-size: 40px;
    }

    article :global(h3) {
        font-size: 30px;
    }

    article :global(> h3) {
        text-align: center;
    }

    article :global(> p) {
        font-size: 18px;
        text-align: center;
    }
</style>