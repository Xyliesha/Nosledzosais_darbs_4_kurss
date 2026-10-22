# Lumiere — Kino biļešu rezervēšanas sistēma

## 1. Projekta apraksts

**Lumiere** ir tīmekļa lietotne kino filmu apskatei un kino biļešu rezervēšanai. Projekts izstrādāts kā noslēguma kvalifikācijas darbs, izmantojot HTML, CSS, JavaScript, PHP un MySQL tehnoloģijas.

Sistēma ļauj lietotājiem apskatīt pieejamās filmas, meklēt filmas pēc nosaukuma, filtrēt tās pēc žanra, apskatīt filmu informāciju un seansus, kā arī rezervēt biļetes. Administratoram ir pieejama administrēšanas sadaļa, kurā iespējams pārvaldīt filmas, seansus un rezervācijas.

Projekta galvenais mērķis ir izveidot vienkārši lietojamu un pārskatāmu sistēmu, kas atvieglo kino filmu izvēli un biļešu rezervēšanas procesu.

## 2. Projekta mērķis

Izstrādāt tīmekļa lietotni, kas nodrošina kino filmu un seansu pārvaldību, lietotāju reģistrāciju un autorizāciju, kā arī biļešu rezervēšanu un rezervāciju administrēšanu.

### Projekta galvenie uzdevumi

- Izveidot lietotājam saprotamu un responsīvu tīmekļa saskarni.
- Nodrošināt filmu apskati, meklēšanu un filtrēšanu.
- Izveidot filmu un seansu informācijas attēlošanu.
- Nodrošināt lietotāju reģistrāciju un pieteikšanos sistēmā.
- Izstrādāt biļešu rezervēšanas funkcionalitāti ar sēdvietu izvēli.
- Izveidot administratora paneli filmu, seansu un rezervāciju pārvaldībai.
- Izmantot MySQL datubāzi informācijas glabāšanai.
- Nodrošināt datu apmaiņu starp tīmekļa saskarni, PHP un datubāzi.
- Izstrādāt biļešu rezervēšanas funkcionalitāti ar iespēju izvēlēties konkrētas sēdvietas kino zālē.

## 3. Izmantotās tehnoloģijas

| Tehnoloģija | Pielietojums                                            |
| ----------- | ------------------------------------------------------- |
| HTML5       | Tīmekļa lapu struktūras izveide                         |
| CSS3        | Lapu noformēšana un responsīvais dizains                |
| JavaScript  | Lietotāja saskarnes interaktivitāte un API pieprasījumi |
| PHP         | Servera puses loģika un datu apstrāde                   |
| MySQL       | Informācijas glabāšana un pārvaldība                    |
| XAMPP       | Vietējās izstrādes vides nodrošināšana                  |
| Apache      | PHP lietotnes apkalpošana lokālajā serverī              |
| phpMyAdmin  | MySQL datubāzes pārvaldība                              |

## 4. Sistēmas funkcionalitāte

### 4.1. Lietotāja funkcijas

Sistēma nodrošina iespēju izmantot kino biļešu iegādes un rezervēšanas funkcionalitāti gan viesiem, gan reģistrētiem Lumiere kluba biedriem.

Viesis var:

- Apskatīt pieejamās filmas un to detalizētu informāciju.
- Meklēt filmas pēc nosaukuma un filtrēt tās pēc žanra.
- Apskatīt filmu plakātus, aprakstus, ilgumu un vecuma ierobežojumus.
- Apskatīt pieejamos kino seansus, to datumus, laikus, zāles un biļešu cenas.
- Iegādāties vai rezervēt kino biļetes bez reģistrācijas, atbilstoši sistēmas darbības loģikai.
- Reģistrēties un pieteikties sistēmā, lai izmantotu Lumiere kluba biedra priekšrocības.
- Izvēlēties konkrētas sēdvietas kino zālē pirms biļešu iegādes.
- Apskatīt aizņemtās un brīvās sēdvietas izvēlētajā seansā.

Viesim tiek piemērota standarta biļetes cena bez Lumiere kluba biedra atlaides.

Reģistrēts Lumiere kluba biedrs var:

- Izmantot visas viesim pieejamās funkcijas.
- Iegādāties vai rezervēt kino biļetes, izmantojot savu lietotāja kontu.
- Saņemt Lumiere kluba biedra atlaidi atbilstoši sistēmā noteiktajiem nosacījumiem.
- Apskatīt savu rezervāciju vēsturi un rezervāciju statusus.
- Pārvaldīt savu lietotāja kontu, ja šāda funkcionalitāte ir pieejama.

Kluba biedra atlaide tiek piemērota reģistrētam lietotājam pēc pieteikšanās sistēmā. Viesim, kurš nav pieteicies savā kontā, tiek piemērota standarta biļetes cena.

### 4.2. Administratora funkcijas

Administrators ir atbildīgs par kino sistēmas satura un rezervāciju pārvaldību.

Administrators var:

- Pievienot jaunas filmas un rediģēt esošo filmu informāciju.
- Dzēst filmas no sistēmas.
- Norādīt filmas nosaukumu, aprakstu latviešu un angļu valodā, žanru, ilgumu, vecuma ierobežojumu un plakāta attēla ceļu.
- Pievienot filmu treileru saites, ja nepieciešams.
- Izveidot un pārvaldīt kino seansus.
- Norādīt seansa datumu, laiku, kino zāli, audio valodu, subtitru valodu un biļetes cenu.
- Apskatīt lietotāju veiktās rezervācijas.
- Mainīt rezervāciju statusus, piemēram, uz pending, paid vai cancelled, ja šādi statusi tiek izmantoti sistēmā.
- Dzēst rezervācijas.
- Apskatīt administrēšanas panelī pieejamo statistiku.

Administratora funkcijas ir paredzētas sistēmas satura atjaunošanai, seansu plānošanai un rezervāciju pārvaldībai.

### 4.3. Papildu funkcionalitāte

Sistēmā ir pieejamas arī šādas papildu iespējas:

- Populārāko filmu sadaļa, kas tiek veidota, pamatojoties uz rezervāciju datiem.
- Filmu treileru skatīšanās, izmantojot pievienotās saites.
- Filmu informācijas attēlošana latviešu un angļu valodā.
- Sistēmas statistikas attēlošana administratora panelī.
- Lumiere kluba biedra atlaižu piemērošana reģistrētiem lietotājiem atbilstoši sistēmā noteiktajiem nosacījumiem.
- Interaktīva kino zāles sēdvietu karte, kas ļauj apskatīt brīvās un aizņemtās sēdvietas un izvēlēties vietas konkrētam seansam.
