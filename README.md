# firstRepo_Webpage
My Webpage Sample Profile

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Webpage</title>
    <link rel="stylesheet" href="style.css">

    <!--This is for material icons | OPTIONAL -->
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <!-- Latest compiled and minified CSS -->
  <link rel="stylesheet"
  href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css"
  integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

  <!-- Optional theme -->
  <link rel="stylesheet"
  href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css"
  integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

  <!--This is for the Social Media Icons-->
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css"
      integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">
  </head>
  <header>
    <h2 id>My Web Development Journey</h2><br>

    <div class="col">
      <ul class="mainNav">
        <li><a href="#aboutMe">ABOUT</a></li>
        <li><a href="#contacts">CONTACT</a><li>
      </ul>
    </div>
  </header>

  <!--BODY-->
  <body>
    <!--Scroll-to-top button-->
    <button id="btnScrollUp">
      <i class="material-icons">arrow_upward</i>
    </button>

    <!--Section 1-->
    <section class="section01">

      <!--Part one-->
      <div class="Journey">
        <p>Hameon</p>
      </div>

    </section>

    <div class="firstScript">
      <script class="script-1">

      </script>
    </div>

    <!--Section2-->
    <section class="section03">

      <div class="about">
        <p class="p1" id="aboutMe">ABOUT ME</p><br>

        <div class="myImage">
          <img src="me.JPG" width="300px" height="400px" align="right">
        </div>

        <p><strong>Name</strong>: Hamad Alsheraifi</p><br>
        <p><strong>Current info</strong>: I am a senior, undergraduate student at UAE University <br>
        majoring in Computer Engineering</p><br>
        <p><strong>Why Web Development</strong>: I found it as a new hobby that I want to <br>
        explore more about.</p><br>
        <p><strong>What I know so far</strong>: Frontend Dev - HTML, CSS, JS</p><br>
        <p><strong>Web Dev Goal</strong>: Achieve Full Stack Development Knowledge</p>
      </div>


    </section>


    <!--Section 3 -->
    <section class="section02">

      <div class="contact">
        <p class="p1" id="contacts">CONTACT</p>
        <p class="p2">Let's get in touch! You can find me in: </p><br>


        <ul class="SocialMediaLists">
          <li><a href="https://www.linkedin.com/in/hamad-h-alsheraifi-129bb51a0/" target="_blank"><i class="fab fa-linkedin"></i> LinkedIn</a></li><br>
          <li><a href="https://www.instagram.com/alsheraifi98/" target="_blank"><i class="fab fa-instagram"></i> Instagram</a></li><br>
          <li><a href="https://github.com/Hameon4" target="_blank"><i class="fab fa-github"></i> GitHub</a></li>
        </ul>
      </div>
    </section>


    <script>
      const btnScrollUp = document.getElementById("btnScrollUp");
      btnScrollUp.addEventListener("click", function() {//Gotta Check this out!!!!!!
        //window.scrollTo(0, 0);

        window.scrollTo ({top:0, left:0, behaviour:"smooth"});

      //$("html, body").animate({scrollTop: 0}, "slow");
      });
    </script>
    <!-- Latest compiled and minified JavaScript -->
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"
    integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>

  </body>
</html>



CSS PART BELOW
* { /*Something always needed*/
  padding: 0;
  margin: 0;
}

header { /*Gives a background to the header part*/
  background: #999;
  padding: 60px;
}

header h2 { /*This and the one below this separates the title and the lists*/
  float: left;
  font-size: 40px;
}

.mainNav {
  float: right;
}

.mainNav li {/*This puts all the list from downward list to row lists*/
  float: left;
  margin-left: 30px; /*Spacing b/w each list*/
}

.col ul { /*Removes the bullet points and any other features*/
  list-style: none;
}
.mainNav li a {/*Removes underlined link in each word*/
  text-decoration: none;
  color: green;
  font-size: 25px;
  transition: 0.3s ease-in;

}

.mainNav li:hover a { /*Animates the boxes on the header*/
  background: darkgrey;
  padding: 10px;
  border-radius: 10%;
}
.section01{
  background-image: url(bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 82vh;
}

.Journey p{ /*Hameon Text*/
  color: darkgreen;
  text-align: center;
  font-size: 100px;
  padding-top: 190px;
  margin-bottom: 20px;
  border: 1px solid black;
}

.frontendIMG{ /*This centers the image on the page*/
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.buttons a button{
  text-decoration: none;
}
#btnScrollUp {
  position: fixed; /*As we scroll down the page, it's gonna float on top of all the content*/
  right: 10px;
  bottom: 10px;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: green;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.25); /*Gotta check what this means*/
  color: white;
  outline: none; /*Need to look at this*/
  cursor: pointer;
  border: none;
}

#btnScrollUp:active { /*active sudo class*/
  background: darkgreen;
}

/*Section2 - About ME*/
.section03 {
  background: url(bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
}
.section03 .p1{
  color: darkgreen;
  font-size: 60px;
  text-align: center;
}

.section03 p{
  color: grey;
  font-size: 30px;
  margin-left: 15px;
}

.myImage img {
  margin-right: 10px;
  opacity: 0.5;
  border-radius: 50px;
}
/*Section 3 - Contact*/
.section02 {
  background: url(bg.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
}
.contact .p1{
  text-align: center;
  font-size: 60px;
  padding-top: 30px;
  color: darkgreen;
}

.contact .p2{
  font-size: 50px;
  padding-left: 10px;
  color: grey;
}

.SocialMediaLists {
  margin-left: 30px;
  float: left;
}

.SocialMediaLists a{
  font-size: 40px;
}

.SocialMediaLists li {
  list-style: none;
  margin: 10px 30px;
  display: inline-block;
  font-size: 20px;
  padding: 20px 20px;
  transition: 0.5s;
  float: left;
}

/*Responsive Part*/
@media only screen and (max-width: 980px) {

  header { /*Gives a background to the header part*/
    background: #999;
    padding: 50px;
  }

  header h2 {/*My Web Development Journey*/
    font-size: 25px;
    text-align: center;
    margin:-50px;
    margin-bottom: 20px;
    margin-left: auto;
    margin-right: auto;
    padding-top: 10px
  }

  .mainNav li{
    margin-left: 5px
  }
  .mainNav li a {
    color: green;
    font-size: 20px;
    transition: 0.3s ease-in;
    margin-left: 20px;
    margin-right: 20px;
  }

.myImage img {
  opacity: 0.5;
  border-radius: 10px;
  width: 150px;
  height: 200px;
  display: block;
  margin-left: auto;
  margin-right: auto;

  }

.section03 p{ /*About me paragraphs*/
  color: grey;
  font-size: 20px;
  margin-left: 15px;
  margin-right: 15px;
  }

.contact .p2{
  text-align: center;
  padding-top: 20px;
  font-size: 30px;
  padding-left: 10px;
  color: grey;
  margin-right: 20px;
  margin-left: 20px;
  }

.SocialMediaLists a{
  font-size: 30px;
  padding-left: 50px;
  }

  .Journey p{ /*Hameon Text*/
    color: darkgreen;
    text-align: center;
    font-size: 70px;
    padding-top: 190px;
    margin-bottom: 20px;
    border: 1px solid black;
  }

  .contact .p1{ /*Contact*/
    text-align: center;
    font-size: 40px;
    padding-top: 30px;
    color: darkgreen;
  }

  .section03 .p1{ /*About Me*/
    color: darkgreen;
    font-size: 40px;
    text-align: center;
  }
}

