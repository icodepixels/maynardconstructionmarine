<script setup>
defineProps({
    msg: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <div class="footer">
        <div class="catch-container">
            <h2 class="action-words" style="">WE PROUDLY SERVE THE ENTIRE GULF SHORES AREA AND NEARBY COMMUNITIES</h2>
            <div class="areas">
                <a href="tel:+12512842500" class="link">
                    <h2 class="blue text-sm phone"><span class="">Call Today</span> (251) 284-2500</h2>
                </a>
            </div>
            <img alt="Maynard Construction & Marine" class="jermey-maynard" src="/images/jeremy_maynard.jpg" width="150" />
            <address>
                Jeremy Maynard
                <br />
                <span>Custom & Refacing Cabinets / Marine Construction</span>
                <br />
                22710 Oak Meadow Dr. Foley, Al 36542
            </address>
        </div>
    </div>
</template>

<style scoped>
address {
    text-align: center;
}
.jermey-maynard {
    margin-bottom: 16px;
}
span {
    font-weight: 700;
}
h3 {
    font-weight: 700;
}
ul {
    margin-bottom: 16px;
}
.served {
    display: flex;
    flex-direction: column;
}
.areas {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: baseline;
    margin: 16px 0;
}
.action-words {
    font-weight: 900;
    font-style: normal;
    color: #555;
    font-size: 1.4rem;
    text-align: center;
}

.footer {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    border-top: 1px solid #eee;
    padding: 8px 16px 8px 16px;
    margin: 0 auto 32px auto;
}
.catch-container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-top: 32px;
    padding: 0 16px;
}
.logo {
    margin-top: 16px;
}
.phone {
    font-weight: bold;
}

@media (max-width: 767px) {
    .phone {
        font-size: 1.5rem;
    }
    .footer {
        flex-direction: column;
        padding: 16px 16px 8px 16px;
    }
    .footer *:not(:last-child) {
        margin-bottom: 16px;
    }
    .catch-container h3 {
        margin: 0px auto;
        font-size: 1rem;
    }
}
</style>
