<template>
    <header class="main-head">
        <nav>
            <h1 id="logo">Arni Verwasa</h1>
            <ul>
                <li><NavLink title="Home" scrollSelector="#welcome-section" /></li>
                <li><NavLink title="Credentials" scrollSelector="#credentials-section" /></li>
                <li><NavLink title="Skills" scrollSelector="#skills-section"/></li>
                <li><NavLink title="Projects" scrollSelector="#projects-section"/></li>
                <li><NavLink title="Contacts" scrollSelector="#contact-section"/></li>
            </ul>
        </nav>
    </header>

</template>

<script>
import NavLink from './sub-components/NavLink'
export default {
    name: 'Header',
    components: {
        NavLink
    }
}
</script>


<style scoped>
.main-head{
    background-color: #B39BC8;
    color: white;
    /* sticky */
    overflow: hidden;
    position: fixed;
    top: 0;
    width: 100%;
}

nav {
    display: flex;
    width: 90%;
    margin: auto;
    padding: 2rem;
    min-height: 10vh;
    align-items: center;
    flex-wrap: wrap;
    
}

nav ul {
    display: flex;
    flex: 1 1 20rem;
    justify-content: space-around;
    align-items: center;
    list-style: none;

}

#logo {
    flex: 1 1 40rem;
}

@media screen and (max-width: 1155px) {
    #logo {
        display: none;
    }
    nav {
        padding: 0;
        margin: 0;
        width: 100%;
    }
}



</style>