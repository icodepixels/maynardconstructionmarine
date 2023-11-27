<script setup>
import HeaderLinks from "./components/HeaderLinks.vue";
import TheWelcome from "./components/TheWelcome.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
    <main class="main">
        <header>
            <HeaderLinks msg="Maynard Construction & Marine" />
        </header>
        <TheWelcome />
        <Footer />
    </main>
</template>

<style scoped>
header {
    background-color: #f5f4f6;
    line-height: 1.5;
    width: 100%;
    border-radius: 8px;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    padding: 16px 32px;
    border-right: 1px solid #eee;
}

.logo {
    display: block;
    margin: 0 auto 2rem;
}

@media (max-width: 746px) {
    header {
        flex-direction: column;
    }
}
@media (min-width: 1024px) {
    .logo {
        margin: 0 2rem 0 0;
    }
}
</style>
