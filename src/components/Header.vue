<template>
    <header class="header">
        <div class="header-logo">
            <p>Gelato</p>
        </div>
        <ul class="header-menu">
            <li><a href="#">Home</a></li>
            <li><a href="#">Menu</a></li>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Pricing</a></li>
            <li><a href="#">Contact Us</a></li>
            <li><a href="#">Location</a></li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    .header{
        width: 100%;
        height: 8.5rem;
        background: var(--main-color);
        color: #fff;
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-size: 1.5rem;
        padding: 0 5rem;
    }

    .header-logo{
        font-size: 3.5rem;
        font-family: var(--logo-font);

    }

    .header-menu{
        width: 60%;
        list-style-type: none;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .header-menu li{
        cursor: pointer;
    }

    .header-menu li a{
        text-decoration: none;
        color: #fff;
    }

    .header-menu li:first-of-type{
        font-weight: bold;
    }

</style>