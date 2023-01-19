<template>
    <section class="Main_review">

        <h3>“Fast and outstanding resutls. Edie understands their customer’s needs. They have a young and talented
            team.” </h3>
        <article class="Main_review-card">
            <img src="../assets/people/person4.png" alt="person" srcset="">
            <div class="Card-text">
                <span>Carlos Tran</span>
                <span>The Decorate Gatsby</span>
            </div>
        </article>
    </section>

</template>



<style>
.Main_review {
    width: 90%;
    max-width: 630px;
}

.Main_review h3 {
    font-size: 2.4rem;
    line-height: 36px;
}

.Main_review-card {
    display: flex;
    margin-block: 30px 100px;

}

.Card-text {
    margin-left: 20px;

}

.Card-text span {
    display: block;
    height: 20px;

}

.Card-text span:nth-child(1) {
    font-size: 2.4rem;
    margin-bottom: 12px;
}

.Card-text span:nth-child(2) {
    font-size: 1.8rem;
    color: #828282;

}

.Main_review img {
    width: 100px;
}

@media only screen and (min-width: 1440px) {


    .Main_review {
        align-self: flex-start;
        margin-left: 150px;
    }
}
</style>