<div class="container">
    <a href="/" class="back-link"><img src="\src\img\back.png" alt="Назад" class="back"></a>
    <div class="content">
        <slot />
    </div>
</div>
<style>
    .back {
        max-width: 200px;
        margin: auto 10px;
    }
    .back-link {
        width: fit-content;
        height: fit-content;
    }
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: auto 20px;
    }
</style>