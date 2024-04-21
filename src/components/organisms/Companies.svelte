<div class="text"><h2 >i have worked with a few brands</h2></div>
<div class="brand">
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
    <div class="brand-logo">
        <img src="/Logos/PhonePe-Logo.png" alt="brand1" />
    </div>
</div>

<style>
h2 {
    font-size: 2.5rem;

}

.text {
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
}

.brand {
    position: relative;
    left: 120%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 2rem;
    animation: marquee 30s linear infinite;
    transition-delay: 1s;
    margin-bottom: 6rem;
}

.brand:hover {
    animation-play-state: paused;

}

img {
    width: 200px;
}

@keyframes marquee {
    0% {
        left: 120%;
    }

    100% {
        left: -100%;
    }
}

@media screen and (max-width: 868px) {
    h2 {
        font-size: 1.3rem;
    }

    .text {
        justify-content: start;
        padding-left: 1.5rem;
        margin-bottom: -1.5rem;
    }

    .brand {
        gap: 1rem;
        animation: marquee 10s linear infinite;
        margin-bottom: 3rem;
    }

    img {
        width: 150px;
    }
}
</style>
