<header>
    <div class="wrapper">
        <div class="flex-left">
            <h1>
                Tom Deeterink
            </h1>
            <nav>
                <ul>
                    <li>
                        <a href="#">Projects</a>
                    </li>
                    <li>
                        <a href="#">About tom</a>
                    </li>
                    <li>
                        <a href="#">Contact</a>
                    </li>
                </ul>
            </nav>
        </div>
        <div class="flex-right">
    
        </div>
    </div>
</header>

<style>
header{
    width: 100%;
    background-color: var(--accent-dark);
}

.wrapper{
    max-width: 800px;
    padding: 4rem 2rem;
    display: flex;
    flex-direction: row;
    gap: 4em;
    margin: 0 auto;
}

.flex-left{
    display: flex;
    flex-direction: column;
    gap: 1em;
}

.flex-left h1{
    font-size: 15vw;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    color: var(--dark);
}

.flex-left ul{
    display: flex;
    flex-direction: column;
    list-style-type: none;
    gap: 2em;
}

.flex-left ul li a{
    font-size: 5vw;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    text-decoration: underline 4px solid;
    text-underline-offset: 0.35em;
    font-weight: 600;
    color: var(--secondary-color);
}

@media only screen and (min-width: 900px) {
    .flex-left h1 {
        font-size: 5em;
    }

    .flex-left ul {
        gap: 2em;
    }

    .flex-left ul li a {
        font-size: 3em;
        transition: 0.2s ease-out;
    }


    .flex-left ul li a::after {
        position: absolute;
        content: ">";
        margin-left: 1em;
        opacity: 0;
        transform: translateX(-100px);
        transition: ease-out 0.3s;
        color: var(--primary-color);
    }

    .flex-left ul li a:hover {
        color: var(--primary-color);
        transition: 0.2s ease-in;
        text-decoration: dotted 4px solid;
        text-underline-offset: 0.45em;
    }

    .flex-left ul li a:focus {
        color: var(--primary-color);
        transition: 0.2s ease-in;
        text-decoration: dotted 4px solid;
        text-underline-offset: 0.45em;
        outline: none;
    }

    .flex-left ul li a:hover::after {
        opacity: 1;
        position: absolute;
        content: ">";
        margin-left: 1em;
        transform: translateX(0px);
        transition: ease-in 0.3s;
    }

    .flex-left ul li a:focus::after {
        opacity: 1;
        position: absolute;
        content: ">";
        margin-left: 1em;
        transform: translateX(0px);
        transition: ease-in 0.3s;
    }
}

</style>