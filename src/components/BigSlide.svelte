<li class="BigSlide">
    <slot></slot>
</li>

<style global>
    .BigSlide {
        list-style: none;
    }

    .BigSlide:nth-child(1){
        background-color: #FAF4D7;
    }
    .BigSlide:nth-child(2){
        background-color: #D7ECE4;
    }
    .BigSlide:nth-child(3){
        background-color: #CAD3EA;
    }

    .BigSlide {
        border-radius: 40px;
        padding: 20px;
        width: 250px;
        box-sizing: border-box;
    }

    .BigSlide :global(> h3) {
        margin-bottom: 10px;
        margin-top: 50px;
    }

    .BigSlide :global(> p) {
        font-size: 16px;
    }

    :global(.Slides--howToEarn),
    :global(.Slides--why) {
        counter-reset: step;
    }

    :global(.Slides--howToEarn .BigSlide::before) {
        content: "Шаг " counter(step);
        counter-increment: step;
        height: 40px;
        display: inline-block;
        font-size: 18px;
        padding: 10px 15px;
        background-color: black;
        color: white;
        box-sizing: border-box;
        border-radius: 20px;
    }

    :global(.Slides--why .BigSlide::before) {
        content: counter(step);
        counter-increment: step;
        height: 40px;
        display: inline-block;
        font-size: 18px;
        padding: 10px 15px;
        background-color: black;
        color: white;
        box-sizing: border-box;
        border-radius: 20px;
    }

    :global(.Slides--education .BigSlide) {
        height: 180px;
        width: 180px;
    }

    :global(.Slides--education .BigSlide:nth-child(n)) {
        background-color: #FAF4D7;
    }

    :global(.Slides--withUs .BigSlide) {
        color: white;
    }

    :global(.Slides--withUs .BigSlide:nth-child(1n)) {
        background-color: #0839E8;
    }
    :global(.Slides--withUs .BigSlide:nth-child(2n)) {
        background-color: #7A4991;
    }
    :global(.Slides--withUs .BigSlide:nth-child(3n)) {
        background-color: #CD4577;
    }


</style>