<div class="content">
    <h1 class="main-title">Кадры из аниме</h1>
    <div class="picture-container">
        {#each pictures as page}
            <div class="picture">
                <img src="{page.image}" alt="" class="picture-image">
                <p>{page.title}</p>
            </div>
        {/each}
    </div>
</div>

<script>
    import {pictures} from './pictures';
</script>

<style>
    .content {
        margin: 50px auto;
        padding: 0 20px;
    }
    .main-title {
        text-align: center;
    }
    .picture-container {
        display: flex;
        flex-direction: row;
        gap: 20px;
        flex-wrap: wrap;
        justify-content: center;
    }
    .picture {
        display: flex;
        flex-direction: column;
    }
    .picture-image {
        max-height: 250px;
        width: 100%;
    }
    .picture p {
        color: gray;
        margin-left: 5px;
    }
</style>