<script setup>
const imgs = Array.from({ length: 28 }, (_, i) => i + 1);
</script>

<template>
    <div class="container">
        <div class="content">
            <div class="catch-container"><h2 class="action-words" style="">GIVE YOUR HOME A CABINET MAKEOVER</h2></div>

            <div class="text-left">
                <section>
                    <p>
                        Why should you completely replace your entire cabinet for a new look when your existing cabinet boxes are still in good
                        condition? Simply put, you shouldn't. Sometimes the best and easiest way to give your cabinets an upgraded exterior is by
                        simply replacing the cabinet doors.
                    </p>

                    <p>
                        At Maynard Construction & Marine of Gulf Shores, we offer a wide variety of door faces, edge profiles, colors, and cabinet
                        hardware to make sure that you get the exact style you're wanting. Once your new doors are in place, we will then match the
                        cabinet boxes to the doors, completing the look of brand new cabinets at a fraction of the cost.
                    </p>

                    <p>
                        This service provides less hassle and cost than installing new cabinets, resulting in minimal family disruption and money left
                        over to update counter tops, back-splash or more. We want to give you the opportunity to bring your dream kitchen to life!
                    </p>

                    <div class="checks">
                        <div class="check-marks-container">
                            <div class="check-mark" />
                            Free, No-Obligation Price Estimates
                        </div>

                        <div class="check-marks-container">
                            <div class="check-mark" />
                            UV Lightspeed Instant Cabinet Curing
                        </div>

                        <div class="check-marks-container">
                            <div class="check-mark" />
                            Locally Owned and Operated
                        </div>
                    </div>
                </section>
            </div>
            <div class="banner-container">
                <div class="banner">
                    <h3 class="banner-img">Custom Wood Cabinets in Gulf Shores, AL</h3>
                </div>
            </div>

            <section class="second-section">
                <h3 class="" style="color: #212427; font-style: normal; font-weight: 700; margin-bottom: 16px">Custom Cabinets</h3>
                The kitchen is the heart of the home. Love is brewed here, and families gather to share meals and laughs. There is nothing more
                uncomfortable than a crowded kitchen. At Maynard Construction & Marine, we know how important a well functioning kitchen is to your
                family and how a perfectly executed kitchen design can make the entire home more comfortable and appealing. Maynard Construction &
                Marine is proud to offer custom-made cabinets in any design, size, and finish. From standard cabinetry to specially made cabinets that
                perfectly fit all of your custom kitchen needs.
            </section>
            <section class="second-section">
                <h3 class="" style="color: #212427; font-style: normal; font-weight: 700; margin-bottom: 16px">Cabinet Refacing</h3>
                Are you tired of looking at your outdated kitchen cabinets? It's time to breathe new life into your kitchen with professional cabinet
                refacing. Cabinet refacing is a cost-effective and efficient way to transform the look and feel of your kitchen without the hassle of
                a full renovation.
            </section>
        </div>
    </div>
    <div>
        <div class="cards">
            <div class="gray-box">
                <h4>INSPIRATION</h4>
                <p>Call today and get design inspiration and custom solutions to spice up your kitchen or bathroom.</p>
            </div>
            <div class="transparent-box inspiration-title">
                <img alt="Maynard Construction & Marine" class="category-img" :src="`/images/kitchen.png`" />
                <h4>KITCHEN REMODELING</h4>
            </div>
            <div class="transparent-box inspiration-title">
                <img alt="Maynard Construction & Marine" class="category-img inspiration-title-2" :src="`/images/bathroom.png`" />
                <h4>BATHROOM REMODELING</h4>
            </div>
            <div class="transparent-box inspiration-title">
                <img alt="Maynard Construction & Marine" class="category-img inspiration-title-3" :src="`/images/cabinet.png`" />
                <h4>CUSTOM CABINETS</h4>
            </div>
        </div>
    </div>
    <section class="images">
        <div class="grid-container">
            <div class="img-container grid-item" v-for="(i, index) in imgs" :key="index">
                <img alt="Maynard Construction & Marine" class="demos" :src="`/images/${i}.jpg`" />
            </div>
        </div>
    </section>
</template>

<style scoped>
.category-img {
    max-width: 140px;
    margin-bottom: 16px;
}
.images {
    margin-top: 64px;
    margin-bottom: 64px;
}
.grid-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-column-gap: 16px;
    grid-row-gap: 16px;
    max-width: 900px;
}
.banner-container {
    border-radius: 8px;
    overflow: hidden;
    margin-top: 16px;
    margin-bottom: 64px;
}
.checks {
    margin-top: 48px;
}
.check-mark {
    background-image: url("/images/checkmark.svg");
    background-repeat: no-repeat;
    background-size: cover;
    background-color: transparent;
    background-position: center;
    width: 20px;
    height: 20px;
    margin-right: 16px;
}
.check-marks-container {
    display: flex;
    align-items: center;
    font-weight: bold;
    margin-bottom: 16px;
}
.banner-img {
    color: #fff;
    background-image: radial-gradient(circle, rgba(0, 0, 0, 0.4) 33.3%, rgba(0, 0, 0, 0.1));
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8rem;
    letter-spacing: 1px;
    font-weight: 700;
}
section {
    max-width: 900px;
    width: 100%;
    margin: auto auto 64px auto;
}
.action-words {
    font-weight: 900;
    font-style: normal;
    color: #212427;
    font-size: 1.8rem;
    text-align: center;
    line-height: 1.4;
}
.catch-container {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 64px 0;
}
.cards {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    flex-wrap: wrap;
}
.gray-box {
    width: 258px;
    padding: 8px;
    color: rgb(90, 90, 90);
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #f8f8f8;
    height: 258px;
}

.transparent-box {
    width: 258px;
    padding: 8px;
    color: rgb(90, 90, 90);
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 258px;
    border-radius: 200px;
    overflow: hidden;
    background-color: #f8f8f8;
}
.transparent-box h4 {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    margin-bottom: 16px;
}
.gray-box h4 {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    margin-bottom: 16px;
}
.inspiration-title-2 {
    max-width: 96px;
}
.inspiration-title-3 {
    max-width: 118px;
}
.inspiration-title {
    display: flex;
    flex-direction: column;
    justify-content: baseline;
    margin-left: 16px;
}
.inspiration-title h4 {
    font-weight: 700;
}
.gray-box h4:after {
    width: 80px;
    height: 2px;
    content: "";
    display: block;
    background: #075d31;
    margin-top: 10px;
}
.check-marks {
    font-weight: 700;
    margin: 24px 0 8px 0;
}
.container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 0 16px;
}
.text-left {
    width: 100%;
    margin: auto;
}
.imgs-container {
    width: 100%;
    max-width: 900px;
    margin: auto;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    margin-top: 64px;
}
.img-container {
    width: 220px;
    height: 220px;
    overflow: hidden;
    display: flex;
}
.demos {
    width: 372px;
}
.banner {
    background-image: url("/images/403825338_1359148251375549_6698411373369828669_n.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-color: transparent;
    background-position: center;
    border: 1px solid #eee;
    height: 320px;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
}
@media (max-width: 1080px) {
    .gray-box {
        margin-bottom: 16px;
    }
    .cards {
        max-width: 600px;
        margin: auto;
    }
    .grid-container {
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(3, 1fr);
        padding-left: 16px;
    }
}
@media (max-width: 767px) {
  .banner-img {
    font-size: 1rem;
  }
    .grid-container {
        padding-left: 0;
    }
    .gray-box {
        margin-bottom: 16px;
    }
    .banner {
        width: 100%;
        margin-bottom: 16px;
    }
    .text-left p {
        font-size: 1.1rem;
    }
    .text-left h3 {
        font-size: 1.2rem;
    }
    .text-left {
        max-width: 100%;
        line-height: 1.4;
    }
    .container {
        flex-direction: column;
        padding: 0 16px;
    }
    .cards {
        max-width: 600px;
    }
}
</style>
