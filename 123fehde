<script type="text/javascript">
// ******************** von http auf https umstellen ****************
// Ein Polyfill für die startsWith-Methode, falls sie nicht vom Browser unterstützt wird
if (!String.prototype.startsWith) {
  String.prototype.startsWith = function(search, pos) {
    pos = !pos || pos < 0 ? 0 : +pos;
    return this.substring(pos, pos + search.length) === search;
  };
}

// Die URL des aktuellen Webseitenaufrufs
var url = window.location.href;

// Die URL, mit der verglichen werden soll
var prefix = "http://www.123feh";

// Die Länge des Präfixes
var prefixLength = prefix.length;

// Die Variable, die den Rest der URL speichern soll
var urlRest;

// Überprüfen, ob die URL mit dem Präfix beginnt
if (url.startsWith(prefix)) {
  // Den Rest der URL ab dem 18. Zeichen extrahieren
  urlRest = url.substring(prefixLength);

  // Die neue URL zusammensetzen
  var NeuURL = "https://123feh.homepage.t-online" + urlRest;

  // Die Seite mit der neuen URL laden und einen Eintrag in der Browser-Historie erstellen
  window.location.assign(NeuURL);
}

// ************************ variablen
var seitenName = document.title;   // 
// ******************************************************

// ************************************** nur ein Button
// let link = document.getElementById("C_TKOMSI_com_cm4all_wdn_Button_26569830__-base");

// Dann ändern wir das target-Attribut des Links von "_blank" nach "_self"
// link.setAttribute("target", "_self");

// ************************************************** Alle Button auf _self.
// Zuerst wählen wir alle Links mit der Klasse "cm-widget-button_2" aus
let links = document.getElementsByClassName("cm-widget-button_2");

// Dann verwenden wir eine for-Schleife, um über alle Links zu iterieren
for (let i = 0; i < links.length; i++) {
  // Für jeden Link ändern wir das target-Attribut von "_blank" nach "_self"
  links[i].setAttribute("target", "_self");
}

// Das ist alles! Jetzt werden alle Links mit der Klasse "cm-widget-button_2" im selben Fenster geöffnet, wenn man darauf klickt.

// ****************************************************
// Ein neues Div-Element für den Inhalt erstellen
// *******************************************************
var div = document.createElement("div");
// 
// Hinter der Domain die zulässigen PageNamen erkennen
// ********************************************************************************
// Mit match die URL checken

//let checkName = window.location.pathname.match(/\/(Magazin|Portfolio|Service-Print|Atelier-Studio|Redaktion-Team)|[\?&;#]|$/);

let checkName = window.location.pathname.match(/\/(Magazin|Portfolio|Service-Print|Atelier-Studio|Redaktion-Team)|[\?&;#]|$/);

// wenn leer, weil Login-Routinen...dann.....
let pageName = checkName[1] || "Magazin"; // pageName ist jetzt "Magazin" oder der gefundene Pagename

// let pageName = checkName[1] || "Kunst-Idee"; // pageName ist jetzt "Kunst-Idee" oder der gefundene Pagename

// Den Inhalt und das Aussehen des Divs je nach dem Seitennamen anpassen
// ************************************
switch (pageName) {
  case "Portfolio":
    div.innerHTML = "<p>⚜Dies ist die Portfolio-Seite</p>";
    div.style.backgroundColor = "gold";
    break;

  case "Service-Print":
    div.innerHTML = "<p>💥Dies ist die Service-Print-Seite</p>";
    div.style.backgroundColor = "gold";
    break;

  case "Atelier-Studio":
    div.innerHTML = "<p>💦Dies ist die Atelier-Studio-Seite</p>";
    div.style.backgroundColor = "#a3c9d1";
    break;

case "Redaktion-Team":
div.innerHTML = "<p>💢Dies ist die Redaktion-Team-Seite</p>";
div.style.backgroundColor = "#a3c9d1";


// *************************************
// Das Element auswählen, das die Meldung enthält
let divC = document.getElementById("content_main");

// Überprüfen, ob die Meldung vorhanden ist
if (divC.innerHTML.includes("Sie sind leider nicht autorisiert, auf diesen Inhalt zuzugreifen.")) {
  // Den neuen HTML-Code anhängen
  divC.insertAdjacentHTML("beforeend", "<p><hr>Dies ist ein neuer Code🌐</p>");
}


// **************************************
    break;

  case "Magazin":
    div.innerHTML = "<p>💠Dies ist die Magazin-Seite</p>";
    div.style.backgroundColor = "Gold";
    break;

// eine Alternative, wenn LEER/ kein Page Name....
case "Kunst-Idee":
 div.innerHTML = "<p><h2><b>K</b>unst <b>I</b>dee⫘<b>A</b>rt <b>I</b>dea</h2></p>";
    div.style.backgroundColor = "#a3c9d1";
    break;
}

// Das "div" im HEAD anpassen
div.style.textAlign = "left"; // center
div.style.padding = "5px";
// div.style.background = "rgba(101, 165, 178, 0.00)"; // % opacity
// *****************was denn nun ?? *********************
// Das Div an das Ende des Body-Bereichs anhängen - jetzt nicht anzeigen !!

// document.body.appendChild(div);
document.body.insertBefore(div, document.body.firstChild);



// Einen Button erstellen
var button = document.createElement("button");
// ******************************************************************
// Den Inhalt und das Aussehen des Buttons anpassen
button.textContent = "⫘"; // ʭ 
button.style.border = "none";
button.style.borderRadius = "50%";
button.style.backgroundColor = "black";
button.style.color = "gold";
button.style.fontSize = "28px";
button.style.width = "50px";
button.style.height = "50px";
button.style.position = "fixed";
button.style.bottom = "10px";
button.style.right = "10px";
button.style.cursor = "pointer";
// Einen z-index-Wert für den Button festlegen
button.style.zIndex = "20"; 
// Dieser Wert muss größer sein als die z-index-Werte der anderen Divs
// Die font-weight-Eigenschaft für den Button auf einen höheren Wert setzen
// button.style.fontWeight = "bold"; 
// Dieser Wert macht das "" fett

// Eine Variable für das Infodiv erstellen
var infoDiv = null;
// ***************************************************************
// Die Funktion für den Button-Klick definieren
button.addEventListener("click", function() {
  // Wenn das Infodiv noch nicht existiert, es erstellen und ....
  if (infoDiv == null) {
    // Ein neues Div-Element für die Info erstellen
    infoDiv = document.createElement("div");
// ******************************************************************************
// Den Inhalt und das Aussehen der Info je nach dem Seitennamen / Farbe anpassen

var seitenName = document.title;   
var addDIV = "<div style='padding: 10px;'><h2>"+seitenName+"</h2><hr>";
var endDIV = "<p><a href='https://123feh.homepage.t-online.de/Magazin#TKOMSI_com_cm4all_wdn_Separatingline_26596260' target='_self' >User</a></p></div>";

switch (pageName) {
      case "Portfolio":
        infoDiv.innerHTML = "<p>Mehr Text zu Portfolio.....</p>";
      //  infoDiv.style.backgroundColor = "#65a5b2";
        break;

      case "Service-Print":
        infoDiv.innerHTML = `<div style="padding: 10px;"><p><h3>Service|Print</h3></p><hr><button onclick="window.location.href = 'https://123feh.homepage.t-online.de/Magazin#:~:text=%E2%82%85';">Herausgeber</button><img src="/.cm4all/uproc.php/0/Atelier-Studio/_8fb680e0-2f60-4977-950b-ecc090dda638.jpg“ style="width:10%;"></div>  `;
       // infoDiv.style.backgroundColor = "#65a5b2";
        break;

      case "Atelier-Studio":
        infoDiv.innerHTML = "<p>Mehr Text zu.... </p>";
       // infoDiv.style.backgroundColor = "#65a5b2";
        break;

      case "Redaktion-Team":
        infoDiv.innerHTML = "<p>Mehr über Redaktion....</p>";
     //   infoDiv.style.backgroundColor = "#8eddd6";
        break;

case "Magazin":
infoDiv.innerHTML = "<p>Weitres zu Magazin....</p>";
//  infoDiv.style.backgroundColor = "#65a5b2";
break;

// eine Alternative, wenn LEER/ kein Page Name....
case "Kunst-Idee":
 infoDiv.innerHTML = "<p><h3><b>K</b>unst <b>I</b>dee⫘<b>A</b>rt <b>I</b>dea</h3></p><hr>Dokument-Titel:"+seitenName;
//  infoDiv.style.backgroundColor = "white";
  break;

    }
infoDiv.innerHTML=addDIV+infoDiv.innerHTML+endDIV;

// infoDiv fstlegen
    infoDiv.style.width = "100%"; //94
    infoDiv.style.height = "100%"; //70
    infoDiv.style.position = "fixed";
    infoDiv.style.top = "0%"; //10
    infoDiv.style.left = "0%"; //3
    infoDiv.style.border = "1px solid red";
    // infoDiv.style.padding = "5px";
    // Einen z-index-Wert für die Info festlegen
    infoDiv.style.zIndex = "10"; // Dieser Wert muss gleich oder größer sein als der z-index-Wert des Buttons

    // Die Info in der Mitte der Seite positionieren
    infoDiv.style.textAlign = "left"; // center
// infoDiv.style.padding = "5px";
infoDiv.style.color = "#ffffff";
    infoDiv.style.position = "fixed";
    infoDiv.style.top = "50%";
    infoDiv.style.left = "50%";
    infoDiv.style.transform = "translate(-50%, -50%)";
   
    infoDiv.style.background = "rgba(101, 165, 178, 0.95)"; // % opacity
    // 101,165,178
   // infoDiv.style.padding = "10px 20px 30px 40px";
   // Ein neues Div-Element für das "X" erstellen (Ausschalter)
//***********************************************************************
    var x = document.createElement("div");
    // Den Inhalt und das Aussehen des "X" anpassen
    x.innerHTML = "❌";
    x.style.position = "absolute";
    x.style.top = "10px";
    x.style.right = "10px";
    x.style.cursor = "pointer";
    x.style.fontSize = "24px";
    x.style.color = "white";

    // Das Fenster schließen, wenn das "X" geklickt wird

    x.addEventListener("click", function() {
      infoDiv.style.display = "none";
    });

    // Das "X" an das Infodiv anhängen
    infoDiv.appendChild(x);

    // Die Info an das Ende des Body-Bereichs anhängen
    document.body.appendChild(infoDiv);
  }
  // Wenn das Infodiv schon existiert, es ein- oder ausblenden
  else {
    // Wenn die Info sichtbar ist, sie ausblenden
    if (infoDiv.style.display != "none") {
      infoDiv.style.display = "none";
    }
    // Wenn die Info nicht sichtbar ist, sie einblenden
    else {
      infoDiv.style.display = "block";
    }
  }
});

// ******Der runde schwebende ⫘ Button ******************
// Den Button an das Ende des Body-Bereichs anhängen
document.body.appendChild(button);

</script>
