# Getting Started with JavaScript

JavaScript biasa di gunakan bebarengan dengan HTML dengan tag <script>

```html
<script>
  window.console.log("hello world");
</script>
```

untuk saat ini lupakan dulu tentang _window.console.log_ kita akan membahasnya setelah ini, _script_ adalah tag html dan seperti tag html lainnya jika ada pembuka maka ada penutup, dan di antara pembuka dan penutup adalah code javaScript yang bisa kita buat.

Hmm, lalu dimana kita bisa meletakkan JavaScript kita ? Mari kita lihat struktur file HTML terlebih dahulu

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

Kalian pasti bisa melihat tag _head_ dan _body_ bukan? nah kita bisa meletakkan JavaScript kita di dalam head ataupun body, namun disini saya hanya akan memberikan contoh _best practice_ yang biasa di gunakan ya, yakni kita akan menempatkan _script_ kita di tag **body** dan di tempatkan paling bawah setelah semua tag html yang kita punya.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>BashoCode - Online Coding Bootcamp</title>

    <!-- CSS  -->
    <link
      href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet"
    />
    <link
      href="css/materialize.css"
      type="text/css"
      rel="stylesheet"
      media="screen,projection"
    />
    <link
      href="css/style.css"
      type="text/css"
      rel="stylesheet"
      media="screen,projection"
    />
  </head>
  <body>
    <nav class="white" role="navigation">
      <div class="nav-wrapper container">
        <a id="logo-container" href="#" class="brand-logo">BhasoCode</a>
        <ul class="right hide-on-med-and-down">
          <li><a href="#">Get Started</a></li>
        </ul>

        <ul id="nav-mobile" class="sidenav">
          <li><a href="https://github.com/bashocode">Get Started</a></li>
        </ul>
        <a href="#" data-target="nav-mobile" class="sidenav-trigger"
          ><i class="material-icons">menu</i></a
        >
      </div>
    </nav>

    <div id="index-banner" class="parallax-container">
      <div class="section no-pad-bot">
        <div class="container">
          <br /><br />
          <h1 class="header center teal-text text-lighten-2">Basho Code</h1>
          <div class="row center">
            <h5 class="header col s12 light">Learn Coding for Free</h5>
          </div>
          <div class="row center">
            <a
              href="https://github.com/bashocode"
              id="download-button"
              class="btn-large waves-effect waves-light teal lighten-1"
              >Get Started</a
            >
          </div>
          <br /><br />
        </div>
      </div>
      <div class="parallax">
        <img src="background3.jpg" alt="Unsplashed background img 1" />
      </div>
    </div>

    <div class="container">
      <div class="section">
        <div class="row">
          <div class="col s12 center">
            <h3><i class="mdi-content-send brown-text"></i></h3>
            <h4>About Us</h4>
            <p class="left-align light">
              We know that coding bootcamp is too expensive, so we born for
              train people who want to dive into coding bootcamp, because we
              don't want to see people getting fail in coding bootcamp like us.
              After you graduated from this online coding bootcamp, we hope you
              guys can have a lot of knowledge to dive more deeper in
              programming, let's grow up together!
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="parallax-container valign-wrapper">
      <div class="section no-pad-bot">
        <div class="container">
          <div class="row center">
            <h5 class="header col s12 light">let's grow together!</h5>
          </div>
        </div>
      </div>
      <div class="parallax">
        <img src="background1.jpg" alt="Unsplashed background img 3" />
      </div>
    </div>

    <footer class="page-footer teal">
      <div class="container">
        <div class="row">
          <div class="col l6 s12">
            <h5 class="white-text">Chief of Sunshine</h5>
            <p class="grey-text text-lighten-4">
              Ikhda Muhammad Wildani is person who fail at coding bootcamp and
              decide to help other, because coding bootcamp is so expensive, we
              need you to know that coding bootcamp is not easy, so we want you
              to prepare yourself before joining coding bootcamp.
            </p>
          </div>
          <div class="col l3 s12">
            <h5 class="white-text">Find Ikhda</h5>
            <ul>
              <li>
                <a
                  class="white-text"
                  href="https://www.facebook.com/muhammad.dany.7161"
                  >Facebook</a
                >
              </li>
              <li>
                <a class="white-text" href="https://twitter.com/IkhdaWildani"
                  >Twitter</a
                >
              </li>
              <li>
                <a class="white-text" href="https://www.instagram.com/el_idni/"
                  >Instagram</a
                >
              </li>
              <li>
                <a
                  class="white-text"
                  href="https://www.linkedin.com/in/ikhda-muhammad-wildani-b98a03164/"
                  >Linkedin</a
                >
              </li>
              <li>
                <a
                  class="white-text"
                  href="https://medium.com/@ikhdamuhammadwildani"
                  >Medium</a
                >
              </li>
              <li>
                <a class="white-text" href="https://github.com/emzhofb"
                  >Github</a
                >
              </li>
            </ul>
          </div>
          <div class="col l3 s12">
            <h5 class="white-text">Find BashoCode</h5>
            <ul>
              <li>
                <a
                  class="white-text"
                  href="https://www.linkedin.com/company/14574156"
                  >Linkedin</a
                >
              </li>
              <li>
                <a class="white-text" href="https://github.com/bashocode"
                  >Github</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-copyright">
        <div class="container">
          Made by
          <a class="brown-text text-lighten-3" href="http://materializecss.com"
            >Materialize</a
          >
        </div>
      </div>
    </footer>

    <!--  Scripts-->
    <script src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
    <script src="js/materialize.js"></script>
    <script src="js/init.js"></script>
  </body>
</html>
```

Seperti yang kita lihat, kalau _css_ di tempatkan di **head** paling bawah, maka _script_ akan di letakkan di **body** paling bawah, itulah best practicenya.

Selanjutnya kita akan belajar window.
