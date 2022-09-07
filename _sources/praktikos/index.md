# Užsienio šalių gerosios praktikos

Šioje dalyje bus aptariami atvirai prieinamų duomenų apie viešąjį transportą Europoje duomenų šaltiniai.

## Nacionaliniai prieigos punktai

Nors Europos Sąjungos valstybės privalo skelbti viešojo transporto duomenų rinkinius per [*nacionalinius prieigos
taškus*](https://transport.ec.europa.eu/system/files/2022-04/its-national-access-points_0.pdf) ([pagal 2017/1926
reglamentą](https://eur-lex.europa.eu/eli/reg_del/2017/1926/oj)), tačiau daugelis šių prieigos taškų yra
pasiekiami tik vietine kalba ir norint gauti duomenis reikia prisijungti.

Toliau pateikiama informacija apie viešojo keleivinio transporto duomenis, jų formatus daugumoje Europos Sąjungos
šalių.

```{table} Užsienio šalių viešojo transporto duomenų atvėrimo situacija. Adaptuota pagal [TrafikLab.se](https://www.trafiklab.se/api/other-apis/public-transport-europe/)
:name: countries-data-by-formats

| Šalis                                                                                                                   | GTFS                                                                                                                                                                 | NeTEx                                                                                              | GTFS Realtime                                                                                      | SIRI                                                                                                                       | Istoriniai statiniai duomenys                                                                        | Istoriniai dinaminiai duomenys                                |
|-------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| [🇮🇪 Airija](https://data.gov.ie/)                                                                                       | [GTFS](https://www.transportforireland.ie/transitData/PT_Data.html)                                                                                                  | [NeTEx](https://www.transportforireland.ie/transitData/PT_Data.html)                               | [GTFS Realtime](https://developer.nationaltransport.ie/apis)                                       |                                                                                                                            |                                                                                                      |                                                               |
| [🇦🇹 Austrija](https://www.mobilitydata.gv.at/)                                                                          | [GTFS](https://www.mobilitydata.gv.at/daten/soll-fahrplandaten-verkehrsverbünde-gtfs)                                                                                | [NeTEx](https://www.mobilitydata.gv.at/daten/soll-fahrplandaten-verkehrsverbünde-netex)            |                                                                                                    |                                                                                                                            | [Istoriniai GTFS](https://data.arge-oevv.at/de/data-sets)                                            |                                                               |
| [🇧🇪 Belgija](https://www.transportdata.be/en/)                                                                          | [GTFS](https://www.transportdata.be/en/dataset/tec-gtfs)                                                                                                             | [NeTEx](https://www.transportdata.be/en/dataset?q=netex&sort=score+desc%2C+metadata_modified+desc) | [GTFS Realtime](https://www.transportdata.be/en/dataset?res_format=Protocol+buffers)               |                                                                                                                            |                                                                                                      |                                                               |
| [🇧🇬 Bulgarija](https://lima.api.bg/)                                                                                    |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇩🇰 Danija](https://nap.vd.dk/)                                                                                         | [GTFS](https://help.rejseplanen.dk/hc/da/articles/214174465-Rejseplanens-API)                                                                                        |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇨🇿 Čekija](https://data.gov.cz/datov%C3%A9-sady)                                                                       | [GTFS](https://data.gov.cz/datová-sada?iri=https%3A%2F%2Fdata.gov.cz%2Fzdroj%2Fdatové-sady%2Fhttps---opendata.praha.eu-api-3-action-package_show-id-dpp-jizdni-rady) |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇪🇪 Estija](https://www.peatus.ee/)                                                                                     | [GTFS](https://www.mnt.ee/eng/public-transportation/public-transport-information-system)                                                                             |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇬🇷 Graikija](https://www.nap.gov.gr/)                                                                                  |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇪🇸 Ispanija](https://nap.mitma.es/)                                                                                    | [GTFS](https://nap.mitma.es)                                                                                                                                         |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇮🇹 Italija](https://www.cciss.it/)                                                                                     | [GTFS](https://data.opendatasoft.com/explore/dataset/it%40navitia/table/)                                                                                            | [NeTEx](https://netex-cen.eu/?page_id=237)                                                         |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇬🇧 Jungtinė Karalystė](https://data.bus-data.dft.gov.uk)                                                               | [GTFS](https://data.bus-data.dft.gov.uk/timetable/download/)                                                                                                         | [NeTEx](https://data.bus-data.dft.gov.uk/timetable/download/)                                      | [GTFS Realtime](https://data.bus-data.dft.gov.uk/avl/download/)                                    | [SIRI](https://data.bus-data.dft.gov.uk/avl/download/)                                                                     |                                                                                                      |                                                               |
| [🇨🇾 Kipras](https://www.traffic4cyprus.org.cy/)                                                                         |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇭🇷 Kroatija](https://www.promet-info.hr/)                                                                              | [GTFS](https://www.promet-info.hr/en/datasets?search=gtfs)                                                                                                           | [NeTEx](https://www.promet-info.hr/en/datasets?search=netex)                                       |                                                                                                    | [SIRI](https://www.promet-info.hr/en/datasets_details?id=ad1b1571-ebce-7fb2-c364-a19c6010175f)                             |                                                                                                      |                                                               |
| [🇱🇻 Latvija](https://lvceli.lv/en/road-network/statistical-data/transport-sector-open-data/)                            | [GTFS](https://data.lvceli.lv/opendata/EN/PublicTransport/)                                                                                                          |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇵🇱 Lenkija](https://dane.gov.pl/pl/dataset/1739,krajowy-punkt-dostepowy-kpd-multimodalne-usugi-informacji-o-podrozach) | [GTFS](https://mkuran.pl/gtfs/)                                                                                                                                      |                                                                                                    | [GTFS Realtime](https://dane.gov.pl/en/dataset/1803/resource/27427,dane-w-formacie-gtfs-rt/table)  |                                                                                                                            |                                                                                                      |                                                               |
| [🇱🇹 Lietuva](https://www.visimarsrutai.lt/gtfs)                                                                         | [GTFS](https://www.visimarsrutai.lt/gtfs/)                                                                                                                           | [NeTEx](https://www.visimarsrutai.lt/netex/)                                                       |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇱🇺 Liuksemburgas](https://data.public.lu/en/)                                                                          | [GTFS](https://data.public.lu/en/datasets/horaires-et-arrets-des-transport-publics-gtfs/)                                                                            | [NeTEx](https://data.public.lu/en/datasets/horaires-et-arrets-des-transport-publics-netex/)        | [GTFS Realtime](https://openov.lu/gtfs-rt/)                                                        |                                                                                                                            | [Istoriniai GTFS](https://data.public.lu/en/datasets/horaires-et-arrets-des-transport-publics-gtfs/) |                                                               |
| [🇲🇹 Malta](https://news.transport.gov.mt/data/)                                                                         |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇳🇴 Norvegija](https://transportportal.atlas.vegvesen.no/no/)                                                           | [GTFS](https://developer.entur.org/stops-and-timetable-data)                                                                                                         | [NeTEx](https://developer.entur.org/stops-and-timetable-data)                                      | [GTFS Realtime](https://developer.entur.org/pages-real-time-intro)                                 | [SIRI](https://developer.entur.org/pages-real-time-intro)                                                                  |                                                                                                      |                                                               |
| [🇳🇱 Nyderlandai](https://ndovloket.nl/)                                                                                 | [GTFS](https://gtfs.ovapi.nl/nl/)                                                                                                                                    |                                                                                                    | [GTFS Realtime](https://gtfs.ovapi.nl/nl/)                                                         |                                                                                                                            | [Istoriniai GTFS](https://gtfs.ovapi.nl/nl/archive/)                                                 |                                                               |
| [🇵🇹 Portugalija](https://nap-portugal.imt-ip.pt/)                                                                       |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇫🇷 Prancūzija](https://transport.data.gouv.fr/)                                                                        | [GTFS](https://transport.data.gouv.fr/datasets?q=GTFS)                                                                                                               | [NeTEx](https://transport.data.gouv.fr/datasets?q=netex)                                           | [GTFS Realtime](https://transport.data.gouv.fr/datasets?q=GTFS-RT)                                 | [SIRI](https://doc.transport.data.gouv.fr/foire-aux-questions-1/donnees-temps-reel-des-transports-en-commun#profils-netex) |                                                                                                      |                                                               |
| [🇷🇴 Rumunija](https://pna.cestrin.ro)                                                                                   | [GTFS](https://flashwebit.github.io/ROTI/)                                                                                                                           |                                                                                                    | [GTFS Realtime](https://flashwebit.github.io/ROTI/)                                                |                                                                                                                            |                                                                                                      |                                                               |
| [🇸🇰 Slovakija](https://odoprave.info)                                                                                   |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇸🇮 Slovėnija](https://www.ncup.si/en/multimodal)                                                                       |                                                                                                                                                                      |                                                                                                    |                                                                                                    |                                                                                                                            |                                                                                                      |                                                               |
| [🇫🇮 Suomija](https://www.finap.fi/)                                                                                     | [GTFS](https://finap.fi/#/services)                                                                                                                                  | [NeTEx](https://finap.fi/#/services)                                                               | [GTFS Realtime](https://finap.fi/#/services)                                                       | [SIRI](https://finap.fi/#/services)                                                                                        |                                                                                                      |                                                               |
| [🇸🇪 Švedija](https://www.trafficdata.se/)                                                                               | [GTFS](https://www.trafiklab.se/api/trafiklab-apis/gtfs-regional/static-specification/)                                                                              | [NeTEx](https://www.trafiklab.se/api/trafiklab-apis/netex-regional/)                               | [GTFS Realtime](https://www.trafiklab.se/api/trafiklab-apis/gtfs-regional/realtime-specification/) | [SIRI](https://www.trafiklab.se/api/trafiklab-apis/netex-regional/siri/)                                                   | [Istoriniai GTFS](https://www.trafiklab.se/api/trafiklab-apis/koda/koda-api-specification/)          | [KoDa API](https://www.trafiklab.se/api/trafiklab-apis/koda/) |
| [🇨🇭 Šveicarija](https://opentransportdata.swiss/en/)                                                                    | [GTFS](https://opentransportdata.swiss/de/dataset/timetable-2021-gtfs2020)                                                                                           | [NeTEx](https://opentransportdata.swiss/de/dataset/timetable-2021-netex-alpha)                     | [GTFS Realtime](https://opentransportdata.swiss/en/dataset/gtfsrt)                                 |                                                                                                                            | [Istoriniai GTFS](https://opentransportdata.swiss/en/dataset/timetable-2022-gtfs2020)                |                                                               |
| [🇭🇺 Vengrija](https://napportal.kozut.hu/)                                                                              | [GTFS](https://data.opendatasoft.com/explore/dataset/hu%40navitia/table/)                                                                                            | [NeTEx](https://www.transmodel-cen.eu/hungary-implementation/)                                     |                                                                                                    | [SIRI](https://www.transmodel-cen.eu/hungary-implementation/)                                                              |                                                                                                      |                                                               |
| [🇩🇪 Vokietija](https://service.mdm-portal.de/)                                                                          | [GTFS](https://gtfs.de/en/)                                                                                                                                          | [NetEx](https://www.vdv.de/netex.aspx)                                                             |                                                                                                    | [SIRI](https://www.transmodel-cen.eu/germany-implementation/)                                                              |                                                                                                      |                                                               |
```
