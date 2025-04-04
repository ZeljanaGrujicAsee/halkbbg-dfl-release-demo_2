# halkbbg-dfl-release-demo_2 - Repozitorijum za Arhiviranje Dokumentacije Isporučene Halk banci

Ovaj repozitorijum služi kao centralizovano mesto za arhiviranje dokumentacije koja se isporučuje banci prilikom svakog release-a. Cilj je da se obezbedi jasna organizacija, istorija promena i efikasna pretraga dokumenata prema nazivu i/ili sadržaju fajla.

## Struktura Repozitorijuma

Repozitorijum je organizovan po sledećoj strukturi:

```
halkbbg-dfl-release-demo_2/
├── ProizvodA/
│   ├── release-1.0.0/
│   │   ├── YYYY-MM-DD_HH_MM/ (timestamp kreiranja PR-a)
│   │   │   ├── dokument1.md
│   │   │   ├── dokument2.pdf
│   │   │   └── ...
│   │   ├── YYYY-MM-DD_HHMMSS/
│   │   │   ├── ...
│   │   └── ...
│   ├── release-1.1.0/
│   │   ├── ...
│   └── ...
├── ProizvodB/
│   ├── release-2.0.0/
│   │   ├── ...
│   └── ...
└── ...
```

* **` halkbbg-dfl-release-demo_2/`**: Root direktorijum repozitorijuma.
* **`ProizvodA/`, `ProizvodB/`, ...**: Grana za svaki proizvod npr. DigitalBranch, DigitalCIF, DigitalOrigination....
* **`release-1.0.0/`, `release-1.1.0/`, ...**: Folder za svaku verziju (release) proizvoda.
* **`YYYY-MM-DD_HHMMSS/`**: Podfolder za svaki pull request, sa timestamp-om kreiranja PR-a.
* **`dokument1.md`, `dokument2.pdf`, ...**: Dokumenti vezani za svaki pull request.

## Mehanizam Arhiviranja

1.  **Kreiranje Pull Request-a (PR), Merge PR-a, Kreiranje Release'a, Kopiranje Dokumenata:**
    * Prilikom kreiranja pull request-a u repozitorijumu [koji generiše](https://github.com/assecosee/halkbbg-dfl-release/tree/main)] generise .zip koji se isporučuje banci, a sadržaj repoa-a se prazni i priprema za sledeću isporuku, pre nego što se sadržaj ovog repo-a isprazni sadržaj documents podfoldera se kopira u okviru našeg repo-a na odgovarajuće grane.

## Prednosti

* **Jasna organizacija:** Dokumentacija je organizovana po proizvodima, verzijama i pull request-ovima.
* **Precizna istorija:** Timestamp-ovi omogućavaju precizno praćenje redosleda primene promena.
* **Efikasna pretraga:** Lako je pronaći dokumentaciju vezanu za određeni proizvod, verziju ili pull request.
* **Automatizacija:** Proces arhiviranja se može automatizovati pomoću Git akcija ili sličnih alata.

## Upotreba

* Koristiti Markdown format (`.md`) za dokumentaciju, jer se na taj način omogućava pretraga po imenu i-ili sadržaju fajlova.
