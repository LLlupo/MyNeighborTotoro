<div class="container">
    <a href="../" class="back-link"><img src="\src\img\back.png" alt="Назад" class="back"></a>
    <div class="content">
        <slot />
    </div>
</div>
<style>
    .back {
        max-height: 200px;
        max-width: 100%;
        margin: auto 10px;
    }
    .back-link {
        width: fit-content;
        height: fit-content;
        transition: all ease-in 0.5s;
    }
    .back-link:hover {
        box-shadow: 0 0 10px 5px #e4ffd4;
        border-radius: 50px;
    }
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: auto 20px;
    }
</style>