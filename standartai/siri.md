# SIRI

SIRI (angl. *Service Interface for Real Time Information*) yra realaus laiko duomenų formatas vyraujantis Europos
Sąjungoje. Šis formatas turi būti naudojamas visuose ES nacionalinės prieigos taškuose siekiant užtikrinti sistemų
sąveikumą bei informuoti apie trumpalaikiais pokyčiais transporto
sistemoje{cite}`directive_multimodal_travel_information_services`.

SIRI yra NeTEx papildymas, NeTEx teikia statinę informaciją, o SIRI – dinaminę informaciją. Tiek SIRI, tiek NeTEx yra
sukurti remiantis bendru koncepciniu modeliu (Transmodel (CEN TC278, EN12896)).

## Naudojimo galimybės

SIRI gali būti naudojamas įvairiose srityse, pavyzdžiui{cite}`siri_cen_overview`:

- Teikti informaciją apie prognozuojamą transporto priemonių išvykimą iš stotelės realiu laiku;
- Teikti realaus laiko informaciją apie transporto priemones;
- Organizuoti transporto priemonių judėjimą tarp skirtingų transporto agentūrų;
- Keistis suplanuotais ir realaus laiko tvarkaraščių pakeitimais;
- Teikti pranešimus viešojo transporto keleiviams;
- Sinchronizuoti skirtingas transporto priemones ir organizuoti persėdimus tarp jų;
- Teikti informaciją apie veiklos rezultatus kitoms valdymo sistemoms

## ES direktyva

Pagal ITS direktyvą (2010/40/ES) šalys nusprendusios atverti dinaminius duomenis turi šiuos duomenis pateikti bent jau
SIRI formatu{cite}`directive_multimodal_travel_information_services`.

> (16) [...] Dėl keitimosi dinaminiais viešojo transporto duomenimis pasakytina, kad, valstybėms narėms nutarus į
> nacionalinį prieigos punktą **įtraukti dinaminius duomenis, tokiems duomenims turėtų būti naudojamos atitinkamos
keitimosi viešojo transporto duomenimis standarto SIRI CEN/TS 15531**, kurį nustatė Europos standartizacijos komitetas,
> dalys ir paskesnės atnaujintos jų redakcijos arba kitas visiškai suderintas kompiuterio skaitomas formatas. Valstybės
> narės gali nuspręsti valstybės narės lygmens nacionaliniam transportui toliau taikyti nacionalinius viešojo transporto
> duomenų standartus, tačiau nacionaliniame prieigos punkte turi būti naudojami nurodyti ES standartai, kad paslaugų
> sąveikumas ir ištisinis veikimas būtų užtikrintas visoje Europos Sąjungoje. Laikydamosi Europos standartizavimo
> reikalavimų, valstybės narės gali taikyti transliavimo ir konvertavimo metodus. Turėtų būti laikomasi nurodytų taikymo
> dieną aktualios redakcijos standartų. Turėtų būti atsižvelgiama į visus aktualius atnaujinimus, kuriais išplečiama
> standartų taikymo sritis arba į ją įtraukiami naujų rūšių duomenys;
>
> -- <cite>Europos Parlamento ir Tarybos direktyvos 2010/40/ES nuostatos dėl informacijos apie keliavimą daugiarūšiu
> transportu paslaugų teikimo{cite}`directive_multimodal_travel_information_services`</cite>

## Sudedamosios dalys

SIRI standartas duomenų apsikeitimui naudoja XML formatą (angl. *Extensible Markup Language*) ir susideda iš tokių
funkcinių dalių{cite}`siri_handbook`:

```{table} Pagrindinės SIRI funkcinės dalys
:name: siri-functional-services-table

| Funkcinė dalis                                                  | Aprašymas                                                                                                                                                          |
|-----------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Estimated Timetable (ET)**                                    | Realaus laiko nukrypimai nuo reguliariaus tvarkaraščio pateikiami dabartinei dienai                                                                                |
| **Production Timetable (PT)**                                   | Ateityje planuojami nurypimai nuo reguliariaus tvarkaraščio                                                                                                        |
| **Situation Exchange (SX)**                                     | Planuoti ir neplanuoti įvykiai transporto sistemoje                                                                                                                |
| **Vehicle Monitoring (VM)**                                     | Dabartinė konkrečios transporto priemonės pozicija bei su tuo susijusią informacija                                                                                |
| **Facility Monitoring (FM)**                                     | Infrastruktūros informacija pvz., susijusi su prieinamumu                                                                                |
| **Stop Timetable (ST)** ir **Stop Monitoring (SM)**             | Konkrečių stotelių prognozuojami transporto priemonių atvykimai ir išvykimai                                                                                       |
| **Connection Timetable (CT)** ir **Connection Monitoring (CM)** | Su persėdimu tarp skirtingų transporto priemonių susijusi realaus laiko informacija pvz., skirtas informuoti, kad vėluojančių traukinio keleivių palauks autobusas |
```

## Duomenų apsikeitimo procesas

SIRI formato duomenimis galima apsikeisti trimis skirtingais būdais.

### Asinchroninis duomenų apsikeitimas

*Publish/Subscribe - Direct delivery* ir *Publish/Subscribe - Fetched delivery* asinchroniniai apsikeitimo būdai leidžia
naudotojams nuolatos gauti duomenų pasikeitimus transporto sistemoje. Šis būdas užtikrina, kad duomenų naudotoją
greičiau pasiektų informaciją apie pasikeitimus bei yra labiau tinkamas dideliems duomenų kiekiams.

### Sinchroninis duomenų apsikeitimas

Sinchroninis duomenų apsikeitimas (*Request/response* metodu) yra gerokai paprastesnis ir buvo sukurtas palengvinti SIRI
formato įgalinimą. Analogiškai kaip ir GTFS Realtime atveju, duomenų naudotojas periodiškai kreipiasi į nuorodą bei
gauna reikalingus transporto sistemos duomenis. Taip pat dažnai suteikiama galimybė užklausos į serverį metu atlikti
filtravimą. Šis būdas įprastai vadinamas **SIRI Lite**.

```{figure} /images/standartai/siri/siri-functional-services.jpg
:name: siri-functional-services

SIRI duomenų apsikeitimo procesas ir funkcinės dalys{cite}`siri_overview`
```

## SIRI ir GTFS Realtime

Nors SIRI, palyginę su GTFS Realtime, SIRI formatą galime laikyti sudėtingesniu ir galinčiu perduoti daugiau
informacijos, tačiau šie formatai neturėtų būti laikomi vienas kito pakaitalais. Vis dėlto, egzistuoja nemažai panašumų
tarp šių formatų. Toliau lentelėje vaizduojami šių formatų atitikmenys.
```{table} GTFS Realtime ir SIRI formatų atitikmenys
:name: gtfs-realtime-and-siri-similarities
| Tipas                                | GTFS Realtime atitikmuo                                                                           | SIRI atitikmuo                                                                                       |
|--------------------------------------|---------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Kelionės eiga**                    | [Trip updates](https://developers.google.com/transit/gtfs-realtime/guides/trip-updates)           | [Estimated Timetable (ET)](https://enturas.atlassian.net/wiki/spaces/PUBLIC/pages/637370392/SIRI-ET) |
| **Transporto priemonės informacija** | [Vehicle positions](https://developers.google.com/transit/gtfs-realtime/guides/vehicle-positions) | [Vehicle Monitoring (VM)](https://enturas.atlassian.net/wiki/spaces/PUBLIC/pages/637370425/SIRI-VM)  |
| **Pranešimai keleiviams**            | [Service alerts](https://developers.google.com/transit/gtfs-realtime/guides/service-alerts)       | [Situation Exchange (SX)](https://enturas.atlassian.net/wiki/spaces/PUBLIC/pages/637370605/SIRI-SX)  |
```

## Naudinga informacija

- [Trumpas SIRI standarto vadovas](https://www.siri.org.uk/schema/1.3/doc/Handbook/Handbookv15.pdf)
- [Trumpas SIRI standarto pristatymas nacionaliniams prieigos punktams](https://www.its-platform.eu/wp-content/uploads/ITS-Platform/AchievementsDocuments/NAP/EU%20EIP%20-%20National%20Access%20Points%20-%20annual%20report%202020.pdf)