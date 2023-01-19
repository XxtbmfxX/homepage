<template>
    <div class="Main_team">


        <div class="Main_tema-text">

            <h3>Meet the team</h3>
            <h1>We are chilled and a laidback team</h1>
            <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</span>
        </div>

        <div class="Main_tema-images">
            <img src="../assets/people/person3.png" alt="person" />
            <img src="../assets/people/person1.png" alt="person" />
            <img src="../assets/people/person2.png" alt="person" />
        </div>
    </div>

</template>

<style>
.Main_team {
    display: grid;
    justify-items: center;
    width: 90%;
}

.Main_team span {
    font-size: 1.6rem;
    display: block;
    width: 270px;
    margin-block: 14px 36px;
}

.Main_team h1 {
    font-size: 3.6rem;
    line-height: 54px;
}

.Main_team h3 {
    color: #EB5757;
}

.Main_team img {
    min-width: 145px;
    width: 30%;
    max-width: 291px;
}

.Main_tema-images img {
    border-radius: 24px;
}

.Main_tema-images {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    position: relative;
    margin-bottom: 100px;
    max-width: 600px;

}

.Main_tema-images img:nth-child(3) {
    grid-column: 2;
    justify-self: flex-end;
    width: 160px;

}

.Main_tema-images img:nth-child(2) {
    grid-column: 2;
    width: 144px !important;
    height: 144px !important;

}

.Main_tema-images img:nth-child(1) {
    position: absolute;
    top: 90px;
    width: 160px;
}

@media only screen and (min-width: 600px) {

    .Main_team {
        display: flex;
        width: 100%;
        justify-content: space-around;
    }

    .Main_tema-text h3 {
        font-size: 1.8rem;
    }

    .Main_tema-text {
        width: 280px;
    }

    .Main_tema-images img:nth-child(1) {
        width: 250px;
        height: 250px;

    }

    .Main_tema-images img:nth-child(2) {
        width: 260px !important;
        height: 260px !important;

    }

    .Main_tema-images img:nth-child(3) {
        width: 300px !important;
        height: 300px !important;
        justify-self: start;
        justify-self: start;

    }



}
</style>
