<script>
    export let titleName;
</script>

<div class="section-title">
    <div class="title-dash">

    </div>
    <h2>{titleName}</h2>
</div>

<style>
    .section-title {
        display: flex;
        justify-content: flex-start;
        flex-direction: column;
    }

    .title-dash {
        width: 1.5rem;
        height: 0.125rem;
        background-color: hsl(0, 0%, 0%);
    }

    @media only screen and (min-width: 1440px) {
        h2 {
            font-size: 2rem;
        }

        .title-dash {
            height: 0.25rem;
        }
    }
</style>