<template>
    <header class="Main_Header">
        <div class="Main_Header-top">

            <small>Unhappy with your website?</small>
            <h1>We create beautiful and fast web services</h1>
        </div>

        <div class="Main_image"></div>
        <div class="Main_text">

            <section class="Main_Header-text">
                <h1>Story, emotion and purpose</h1>
                <p>We help transform your ideas into real world applications that will outperform your toughest
                    competition
                    and help you achieve your strategic goals in short period of time.</p>
            </section>
            <section class="Main_header-contact spanInput">
                <label>Want us to contact you?</label>
                <span> <input placeholder="Email" type="text"> <small>Join</small></span>
            </section>
        </div>

    </header>
</template>

<style scoped>
.Main_Header {
    display: grid;
    justify-items: center;
    text-align: start;
    min-height: 500px;
    height: 50%;
    width: 100%;
    margin-block: 40px 100px;
}

.Main_Header-top {
    width: 80%;
    margin-bottom: 15px;
}

.Main_image {
    background-image: url("../assets/people/photo1.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;


    width: 90%;
    max-width: 1330px;
    min-height: 114px;
    height: 20vh;

    border-radius: 12px;
    margin-bottom: 20px;
}



.Main_header-contact input {
    background-color: transparent;
}

.Main_header-contact span {
    background-color: #e1e1e1;
    /* padding: 0px; */
}

.Main_Header-text {
    width: 80%;
    max-width: 370px;
    text-align: center;
}

.Main_Header-text h1 {
    width: 200px;
}

.Main_Header-text p {
    font-size: 1.2rem;
    margin-block: 33px;
    width: 275px;

}


@media only screen and (min-width: 700px) {
    .Main_image {
        height: 30vh;
    }

    .Main_Header-top small {
        font-size: 1.8rem;
    }

    .Main_Header-top h1 {
        font-size: 4.8rem;
        width: 540px;
        margin-block: 16px 40px;
        line-height: 72px;
    }

    .Main_Header-text h1 {
        font-size: 4.8rem;
        width: 370px;
        line-height: 72px;
    }

    .Main_Header-text p {
        font-size: 1.8rem;
        line-height: 27px;
        width: 370px;
    }



}

@media only screen and (min-width: 1440px) {
    .Main_text {
        width: 80%;
    }

}
</style>