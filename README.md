Om
==
Dette er en alternativ leser for ebøkene på den digitale bokhylla til Nasjonalbiblioteket. Fra bokhylla kan du streame/lese over 170 tusen norske bøker, helt gratis! Du kan bruke leseren her: http://nbleser.herokuapp.com

Her er en demovideo av leseren: http://youtu.be/waUmeowGwjM

Hvorfor
=======
Jeg har irritert meg over Nasjonalbibliotekets leser, og håper de vil forbedre den. Her er noen av de tingene jeg mener ikke er optimale:

* Kræsjer ofte 
    - ubrukelig på iPad 
    - er på grunn av minnelekasje ved CSS overflow-y og -webkit-overflow-scrolling touch på iOS
* Dårlige muligheter for zoom
* Dårlig kontroll over kvalitet
* Ikke tilpasset fullscreen for iPad
* Vanskelig å gå til bestemt side (liten scroller)
* Popup med vilkår - unødvendig påtrengende

Poengene er demonstrert her: http://youtu.be/zvQaJ54-P4s

# Nåværende mangler i NBLeser
* Tekstsøk og merking i bok

[Les TODO](TODO.md)

# Nettressurser
Ressursene hentes av node.js ettersom nb.no ikke har access-control-allow-origin på nettressursene.

OpenSearch:
http://www.nb.no/services/search/v2/

Tilemap service:
http://www.nb.no/services/tilesv2/tilemap?viewer=html&pagetype=&format=json&URN=

Henter bilder(url fra tilemap):
http://www.nb.no/services/image/

Metadata til bøker:
http://xisbn.worldcat.org/webservices/xid/isbn/8200427005?method=getMetadata&format=json&fl=*

## Ressurser som ikke er tatt i bruk
Søkeforslag - http://www.nb.no/nbsok/suggestion/search?searchString=jo&maxResults=5&mediaType=&highlight=true

# Installer og kjør
```
git clone https://github.com/arve0/NBLeser.git
cd NBLeser
npm install
grunt
```
Åpne nettleser og gå til http://localhost:3000/

# Lisens
MIT - [les lisens](LICENSE.md)
