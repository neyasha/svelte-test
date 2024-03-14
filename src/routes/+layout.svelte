<nav>
    <div class = "nav-container">
        <a href="/" class ="nav-logo" title="Back to Homepages">Настя Палагина</a>
        <div class="nav-links">
            {#each nav as link}
            <a href={link.href} class="link">{link.title}</a>
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <!--Pages will be injected below-->
    <slot></slot>
</div>
<script>
    const nav = [
        {
         title: "Обо мне",
         href: "/about"
        },
        {
         title: "Блог",
         href: "/blog",
        },
        {
         title: "Проект",
         href: "/project",
        },
        {
         title: "Контакты",
         href: "/contacts",
        },
        {
         title: "temp",
         href: "/temp"
        }
    ]
</script>
<style>
    .container{
        max-width: 1400px;
        margin: 50 px auto;
    }
</style>