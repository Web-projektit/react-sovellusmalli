# React-sovellusmalli, ver. 2312 
Autentikointi: React context 
Muotoilu: Styled-components
Lomakkeiden validointi: React-hook-form v. 7
React-rooter-dom v. 6
Palvelinliitäntä:
- Autentikointi Session-evästeillä
- CORS-Headerit (cross origin)
- CSRF-tokenit 
Toimiva palveluliitäntä Flaskiin:
- Kirjautuminen, Poistuminen, Profiili
- Sovellusmallin käynnistäminen myös Flaskissä

Build toimii sekä Xamppissa että Flask-Blueprintissa react-sovellusmalli-nimisenä. Huom. haluttu package.json
täytyy kopioida halutun palvelimen mukaisesti joko kehitys-,
Xampp- tai flask-palvelimen package-*.json-tiedostosta.
Niissä on määritys build-kansion oikeaksi kohdeosoitteeksi.

Xamppissa se voidaan sijoittaa esim. htdocs/projektit_react-kansioon, jolloin
package.jsonin homepage-asetus on:

"homepage:"http://localhost/projektit_react/react-sovellusmalli/"

ja index.js-tiedostossa:

Router basename="/projektit_react/react-sovellusmalli"

Flask-Blueprinttiä ja React-kehityspalvelinta vastaavat asetukset ovat:
"homepage:"/react-sovellusmalli/" ja basename="/react-sovellusmalli"


React-autentikoinnin lähde: Denny Scott
https://www.dennyscott.io/blog/react-hooks-authentication, siinä käytetään
vanhempia React-ohjelmakirjastoja.

Laatinut: Jukka Aula
