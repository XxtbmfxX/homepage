<template>
    <footer class="Footer">
        <ul class="Footer_links">
            <li><a href="#"> Home </a></li>
            <li><a href="#"> Services </a></li>
            <li><a href="#"> Our Works</a></li>
            <li><a href="#"> Clients </a></li>
            <li><a href="#"> Contact</a> </li>
        </ul>
        <section class="Footer_social">
            <a href="#">
                <h1>
                    Edie
                </h1>
            </a>
            <div class="Footer_social-links">
                <ul>
                    <li><a href="#"><img src="../assets/linkIcons/instagram.svg" /> </a>
                    </li>
                    <li><a href="#"><img src="../assets/linkIcons/linkedin.svg" /> </a>
                    </li>
                    <li><a href="#"><img src="../assets/linkIcons/twitter.svg" /> </a>
                    </li>
                </ul>
            </div>

        </section>
        <section class="Footer_contact spanInput ">
            <label>Want us to contact you?</label>
            <span><input placeholder="Email" type="text"><small> Join</small></span>
        </section>
        <section class="Footer_by">
            <p>created by <a target="_blank" href="https://devchallenges.io/portfolio/XxtbmfxX">Toro </a> - <a
                    target="_blank" href="https://devchallenges.io">devChallenges.io</a> </p>
        </section>
    </footer>
</template>

<style>
.Footer_links,
.Footer_social,
.Footer_contact {
    margin-left: 44px;
    align-self: start;

}

.Footer li {
    margin-bottom: 10px;
}

.Footer a {
    color: #efefef;
    font-size: 1.8rem;
    margin-bottom: 20px;
}

.Footer {
    display: flex;
    flex-direction: column;
    align-items: center;

    background-color: #100E1D;
    color: #efefef;
    width: 100vw;
}


.Footer_links {
    margin-block: 40px 64px;
    width: 100px;
}


.Footer_social h1 a {
    color: #efefef;

}

.Footer_social h1 {
    margin-bottom: 20px;
    font-size: 3.6rem;
}

.Footer_social-links ul {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100px;
    margin-bottom: 65px;
}

.Footer_social-links ul li img {
    width: 24px;
    height: 24px;
    border-radius: 0px;

}

.Footer_contact {
    display: grid;
}


.Footer_by {
    margin-block: 150px 24px;
    font-size: 1.4rem;
}

.Footer_by p a:hover {
    text-decoration: underline;
    color: #333333;
}

@media only screen and (min-width: 700px) {

    .Footer_links,
    .Footer_social,
    .Footer_contact {
        margin: 0px;
        align-self: center;
    }

    .Footer {
        display: grid;
        gap: 20px;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: 300px 200px;
        justify-items: center;
        align-items: center;
    }

    .Footer_social ul {
        margin: 0px;
    }

    .Footer_by {
        grid-column: 2;
        margin: 0px;
    }
}
</style>
