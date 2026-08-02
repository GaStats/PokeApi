# PokeAPI vjezba

- Uključite Handlebars biblioteku na stranicu koristeći CDN. View Handlebars [youtube guide](https://www.youtube.com/watch?v=2sXjmewEQOY)
- Proučite [Pokemon API](https://pokeapi.co/)
- Kreirajte request (bilo kojom metodom, fetch, XHR...) na API koji dohvaća prvih 20 Pokemon vrsta koje su žute boje
- Kreirajte HTML stiliziranu tablicu dobivenih rezultata koristeći Handlebars
- Lista mora sadržavati:
  - redni broj
  - ime vrste koje je ujedno i link na API endpoint sa vise informacija o vrsti

## Kako doprinjeti?

### Prvo forkaj pa kloniraj

Prvi korak je uvjek napraviti vlastitu kopiju odnosno _fork_ repozitorija te zatim klonirati taj svoj _fork_ na lokalni disk:

```sh
git clone https://github.com/<YOUR-USERNAME>/PokeApi.git
```

Otvoriti root repozitorija i instalirati pakete definirane u `package.json` datoteci: `handlebars`, `handlebars-loader`, `webpack`, `webpack-cli`. O navedenim paketima mozes procitati u sljedecem odlomku: [#dependancies](#dependancies)

```sh
cd PokeApi
npm install
```

>[!note]
>Ako nemas `npm` (_Node Package Manager_) potrebno je instalirati `node.js`, preuzmi ga sa sluzbenog weba: [nodejs.org](https://nodejs.org/en)

### Odradi svoj doprinos

Ako mislis da je tvoj doprinos premalen bit ce to dodatno iskustvo za tebe. Ne zamaraj se sa time. Svi smo tu da ucimo i rastemo.

>[!note]
>Bilo bi dobro da za sve sto radis imas odvojeni _branch_. U slucaju da nisi napravio redovan _sync_ svojeg i orginalnog repozitorija ili jednostvano dode do nekih konflikta sa starim i novim kodom, tada puno lakse uskladiti sve promjene ukoliko one nisu na _main_ branchu.

Nakon kaj napravis `git commit` pa onda i `git push` u svoju verziju remote repozitorija, na githubu otvori novi `pull request` i pricekaj da vlasnik originalnog repozitorija odobri tvoj zahtjev i napravi _merge_.

## Dependancies

```sh
npm install --save-dev handlebars handlebars-loader webpack webpack-cli
```

- [webpack](https://webpack.js.org): _bundler_, alat za _build_ i optimizaciju javascript i css datoteka. Iako trenutno postoje moderniji alati webpack je i dalje jedan od najrasirenijih alata. Tome je pridonio i _React.js_ koji ga je godinama koristio kao defaultni build tool.
- [webpack-cli](https://webpack.js.org/api/cli/): Omogucuje dodatne komande kako bi olaksao rad sa webpackom.
- [handlebars-loader for webpack](https://handlebarsjs.com/guide/installation/integrations.html#webpack-handlebars-loader): Omogucuje import predkompajlanih templatea. Kreiraj handlebars template datoteku `template.hbs` i mozes koristiti klasicnu import deklaraciju.

```js
import compiledTemplate from "./template.hbs";
```

### Read more

Bez obzira sto je zadatak jednostavan bilo bi dobro proci kroz dokumentaciju. Tako ces sa vremenom steci naviku citanja dokumentacije koje je ponekad tesko razumljiva ili jednostavno nije dovoljno prilagodjena razlicitim korisnicima. Snalazenje unutar tone podataka i novih informacija je vjestina koja se gradi polako.

- [handlebarsjs.com](https://handlebarsjs.com)
- [webpack.js.org](https://webpack.js.org)
