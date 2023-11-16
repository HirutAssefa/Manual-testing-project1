# Registrační formulář – Projekt 1 - Manuální testování (cz)

![Manuální testování](/images/registration-form.png)

## Obsah

- [Přehled projektu](#projekt-přehled)
- [Popis projektu](#Popis-projektu)
  - [V rozsahu](#v-rozsahu)
  - [Mimo rozsah](#mimo-rozsah)
  - [Prostředí - Prohlížeče](#prostředí-prohlížeče)
  - [Pokyny pro nastavení](#setup-instrukce)
  - [Jak spustit testy](#How-to-Run-the-Tests)
  - [Pokyny k hlášení problému](#insue-reporting-instructions)
  - [Pokyny pro testovací případy](#test-case-instrukce)
  - [Zkušební scénář-pdf](#Zkušební-scénář-pdf)
  - [Testovací případy-pdf](#Testovací-případy-pdf)
  - [Požadavky Matice sledovatelnosti-pdf](#Požadavky-Matice-sledovatelnosti-pdf)
  - [Hlášení chyb](#Hlášení-chyb)
- [Přispěvatelé](#přispěvatelé)
- [Licence](#licence)

## Přehled projektu

Vítejte v projektu manuální testování registračního formuláře. Tento projekt simuluje scénář v reálném světě, ve kterém manuální tester provádí hodnocení webových stránek registračních formulářů. Tento web jsem vytvořila pomocí CSS Bootstrap a projekt si klade za cíl otestovat různé funkce a funkce poskytované platformou pomocí průzkumného testování.

## Popis projektu

**Cíl projektu**

Tento projekt demonstruje mé dovednosti manuálního testování prostřednictvím komplexního vyhodnocení registračního formuláře. Mezi prováděné úkoly patří vytváření testovacích případů, scénářů, matice sledovatelnosti a hlášení chyb. Odráží základní povinnosti manuálních testerů v reálných scénářích.

### V rozsahu

**Test URL:** [OTEVŘENO`index.html` soubor]

**Oblasti zaměření:**

- Jméno
- Příjmení
- E-mail
- Heslo
- Registrace

**Zařízení:** PC/laptop

### Mimo rozsah

**Oblasti mimo rozsah:**

- Nefunkční testování

**Nehlásit:**

- Bezpečnostní problémy
- Problémy, které nelze reprodukovat více než dvakrát
- Problémy, které nejsou v rozsahu oblasti zaměření
- Problémy, které nejsou viditelné pro běžné uživatele (včetně chyb v protokolech konzoly)

**Drobné problémy:**

- Problémy se změnou velikosti okna prohlížeče

### Prostředí – Prohlížeče

**Podporovaná zařízení:** Mobilní zařízení, PC/laptop

**Nikdy nepoužívejte emulátory, simulátory.**

### Pokyny k nastavení

- Před zahájením testu vymažte mezipaměť prohlížeče a soubory cookie.
- Vypněte všechny blokátory reklam nebo skriptů, které mohou ovlivnit web.

### Jak spouštět testy

1. Klonujte toto úložiště.
2. Vstupte do registračního formuláře otevřením  souboru `index.html` ve webovém prohlížeči.
3. Proveďte manuální testování.
4. Zaznamenejte výsledky svých testů do matice sledovatelnosti a do dokumentů hlášení chyb.

### Pokyny k hlášení problémů

- Zajistěte dodržování pravidel hlášení chyb.
- **Formát názvu:** Zařízení – Oblast – Popis problému
  - Příklad: `[Windows 10][Domovská stránka]` – Po kliknutí na odkaz O Nás v patičce se otevře chybová stránka
  - Příklad: `[macOS Monterey 12.6.3][Košík]` – Kód kupónu zamítnut u vybrané položky

### Pokyny pro testovací případ

- Dokončete testovací případ ve stanoveném čase.
- Po dokončení testovacího případu nezapomeňte odeslat.

## Testovací scénář

**Scénář testu: Ověřte vstupy do registračního formuláře**

**Objektivní:** Ověřte vstupní pole registračního formuláře.

- Podrobné testovací scénáře pro registrační formulář naleznete v [Testovací scénář](/Documenty/RegistračníFormulář-testScénáře.pdf).

## Testovací případy

- Podrobné testovací případy pro výše uvedené scénáře lze nalézt v [Testovací případy](/Documenty/RegistračníFormulář-TestovacíPřípady.pdf).

## Matice sledovatelnosti

- Matice sledovatelnosti mapuje testovací scénáře na testovací případy, aby bylo zajištěno komplexní pokrytí testem. Matici lze nalézt v [Matice sledovatelnosti](/Documenty/RegistračníFormulář-RTM.pdf).

## Hlášení chyb

Níže jsou hlášení chyb, se kterými jsem se setkal. Protože existuje jen několik hlášení o chybách, nepoužil jsem nástroje pro hlášení chyb.

### Hlášení chyby 1

## Název: `[Windows 10][Stránka registrace]` – Dokončení procesu registrace bez potvrzovací zprávy

**ID chyby:** Registrace - chyba -1

**Vážnost:** Vysoký

**Typ problému:** Funkční

**Popis:**

Zdroj: Testovací případ TC_031

**Frekvence:** Reprodukovatelné

**Životní prostředí:** Windows 10, prohlížeč Chrome

**Provedená akce:**

1. Registrační stránku otevřete otevřením `index.html` soubor v prohlížeči.
2. Do pole „First Name“ zadejte platné křestní jméno (např. „Hirut“).
3. Do pole „Last Name“ zadejte platné příjmení (např. „Assefa“).
4. zadejte platnou e-mailovou adresu (např. „example@yahoo.com“).
5. zadejte platné heslo (např. „Wh@1ghafsdrW“).
6. Klikněte na tlačítko "Registrovat".

**Očekávaný výsledek:**

Po kliknutí na tlačítko "Registrovat" se všemi platnými údaji by měl být proces registrace úspěšně dokončen a měla by se zobrazit potvrzovací zpráva.

**Skutečný výsledek:**

Proces registrace byl úspěšně dokončen, ale nezobrazila se žádná potvrzovací zpráva.

**Přílohy:**

- Snímek obrazovky stránky "potvrzení registrace".

### Hlášení chyby 2

## Název: `[Window 10][Stránka registrace]` – 'Děkujeme za registraci' nebylo doručeno na mail

**ID chyby:** Registrace - chyba - 2

**Vážnost:** Vysoký

**Typ problému:** Funkční

**Popis:**

Zdroj: Testovací případ TC_037

**Frekvence:** Reprodukovatelné

**Životní prostředí:** Windows 10, prohlížeč Chrome

**Provedená akce:**

1. Registrační stránku otevřete otevřením`index.html` soubor v prohlížeči.
2. Do pole „First Name“ zadajte platné křestní jméno (např. „Hirut“).
3. Do pole „Last Name“ zadajte platné příjmení (např. „Assefa“).
4. zadajte platnou e-mailovou adresu (např. „example@yahoo.com“).
5. zadajte platné heslo (např. „Wh@1ghafsdrW“).
6. Klikněte na tlačítko "Registrovat".

**Očekávaný výsledek:**

Po úspěšné registraci účtu kliknutím na tlačítko „Registrovat“ se všemi platnými údaji by vám měl přijít e-mail „Děkujeme za registraci“.

**Skutečný výsledek:**

Po registraci nepřichází žádný e-mail „Děkujeme za registraci“.

**Přílohy:**

- Snímek obrazovky

## Přispěvatelé

- [Hirut Assefa](mailto:hirutassefa04@yahoo.com)

## Licence

Tento projekt je licencován pod licencí MIT. Viz [LICENCE](LICENCE) soubor pro podrobnosti.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Registration Form - Manual Testing Project - 1(en)

![Manual Testing](/images/registration-form.png)

## Table of Contents
- [Project Overview](#project-overview)
- [Project Description](#project-description)
  - [In Scope](#in-scope)
  - [Out of Scope](#out-of-scope)
  - [Environments - Browsers](#environments---browsers)
  - [Setup Instructions](#setup-instructions)
  - [How to Run the Tests](#How-to-Run-the-Tests)
  - [Issue Reporting Instructions](#issue-reporting-instructions)
  - [Test Case Instructions](#test-case-instructions)
  - [Test scenario-pdf](#test-scenario-pdf)
  - [Test cases-pdf](#test-scenario-pdf)
  - [Requirements Traceability Matrix-pdf](#Requirements-Traceability-Matrix)
  - [Bug report](#bug-report)
- [Contributors](#contributors)
- [License](#license)

## Project Overview

Welcome to the Registration Form manual testing project. This project simulates a real-world scenario in which a manual tester conducts the evaluation of registration form websites. I created this website using CSS Bootstrap, and the project aims to test various features and functionalities provided by the platform using exploratory testing.

## Project Description

**Project Objective**

This project demonstrates my manual testing skills through a comprehensive evaluation of a registration form. Tasks performed include creating test cases, scenarios, a traceability matrix, and bug reports. It mirrors the essential responsibilities of manual testers in real-life scenarios.

### In Scope

**Test URL:** [Open `index.html` file]

**Focus Areas:**

- First Name
- Last Name
- Email
- Password
- Register

**Devices:** PC/Laptop

### Out of Scope

**Out of Scope Areas:**

- Non-functional testing

**Do Not Report:**

- Security issues
- Issues that cannot be reproduced more than twice
- Issues that are not in scope
- Issues that are not visible to regular users (including errors in the console logs)

**Minor Issues:**

- Resize the browser window issues

### Environments - Browsers

**Supported Devices:** Mobile devices, PC/Laptop

**Never use emulators, simulators.**

### Setup Instructions

- Clear the browser's cache and cookies before starting the test.
- Disable any ad-blocker or script blocker that may affect the website.

### How to run tests

1. Clone this repository.
2. Access the registration form by opening the `index.html` file in a web browser.
3. Perform the manual tests.
4. Record your test results in the traceability matrix and bug report documents.

### Issue Reporting Instructions

- Ensure compliance with bug reporting rules.
- **Title Format:** Device - Area - Description of the issue
  - Example: `[Windows 10][Homepage]` - An error page opens after clicking on the About Us link in the footer
  - Example: `[macOS Monterey 12.6.3][Cart]` - Coupon code rejected for selected item

### Test Case Instructions

- Complete the test case within the specified time.
- Make sure to submit the test case after completing it.

## Test Scenario

**Test Scenario: Validate registration form inputs**

**Objective:** Validate the input fields of the registration form.

- Detailed test scenarios for the registration form can be found in the [Test Scenario](/Documenty/TestScenario-RegistrationForm(en).pdf) document.

## Test Cases

Detailed test cases for the above scenarios can be found in the [Test Cases](/Documenty/testCases-RegistrationForm(en).pdf) document.

## Traceability Matrix

The traceability matrix maps test scenarios to test cases to ensure comprehensive test coverage. The matrix can be found in the [Traceability Matrix](/Documenty/RegistrationForm-RTM(en).pdf) document.

## Bug reports

Below are bug reports I've encountered. Since there are only a few bug reports, I didn't utilize bug reporting tools.

### Bug report 1

## Title: `[Windows 10][Registration Page]` - Registration process completion without confirmation message

**Bug Id:** Registration - bug -1

**Severity:** High

**Issue Type:** Functional

**Description:**

Source: Test Case TC_031

**Frequency:** Reproducible

**Environment:** Windows 10, Chrome Browser

**Action Performed:**

1. Opened the registration page by opening the `index.html` file in the browser.
2. Entered a valid first name in the "First Name" field (e.g., "hirut").
3. Entered a valid last name in the "Last Name" field (e.g., "Assefa").
4. Entered a valid email address (e.g., "example@yahoo.com").
5. Entered a valid password (e.g., "Wh@1ghafsdrW").
6. Clicked on the "Register" button.

**Expected Result:**

Upon clicking the "Register" button with all valid inputs, the registration process should complete successfully, and a confirmation message should be displayed.

**Actual Result:**

The registration process completed successfully, but no confirmation message was displayed.

**Attachments:**

- Screenshot of the registration confirmation page.

### Bug report 2

# Bug Report

## Title: `[Windows 10][Registration Page]` - 'Thank you for registering' email not received after successful registration

**Bug Id:** Registration - bug -2

**Severity:** High

**Issue Type:** Functional

**Description:**

Source: Test Case TC_037

**Frequency:** Reproducible

**Environment:** Windows 10, Chrome Browser

**Action Performed:**

1. Opened the registration page by opening the `index.html` file in the browser.
2. Entered a valid first name in the "First Name" field (e.g., "hirut").
3. Entered a valid last name in the "Last Name" field (e.g., "Assefa").
4. Entered a valid email address (e.g., "example@yahoo.com").
5. Entered a valid password (e.g., "Wh@1ghafsdrW").
6. Clicked on the "Register" button.

**Expected Result:**

After successfully registering an account by clicking the "Register" button with all valid inputs, a 'Thank you for registering' email should be received.

**Actual Result:**

No 'Thank you for registering' email is received after registering.

**Attachments:**

- Screenshot

