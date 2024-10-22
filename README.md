*, *::after, *::before {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    line-height: 1;
    font-weight: 400;
    color: #333;
}


/*  */
.container {
    width: 960px;
    margin: 0 auto;
}

header, section {
    margin-bottom: 96px;
}

.features--grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 80px;
}
.header--grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
}
img {
    border-radius: 12px;
}

.btn:link, .btn:visited {
    background-color: #087f5b;
    text-decoration: none;
    color: #fff;
    text-transform: uppercase;
    font-weight: 500;

    display: inline-block;
    border-radius: 100px;
    transition: all .35s;
}

.btn--big {
    padding: 16px 32px;
    font-size: 18px;
}
.btn--small {
    font-size: 14px;
    padding: 8px 12px;
}
.btn:hover, .btn:active {
    background-color: #099268;
}
/* .btn:hover {
    transform: translateY(-5px);
    box-shadow: 4px 10px 40px rgba(0, 0, 0, .2);
}
.btn:active {
    transform: translateY(-2px);
    box-shadow: 2px 6px 40px rgba(0, 0, 0, .15);
} */

h2 {
    font-size: 36px;
    letter-spacing: -0.5px;
    margin-bottom: 48px;
}

/* ========================= */
/* HEADER STYLES */
/* ========================= */
header {
    column-gap: 80px;
    margin-top: 64px;
    align-items: center;
}

header img {
    width: 100%;
}
h1 {
    margin-bottom: 32px;
    font-size: 44px;
    line-height: 1.1;
}

.header-text {
    margin-bottom: 24px;
    font-size: 18px;
    line-height: 1.5;
}


/* ========================= */
/* FEATURE SECTION */
/* ========================= */
.features-icon {
    width: 32px;
    height: 32px;
    stroke: #087f5b;
    margin-bottom: 24px;
}

.features-title {
    margin-bottom: 16px;
    font-size: 20px;
    font-weight: 700;
}
.features-text {
    font-size: 17px;
    line-height: 1.6;
}



/* =========================== */
/* TESTIMONIAL SECTION */
/* =========================== */

.testimonial-section {
    background-color: #087f5b;
    color: #fff;
    padding: 24px;
    border-radius: 12px;
}
.testimonial-grid {
    display: grid;
    grid-template-columns: 1.4fr 3fr;
    gap: 80px;
    align-items: center;
}
.testimonial-section img {
    width: 100%;
}
.testimonial-text {
    display: flex;
    flex-direction: column;
    gap: 24px;
}
.testimonial-text h3 {
    font-size: 24px;
}
blockquote {
    font-style: italic;
    font-size: 18px;
    line-height: 1.5;
}
.testimonial-author {
    font-size: 14px;
    color: #e6fcf5;
}


/* ===================== */
/* BEST SELLING SECTION */
/* ===================== */

.chair-figure {
    border-radius: 12px;
    box-shadow: 0 20px 30px rgba(0, 0, 0, .07);
    overflow: hidden;
}
.chair-figure img {
    width: 100%;
    border-radius: 0;
}
.chair-box {
    padding: 32px;
}
.chair-figure h3 {
    margin-bottom: 24px;
    font-size: 20px;
}
.chair-details {
    list-style: none;
    margin-bottom: 48px;
    display: flex;
    flex-direction: column;
    gap: 16px;
}
.chair-details li {
    display: flex;
    gap: 12px;
    align-items: center;
}
.chair-icon {
    width: 24px;
    height: 24px;
    margin-bottom: 2px;
    stroke: #087f5b;
}

.chair-price {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 20px;
}


/* =============================== */
/* MEDIA QUERY */
/* =============================== */
@media screen and (max-width: 450px) {
    html {
        zoom: 90%;
    }
    body {
        font-size: 14px;
    }
    .container {
        padding: 0 32px;
        max-width: 100%; /* fluid */
    }
    .header--grid {
        grid-template-columns: 1fr;
        text-align: center;
        row-gap: 32px;
    }
    .header-image-box {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    header img {
        width: 100%;
    }

    .features--grid {
        grid-template-columns: 1fr;
    }

    .testimonial-grid {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    }

    .testimonial-grid img {
        width: 100%;
    }
}
