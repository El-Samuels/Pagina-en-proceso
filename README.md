<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Página de El Samuels</title>
    <link rel="shortcut icon" href="imgSAM/favicon.png" type="image/x-icon">
    <!-- <link rel="stylesheet" href="css-terminado-ALEX/estilos.css"> -->
    <link href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,700,800&display=swap" rel="stylesheet">




    <style>
        * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'open sans';
}

.contenedor {
    padding: 60px 0;
    width: 90%;
    max-width: 1000px; 
    margin: auto;
    overflow: hidden;
}

.titulo {
    color: #642a73;
    font-size: 30px;
    text-align: center;
    margin-bottom: 60px;
}

/* Header */

header {
    width: 100%;
    height: 600px;
    background: #bc4e9c;
    /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, hsla(340, 95%, 50%, 0.459), hsla(317, 45%, 52%, 0.664)), url(../img-terminado-ALEX/portada.jpg);
    /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, hsla(340, 95%, 50%, 0.459), hsla(317, 45%, 52%, 0.664)), url(../img-terminado-ALEX/portada.jpg);
    /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    background-size: cover;
    background-attachment: fixed;
    position: relative;
}

nav{
    text-align: center;
    padding: 30px 50px 0 0;
}

nav > a{
    color:#fff;
    font-weight: 300;
    text-decoration: none;
    margin-right: 10px;
}

nav > a:hover{
    text-decoration: underline;
}

header .textos-header{
    display: flex;
    height: 430px;
    width: 100%;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    text-align: center;
}

.textos-header h1{
    font-size: 50px;
    color:#fff;
}

.textos-header h2{
    font-size: 30px;
    font-weight: 300;
    color:#fff;
}

.wave{
    position: absolute;
    bottom: 0;
    width: 100%;
}

/* About us */

main .sobre-nosotros{
    padding: 30px 0 60px 0;
}
.contenedor-sobre-nosotros{
    display: flex;
    justify-content: space-evenly;
}

.imagen-about-us{
    width: 48%;
}

.sobre-nosotros .contenido-textos{
    width: 48%;
}

.contenido-textos h3{
    margin-bottom: 15px;
}

.contenido-textos h3 span{
    background: #4d0686;
    color: #fff;
    border-radius: 50%;
    display: inline-block;
    text-align: center;
    width: 30px;
    height: 30px;
    padding: 2px;
    box-shadow: 0 0 6px 0 rgba(0, 0, 0, .5);
    margin-right: 5px;
}

.contenido-textos p{
    padding: 0px 0px 30px 15px;
    font-weight: 300;
    text-align: justify;
}

/* Galeria */


.portafolio{
    background: #f2f2f2;
}

.galeria-port{
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}

.imagen-port{
    width: 24%;
    margin-bottom: 10px;
    overflow: hidden;
    position: relative;
    cursor: pointer;
    box-shadow: 0 0 6px 0 rgba(0, 0, 0, .5);
}

.imagen-port > img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

.hover-galeria{
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    transform: scale(0);
    background: hsla(273,91%,27%, 0.7);
    transition: transform .5s;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

.hover-galeria img{
    width: 50px;
}

.hover-galeria p{
    color: #fff;
}

.imagen-port:hover .hover-galeria{
    transform: scale(1);
}

/* Clients */

.cards{
    display: flex;
    justify-content: space-evenly;
}

.cards .card{
    background: #4d0686;
    display: flex;
    width: 46%;
    height: 200px;
    align-items: center;
    justify-content: space-evenly;
    border-radius: 5px;
    box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.6);
}

.cards .card img{
    width: 100px;
    height: 100px;
    object-fit: cover;
    border: 3px solid #fff;
    border-radius: 50%;
    display: block;
}

.cards .card > .contenido-texto-card{
    width: 60%;
    color: #fff;
}

.cards .card > .contenido-texto-card p{
    font-weight: 300;
    padding-top: 5px;
}

/*  Our team */

.about-services{
    background: #f2f2f2;
    padding-bottom: 30px;
}


.servicio-cont{
    display:flex;
    justify-content: space-between;
    align-items: center;
}

.servicio-ind{
    width: 28%;
    text-align: center;
}

.servicio-ind img{
    width: 90%;
}

.servicio-ind h3{
    margin: 10px 0;
}

.servicio-ind p{
    font-weight: 300;
    text-align: justify;
}

/* footer */

footer{
    background: #414141;
    padding: 60px 0 30px 0;
    margin: auto;
    overflow: hidden;
}

.contenedor-footer{
    display: flex;
    width: 90%;
    justify-content: space-evenly;
    margin: auto;
    padding-bottom: 50px;
    border-bottom: 1px solid #ccc;
}

.content-foo{
    text-align: center;
}

.content-foo h4{
    color: #fff;
    border-bottom: 3px solid #af20d3;
    padding-bottom: 5px;
    margin-bottom: 10px;
}

.content-foo p{
    color: #ccc;
}

.titulo-final{
    text-align: center;
    font-size: 24px;
    margin: 20px 0 0 0;
    color: #9e9797;
}

@media screen and (max-width:900px){
    header{
        background-position: center;
    }

    .contenedor-sobre-nosotros{
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .sobre-nosotros .contenido-textos{
        width: 90%;
    }

    .imagen-about-us{
        width: 90%;
    }

    /* Galeria */

    .imagen-port{
        width: 44%;
    }

    /* Clientes */

    .cards{
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .cards .card{
        width: 90%;
    }

    .cards .card:first-child{
        margin-bottom: 30px;
    }

    /* servicios */

    .servicio-cont{
        justify-content: center;
        flex-direction: column;
    }

    .servicio-ind{
        width: 100%;
        text-align: center;
    }

    .servicio-ind:nth-child(1), .servicio-ind:nth-child(2){
        margin-bottom: 60px;
    }

    .servicio-ind img{
        width: 90%;
    }
}

@media screen and (max-width:500px){
    nav{
        text-align: center;
        padding: 30px 0 0 0;
    }

    nav > a{
        margin-right: 5px;
    }

    .textos-header h1{
        font-size: 35px;
    }

    .textos-header h2{
        font-size: 20px;
    }

    /* ABOUT US */

    .imagen-about-us{
        margin-bottom: 60px;
        width: 99%;
    }

    .sobre-nosotros .contenido-textos{
        width: 95%;
    }

    /* Galeria */

    .imagen-port{
        width: 95%;
    }

    /* Clients */

    .cards .card{
        height: 450px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .cards .card img{
        width: 90px;
        height: 90px;
    }

    /* Footer */

    .contenedor-footer{
        flex-direction: column;
        border: none;
    }

    .content-foo{
        margin-bottom: 20px;
        text-align: center;
    }

    .content-foo h4{
        border: none;
    }

    .content-foo p{
        color: #ccc;
        border-bottom: 1px solid #f2f2f2;
        padding-bottom: 20px;
    }

    .titulo-final{
        font-size: 20px;
    }
}
    </style>

</head> 

<body>
    <header>
        <nav>
            <a href="#">inicio</a>
            <a href="#"></a>
            <a href="#"></a>
            <a href="#"></a>
            <a href="#"></a>
        </nav>
        <section class="textos-header">
            <h1>Hola</h1>
            <h2>Pagina en proceso</h2>
        </section>
        <div class="wave" style="height: 150px; overflow: hidden;"><svg viewBox="0 0 500 150" preserveAspectRatio="none"
                style="height: 100%; width: 100%;">
                <path d="M0.00,49.98 C150.00,150.00 349.20,-50.00 500.00,49.98 L500.00,150.00 L0.00,150.00 Z"
                    style="stroke: none; fill: #fff;"></path>
            </svg></div>
    </header>
    <main>
        <section class="contenedor sobre-nosotros">
            <h2 class="titulo">Hola</h2>
            <div class="contenedor-sobre-nosotros">
                <img src="img-terminado-ALEX/ilustracion2.svg" alt="" class="imagen-about-us">
                <div class="contenido-textos">
                    <h3><span>1</span></h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, error?</p>
                    <h3><span>2</span></h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, excepturi.</p>
                        <h3><span>3</span></h3>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eveniet, illo!</p>
                </div>
            </div>
        </section>
        <section class="portafolio">
            <div class="contenedor">
                <h2 class="titulo">Portafolio</h2>
                <div class="galeria-port">
                    <div class="imagen-port">
                        <img src="img-terminado-ALEX/img1.jpg" alt="">
                        <div class="hover-galeria">
                            <img src="img-terminado-ALEX/icono1.png" alt="">
                            <p>Nuestro trabajo</p>
                        </div>
                    </div>
                    <div class="imagen-port">
                        <img src="img-terminado-ALEX/img2.jpg" alt="">
                        <div class="hover-galeria">
                            <img src="img-terminado-ALEX/icono1.png" alt="">
                            <p>Nuestro trabajo</p>
                        </div>
                    </div>
                    <div class="imagen-port">
                        <img src="img-terminado-ALEX/img3.jpg" alt="">
                        <div class="hover-galeria">
                            <img src="img-terminado-ALEX/icono1.png" alt="">
                            <p>Nuestro trabajo</p>
                        </div>
                    </div>
                </div>
            </div>
            </div>
            </div>
        </section>
        <section class="clientes contenedor">
            <h2 class="titulo">Que dicen nuestros clientes</h2>
            <div class="cards">
                <div class="card">
                    <img src="img-terminado-ALEX/face1.jpg" alt="">
                    <div class="contenido-texto-card">
                        <h4>Name</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae, sapiente!</p>
                    </div>
                </div>
                <div class="card">
                    <img src="img-terminado-ALEX/face2.jpg" alt="">
                    <div class="contenido-texto-card">
                        <h4>Name</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae, sapiente!</p>
                    </div>
                </div>
            </div>
        </section>
        <section class="about-services">
            <div class="contenedor">
                <h2 class="titulo">Nuestros servicios</h2>
                <div class="servicio-cont">
                    <div class="servicio-ind">
                        <img src="img-terminado-ALEX/ilustracion1.svg" alt="">
                        <h3>Name</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore, qui?</p>
                    </div>
                    <div class="servicio-ind">
                        <img src="img-terminado-ALEX/ilustracion4.svg" alt="">
                        <h3>Name</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore, qui?</p>
                    </div>
                    <div class="servicio-ind">
                        <img src="img-terminado-ALEX/ilustracion3.svg" alt="">
                        <h3>Name</h3>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore, qui?</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
    <footer>
        <div class="contenedor-footer">
            <div class="content-foo">
                <h4>Phone</h4>
                <p>8296312</p>
            </div>
            <div class="content-foo">
                <h4>Email</h4>
                <p>8296312</p>
            </div>
            <div class="content-foo">
                <h4>Location</h4>
                <p>8296312</p>
            </div>
        </div>
        <h2 class="titulo-final">&copy; El Samuels | Samuel</h2>
    </footer>
</body>

</html>
