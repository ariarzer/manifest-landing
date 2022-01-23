<li class="LabeledSlide">
    <div class="LabeledSlide__slide">
        <div class="LabeledSlide__topBadge Rounded">
            <slot name="topBadge"></slot>
        </div>
        <div class="LabeledSlide__bottomBadge Rounded">
            <slot name="bottomBadge"></slot>
        </div>
    </div>
    <div class="LabeledSlide__label">
        <span class=""></span>
        <slot name="label"></slot>
        <slot name="secondaryLabel"></slot>
    </div>
</li>

<style>

    .LabeledSlide {
        list-style: none;
        width: 170px;
        box-sizing: border-box;
        margin: 10px;
    }

    .LabeledSlide__label,
    .LabeledSlide__slide {
        padding: 10px;
    }

    .LabeledSlide__slide {
        background-color: #F2D76F;
        height: 190px;
        border-radius: 24px;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
    }

    .LabeledSlide__topBadge,
    .LabeledSlide__bottomBadge{
        --height: 30px;
        font-size: 14px;
        background-color: white;
        border-radius: 40px;
    }
</style>