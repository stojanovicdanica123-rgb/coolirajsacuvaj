# °Cooliraj Sačuvaj™ — sajt

Novi sajt za [coolirajsacuvaj.rs](https://www.coolirajsacuvaj.rs/): uređaj koji od običnog kućnog klima uređaja i izolovanog prostora pravi pametnu rashladnu komoru.

Sajt je jedna statička stranica (HTML, CSS i JavaScript u `index.html`) i ne traži nikakav server ni build.

## Sadržaj

```
index.html        cela stranica
img/              slike (logo, uređaj, galerija, ledene teksture)
```

## Objavljivanje na GitHub Pages

1. Na GitHub-u napravite novi repozitorijum (npr. `coolirajsacuvaj`).
2. Kliknite **Add file → Upload files** i prevucite `index.html`, `README.md` i ceo folder `img`.
3. Kliknite **Commit changes**.
4. Idite na **Settings → Pages**, pod *Build and deployment* izaberite **Deploy from a branch**, grana `main`, folder `/ (root)`, pa **Save**.
5. Posle minut-dva sajt je dostupan na `https://<vaše-korisničko-ime>.github.io/coolirajsacuvaj/`.

### Sopstveni domen (coolirajsacuvaj.rs)

U **Settings → Pages → Custom domain** upišite `www.coolirajsacuvaj.rs`. Zatim kod registrara domena dodajte DNS zapis:

- `CNAME` za `www` → `<vaše-korisničko-ime>.github.io`

Kada se domen potvrdi, uključite **Enforce HTTPS**.

## Lokalni pregled

Otvorite `index.html` u browseru. Za potpuno isti prikaz kao na internetu (ledeni uvod koristi WebGL i učitava slike) pokrenite bilo koji lokalni server u ovom folderu, npr.:

```
npx serve .
```

## Napomene

- **Formular za upit** otvara email program posetioca sa popunjenom porukom na `info@coolirajsacuvaj.rs`. Za slanje direktno sa sajta može se povezati besplatan servis kao što je [Web3Forms](https://web3forms.com/) ili [Formspree](https://formspree.io/).
- **Ledeni uvod** se prikazuje jednom po poseti. Dodajte `?intro` na kraj adrese da ga ponovo vidite.
- Link **Prodavnica** u futeru i dalje vodi na postojeću prodavnicu (`coolirajsacuvaj.company.site`).
