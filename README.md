# 🧑🏻‍🚀 NFCtron Backend Case Study

> 👋 Vítejte u zadání pro kandidáty na pozici ⚙️ **Backend Developer** v NFCtron!

<img src="https://www.nfctron.com/data/blog/hr-mock.1733915983.jpg" alt="Buduj s NFCtron!" />

## 🛠️ Technologie

-   NodeJS 20+
-   Backendový framework NestJS 10 https://nestjs.com/
-   Typescript
-   Balíčkovací manager pnpm https://pnpm.io/
-   Testovací framework Jest https://jestjs.io/
-   git

## 📝 Zadání

Cílem je seznámit se se základními koncepty frameworku NestJS a napsat jednoduchý webový server, který simuluje evidenci zákazníků.

Po dokončení úkolu přiložte do žádosti u našeho inzerátu **Backend Developer | Incubation 2025**:

-   odkaz na Váš repozitář,
-   a odkaz na nasazenou aplikaci.

Struktura aplikace:

-   `AppModule`: hlavní modul, ze kterého se spouští aplikace, importuje `DataModule`
    -   `AppController`: HTTP controller, volá `DataService`
-   `DataModule`: modul pro správu dat
    -   `DataService`: služba, která simuluje práci s databází

Aplikace bude mít 4 HTTP endpointy:

-   Výpis všech zákazníků se základními informacemi
-   Detail jednoho zákazníka podle jeho ID
-   Vytvoření nového zákazníka
-   Editace zákazníka podle jeho ID

Úkolem Controlleru je přijímání požadavků a vracení odpovědi, ale nikoli správa dat. Data budou uskladněná v `DataService`. Není potřeba implementovat žádnou databázi, pro demonstraci postačí uložit do objektu/mapy/pole.

Jednoduchá sada unit testů vytvoří testovací modul a vyzkouší několik jednoduchých scénářů volání method `DataService`.

Pro splnění zadání se musí dát aplikace spustit přes `pnpm run start`, testy musí proběhnout zavoláním `pnpm run test`. Všechny parametry a návratové hodnoty musí mít explicitní Typescript datové typy.

## ⭐ Bonusy (podle obtížnosti)

-   [ ] Repozitář obsahuje více commitů s formátem podle https://www.conventionalcommits.org/en/v1.0.0/
-   [ ] Aplikace se spustí na portu definovaném ENV proměnnou `PORT`
-   [ ] Aplikace při startu načte ENV proměnné ze souboru `.env` přes https://www.npmjs.com/package/dotenv
-   [ ] DataService se při startu naplní náhodnými daty z knihovny https://github.com/faker-js/faker
-   [ ] Testy pro `AppController`, kde je `DataService` nahrazená mockem, který vrací předem definované hodnoty.
-   [ ] Interaktivní dokumentace k API generovaná přímo z kódu https://docs.nestjs.com/openapi/introduction.
-   [ ] Napojení na skutečnou relační (SQL) databázi podle vlastního výběru.

_A dalším vychytávkám se meze nekladou! Ukažte, co umíte! 💫_

## 📚 Zdroje

Doporučuju přečíst alespoň první kapitoly dokumentace NestJS, na internetu je spousta návodů, dobrý odrazový bod je třeba https://github.com/nestjs/typescript-starter. Testování je popsané v https://docs.nestjs.com/fundamentals/testing.

## 📋 Očekávané kompetence

-   V NFCtron pracujeme s širokým spektrem technologií, často je nutné se s nimi samostatně seznámit, projít dokumentaci a tutoriály. Seznamování s frameworkem NestJS by nemělo zabrat více než pár desítek minut.
-   Základ projektu je mít dobře rozvrženou architekturu. Projekt by měl být smysluplně rozdělený. **Přemýšlení** zabírá nejvíce času.
-   Na jednom projektu pracuje víc lidí a jeden člověk pracuje na více projektech. Je důležité, aby kód byl hezký, okomentovaný a pochopitelný i s odstupem času. Očekáváme, že toto **základní zadání se dá naprogramovat do dvou hodin.**
-   V bonusových zadáních jsou příklady věcí, se kterými se v našem týmu budeš potkávat denně. Hodně záleží na předchozích znalostech, proto jsou záměrně volně zadané. Bude nás zajímat i tvůj komentář, jak jsi se s nimi popral!

📧 Máte-li jakékoli dotazy nebo potřebujete pomoci, neváhejte se na nás obrátit na emailu [hr@nfctron.com](mailto:hr@nfctron.com).

---

Přejeme vám hodně štěstí a těšíme se na vaše řešení! 🌟

_–– Tým NFCtron_
