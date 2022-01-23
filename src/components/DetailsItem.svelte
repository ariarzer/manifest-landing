<details>
    <slot></slot>
</details>

<style>
    details {
        width: 800px;
    }
    details :global(summary) {
        list-style: none;
        position: relative;
    }

    details :global(p) {
        font-size: 16px;
        line-height: 24px;
    }

    details :global(summary::after) {
        content: '';
        display: inline-block;
        position: absolute;
        top: 50%;
        right: 0;
        transition: transform 1s;
        height: 15px;
        width: 15px;
        border: 3px solid black;
        border-top: 0;
        border-left: 0;

        transform: rotate(-45deg);
    }

    details[open] :global(summary::after) {
        transform: rotate(45deg);
    }
</style>