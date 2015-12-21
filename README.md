# Cookie-Policy-Bar
Come oramai è ben noto è obbligatorio inserire in qualsiasi sito web che faccia uso di Cookies una privacy policy che avverta l'utente di ciò che sta accadendo. A questo proposito eccomi qua per spiegarvi come creare un semplice popup che vi permetta di dichiarare all'utente l'utilizzo dei cookies.


<!-- Inserire questa porzione di codice subito dopo il tag <body> -->

<div id="cookie">
  <p>
    Questo sito usa i cookies per darti una migliore esperienza nella navigazione. Continuando accetti la nostra <a href="#">Cookies Policy</a>. 
      &nbsp; 
    <a id="close" href="#" onclick="javascript:nascondi()">X</a>
  </p>
</div>

<!----->



/* Inserire questa porzione di codice dentro dei tag <script> </script> all'interno dei tag <head> </head> */

function nascondi() {
		document.getElementById("cookie").style.display="none";
		}




/* Inserire questa porzione di codice dentro il vostro foglio di stile */

* {
  margin: 0;
  padding: 0;
}

body {
  background: #0000;
}

#cookie {
  position: relative;
  top: 0;
  width: 100%;
  background-color: #000;
  opacity: 0.8;
  color: #DFDFDF;
  text-align: center;
}

#cookie p {
  padding: 6px;
  font-family: Tahoma;
  font-size: 12px;
}

#cookie a {
  color: #aaa;
  text-decoration: underline;
}

#cookie a#close {
  font-weight: 900;
  color: #fff;
  text-decoration: none;
  background: #aaa;
  padding: 3px;
  -webkit-border-radius: 2px;
  -moz-border-radius: 2px;
  border-radius: 2px;
}
