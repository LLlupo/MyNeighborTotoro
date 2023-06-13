<div class="navig">
    {#each nav as link}
        <div class="navig-button-{link.title}"><a href={link.href}><img src={link.img} alt={link.alt} class="navig-button-img"/></a></div>
    {/each}
</div>
<script>
    const nav = [
        {
            title: 'plot',
            href: '/plot',
            img: 'src/img/plot.png',
            alt: 'Сюжет',
            
        },
        {
            title: 'characterlist',
            href: '/CharacterList',
            img: 'src/img/characters.png',
            alt: 'Персонажи',
            
        },
        {
            title: 'o',
            href: '/o',
            img: 'src/img/',
            alt: 'j',
            
        },
    ]
</script>
<style>
    .navig {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .navig div {
        border-radius: 10px;
        margin: 0 20px 3% 20px;
        height: fit-content;
        width: fit-content;
        box-shadow: 0 0 10px 5px #dfdfdf;
        transition: all ease-in 0.5s;
    }
    
    .navig-button-plot:hover {
        box-shadow: 0 0 10px 5px #ced2ff;
    }
    .navig-button-characterlist:hover {
        box-shadow: 0 0 10px 5px #c1f3ff;
    }
    .navig-button-o:hover {
        box-shadow: 0 0 10px 5px #e1ffcf;
    }
    .navig-button-img {
        max-height: 400px;
    }   
</style>