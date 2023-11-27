<script setup>
defineProps({
    msg: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <a href="tel:+12512842500" class="btn">Schedule an Estimate</a>
    <img alt="Maynard Construction & Marine" class="logo" src="../../src/assets/logo.svg" width="150" />
    <a href="tel:+12512842500" class="link">
        <h2 class="blue text-md phone"><span class="gray">Call Now</span> (251) 284-2500</h2>
    </a>
</template>

<style scoped>
h1 {
    font-weight: 500;
    position: relative;
}

.greetings {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #eee;
    border-left: 1px solid #eee;
    border-right: 1px solid #eee;
    padding: 8px 16px 8px 16px;
    margin: 0 auto;
}
.logo {
    margin-top: 4px;
    margin-bottom: 4px;
}
.phone {
    font-weight: bold;
}
.phone:hover {
    color: #c80163;
}

@media (max-width: 767px) {
    .logo {
        margin-top: 16px;
        margin-bottom: 16px;
    }
    .greetings {
        flex-direction: column;
        padding: 16px 16px 8px 16px;
    }
    .greetings *:not(:last-child) {
        margin-bottom: 16px;
    }
    .catch-container h3 {
        margin: 0px auto;
        font-size: 1rem;
    }
}
</style>
