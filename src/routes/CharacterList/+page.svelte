<div class="content">
    <h1 class="main-title">Персонажи</h1>
    <div class="cards">
        {#each characters as page}
            <div class="card">
                <img src="{page.image}" alt="{page.title}" class="card-image">
                <h2 class="card-title">{page.title}</h2>
                <p>
                    {#if page.body}
                        {page.body}
                    {:else}
                        Описание к этому персонажу еще не было добавлено
                    {/if}
                </p>
                {#if page.readMore}
                    <p class="readmore">
                        <a class="link" href={`/CharacterList/characters/${page.id}`}>Подробнее</a>
                    </p>
                {/if}
            </div>
        {/each}
    </div>
</div>


<script>
    import {characters} from './characters';
</script>

<style>
    .content {
        margin: 50px auto;
        padding: 0 20px;
    }
    .main-title {
        text-align: center;
    }
    .cards {
        display: flex;
        flex-direction: row;
        gap: 20px;
        flex-wrap: wrap;
        justify-content: center;
    }
    .card {
        padding: 10px;
        max-width: 300px;   
        display: flex;
        flex-direction: column;
        border-radius: 10px;
        box-shadow: 0 0 10px 1px #888;
    }
    .link {
        color: rgb(10, 10, 139);
    }
    .link:hover {
        color: rgb(23, 23, 207);
    }
    .card-image {
        margin: 0 auto;
        max-width: 200px;
        border-radius: 10px;
    }
    .card-title {
        text-align: center;
        margin: 20px 0 0 0;
    }
   </style>