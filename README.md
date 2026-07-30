# Voertuigregistratie (MAGDA)

## Inleiding

Het traject _Voertuigregistratie_ streeft naar het ontsluiten van de gegevens over de houder en het voertuig achter een nummerplaat die op het wegennet wordt vastgesteld, bijvoorbeeld in het kader van trajectcontrole. Een trajectcontrole is een systeem dat de gemiddelde snelheid van een voertuig over een langere afstand meet via nummerplaatherkenning tussen twee meetpunten, in plaats van de snelheid op één punt zoals bij een klassieke flitspaal.

Dit traject is het implementatiemodel voor de gegevensuitwisseling rond de bestuurder. De registratie-, houder-, eigenaar- en voertuiggegevens worden op een uniforme, gestandaardiseerde wijze aan een nummerplaat gekoppeld, die hier gebruikt is als unieke identificator om de bijhorende informatie mee te ontsluiten. Het datamodel is gemodelleerd volgens een OSLO-applicatieprofiel en ontsloten via een REST-API (MAGDA Eucaris voertuigregistraties) met een Swagger/OpenAPI-specificatie.

Dankzij deze ontsluiting kunnen afnemers, die de nodige machtigingen bezitten, snel en makkelijk de houder en de voertuiggegevens opzoeken die horen bij een voertuig dat op een bepaald moment op het wegennet werd vastgesteld. Ook grensoverschrijdende (buitenlandse) nummerplaten kunnen zo, via Eucaris, bevraagd worden.

## Verslagen en presentaties

De verslagen en presentaties van dit traject kan je terugvinden op het [Standaardenregister](https://data.vlaanderen.be/standaarden).

## In deze repository

Deze repository bevat de bronbestanden en de configuratie om de specificaties van het traject te genereren en te publiceren:

- EAP-files met de UML-diagrammen van het informatie- en implementatiemodel ([`OSLO-Voertuigregistratie-MAGDA-IMPL.eap`](./OSLO-Voertuigregistratie-MAGDA-IMPL.eap)).
- De [Swagger/OpenAPI-specificatie](./resources/OSLO-Trajectcontrole-MAGDA-IM/artefacts/swagger/MAGDA-Voertuigregistraties-REST-Swagger.json) van de REST-API (`MAGDA Eucaris voertuigregistraties REST`, v0.1.0).
- Configuratie en bestanden voor het publiceren van de specs in de folders [`config`](./config), [`site-skeleton`](./site-skeleton) en [`templates`](./templates).
- Een [changelog](./resources/OSLO-Trajectcontrole-MAGDA-IM/artefacts/CHANGELOG.md) met de wijzigingen ten opzichte van vorige versies.

## Issues

Via de tab [issues](https://github.com/Informatievlaanderen/OSLOthema-voertuigregistratie/issues) kan je opmerkingen en feedback over het model geven.

## Publicaties

Uit dit traject vloeien de volgende specificaties voort. De licentie voor hergebruik is de [Modellicentie Gratis Hergebruik v1.0](https://data.vlaanderen.be/id/licentie/modellicentie-gratis-hergebruik/v1.0).

<!--TODO: Werk de status en de links bij zodra de standaarden op productie (data.vlaanderen.be) voorgelegd/gepubliceerd zijn. De onderstaande status is "Zonder status".-->

| Naam | Status | Uitgiftedatum | VOC | IMP |
| ---- | ------ | ------------- | --- | --- |
| Vocabularium Voertuigregistratie | Zonder status | 2026-07-24 | [Link](https://data.vlaanderen.be/standaarden/vocabularium-magda-voertuigregistratie/) | — |
| Vocabularium MAGDA-Voertuigregistratie | Zonder status | 2026-07-24 | [Link](https://data.vlaanderen.be/standaarden/vocabularium-magda-voertuigregistratie/) | — |
| Implementatiemodel MAGDA-Voertuigregistratie | Zonder status | 2026-07-24 | — | [Link](https://data.vlaanderen.be/standaarden/implementatiemodel-voertuigregistratie-magda/) |

## Codelijsten

### Github actions - generate_codelist.yml

Deze workflow converteert een CSV-codelijst naar een Turtle (.ttl) RDF-bestand. Volg deze stappen om deze workflow te gebruiken:

1. Bereid uw CSV-bestand voor in het formaat dat wordt verwacht door de generator (bv. `codelijsten/codelist.csv`).
2. Navigeer naar het tabblad **Actions** in de GitHub-repository.
3. Selecteer de workflow **Convert the codelist.csv into a .ttl file**.
4. Klik op **Run workflow** en geef het pad naar uw CSV-bestand op (bv. `codelijsten/codelist.csv`).
5. De workflow voert het volgende uit:
   - Genereert een `.ttl`-bestand uit het opgegeven CSV-bestand.
   - Verplaatst het gegenereerde bestand naar dezelfde map als uw CSV met de `.ttl`-extensie.
   - Voert het gegenereerde bestand automatisch in en pusht het naar de repository.

Het gegenereerde Turtle-bestand wordt opgeslagen naast uw CSV-bestand met dezelfde basisnaam maar met een `.ttl`-extensie.
