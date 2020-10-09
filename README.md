# cpnt260-a3
<!DOCTYPE html>
<html lang="en">
 <head> 
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> 

  <title>cpnt260-a3</title>
 <link rel="stylesheet" href="css/main.css"> 
<!-- This is a from font awsome -->
 <script src="https://kit.fontawesome.com/47de5a11a5.js" crossorigin="anonymous"></script>
   <style>

    body * {
     box-sizing: border-box;
     max-width:100vw; 
     height:auto;
     margin:0 auto 0 auto;;
     background-size:cover;
     background-position:center;
     font-family: 'Proza Libre', sans-serif;
    }
 
    main { 
     display: flex;
     flex-direction: column;
     height: 100vh;
     background-image: linear-gradient(180deg,white,hsla(360, 100%, 100%, 0.68)60%,transparent),linear-gradient(300deg,hsla(80, 100%, 50%, 0.17)10%, transparent), 
     url('https://static.politico.com/dims4/default/f4cf2c1/2147483647/resize/1160x%3E/quality/90/?url=https%3A%2F%2Fstatic.politico.com%2Fa3%2F9c%2F2cf9c39f479a8dfe5f7857f97913%2F200214-tobacco-ap-773.jpg');
     background-size: cover;
     background-repeat: no-repeat;
     background-position: center;
     font-family: 'Proza Libre', sans-serif;
    }
    
    h1{
     display: inline-block; 
     text-align:left;
     justify-content:left;
     font-size: 40px;
     letter-spacing: 5px;
     color:black;
     margin: 0.2em auto 0 auto;
     font-family: 'Open Sans', sans-serif;
    
    }
    .fas {
     display: inline-block; 
     justify-content:center;
     align-items:center;
     color:black;
     font-size: 50px;
     }

   p {
     display: flex; 
     text-align: center;
     justify-content:center;
     font-size: 20px;
     font-variant: small-caps;
     font-family: 'Proza Libre', sans-serif;
     background-position: center; 
     color:black;
     margin:auto;  
    }
    
   .card {
     display: flex; 
     min-width: 20ch;
     max-width: 50ch;
     margin:auto; 
     position:relative; 
     padding: 0.75em;
     border: 1px  solid rgba(40, 63, 63, 0.548) ;
     border-radius: 0.3em;
     font-family: 'Proza Libre', sans-serif;
     
    } 
    button {     
      display:inline-block;
      justify-content:center;
      align-items:center;
      border: 2px  solid rgb(97, 91, 91);
      border-radius: 0.2em;
      margin: 0;
      font-size: 20px; 
	    color:white;
      background-color: hsla(128, 100%, 16%, 1);
     	cursor: pointer;
     font-family: 'Proza Libre', sans-serif;
      font-weight: bold;
    }
    
    button:hover {
      font-size: 20px;
      background-color:tomato;
      color:black;
      text-decoration: underline;
    }
    
    botton:active {
     background-color: hsla(13, 100%, 33%, 1); 
      color:black;
    }

  / *paragraph*/
     legend {
     font-weight: bold;
     display:table;
     color:black;
     font-size:25px;
     justify-content:left;
     margin: 1em auto 0 auto;
     font-family: 'Proza Libre', sans-serif; 

    }
    /*form desiging*/
    .form {
     min-width: 50vh; 
     max-width: 50vh;
     height:auto ;
     margin: auto ;
     border: 1px solid grey;
     border-radius: 1rem;
     font-family: 'Proza Libre', sans-serif;
    }
    input {
      border: 1px solid rgb(90, 86, 86);
    }  
    /* Text fields */
     .text-fields p {
     display: flex;
     font-family: 'Proza Libre', sans-serif;
    }
    
    .text-fields p label {
     width: 15ch;
     font-size:15px;
     justify-content: center;
     font-weight:bold;
     font-size:17px;
     font-family: 'Proza Libre', sans-serif;
      }
   
    .text-fields p input {
     flex:1;
     width: 20ch; 
     font-size:12px;
     font-family: 'Proza Libre', sans-serif;
    }
    /* Checkboxes and Radio buttons */
    
    fieldset ul {
      margin-left: 1rem;
      margin-right: 1rem;
      border: none;
    }
    
    fieldset ul input {
     height:1em;
     width: 1em;
     border: none;

    }
    .reset-list{
     font-size: 12px;
     font-family: 'Proza Libre', sans-serif;
    }

    /* Submit */
    footer {
     text-align: center; 
     justify-content:center;
     font-family: 'Proza Libre', sans-serif;
    }
    
    /* Form reset */
    fieldset {
     border: none;
     margin: auto;
     font-size: 20px;
    }
/*red stat */
    abbr {
     color:red;
    }

   /*Media Queriesfor orientation and mobile screen*/
   @media (orientation: landscape) {
  body {
     flex-direction: row;
     background-repeat:repeat;
  }
}

@media (orientation: portrait) {
  body {
    flex-direction: column;
  }
}

@media screen and (max-width: 400px) {
  body {
     font-size: 15px;
     height:100vh;
  }
}
@media screen and (max-width: 800px) {
  body {
     font-size: 18px;
     height:100vh;
     background-repeat: repeat;
  }
}
</style>
 </head>
   <body>
    <main>
       <div>
        <h1>Green tobacco <i class="fas fa-smoking"></i></h1> 
         <p>"experince our full line of cigaret and cigar  accessories" </p>   
            <figure class="card">  
             <p> Stay Informed!</p>
              <button class="BT" type="submit">Subscribe</button>
            </figure> 
               <form action="#">
              <fieldset>
                 <legend>Please fill out the form:</legend>
                    <div class="form-wrapper">
                    <div class="text-fields">
                        <p>
                         <label for="fname">First Name:<abbr title="required" aria-label="required">*</abbr></label> 
                         <input type="text" id="fname" name="firstName" placeholder="What is your first name?" required>
                        </p>
                        <p>
                         <label for="lname">Last Name:<abbr title="required" aria-label="required">*</abbr></label> 
                         <input type="text" id="lname" name="lastName" placeholder="how about your last name?" required>
                          </p>
                        <p>
                         <label for="email">Email:<abbr title="required" aria-label="required">*</abbr></label> 
                         <input type="email" id="email" name="email"  placeholder="How do we contact you?" required>
                        </p>
                    </div>
              <fieldset>
                 <legend>Favorit meal of day</legend>
                <ul class="list-reset"> 
                 <li>
                    <label for="m1">
                      <input type="radio" id="m1" name="title" value="b">
                       Breakfast
                    </label>
                  </li>
                  <li>
                    <label for="m2">
                      <input type="radio" id="m2" name="title" value="l">
                       Lunch
                    </label>
                  </li>
                  <li> 
                     <label for="m3"> 
                      <input type="radio" id="m3" name="title" value="d">
                     Dinner
                     </label> 
                  </li>
                </ul>
               </fieldset>
              <footer>
               <button class="BT" type="submit">Submit</button>
              </footer>
            </div>
          </fieldset>
        </form>
      </div>
    </main>
  </body>
</html>
