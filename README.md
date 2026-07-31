#  Voertuigregistraties

## Inleiding

Het _MAGDA-Voertuigregistraties Implementatiemodel_, gebaseerd op de Europese standaard Eucaris, wisselt voertuigregistraties uit tussen Europese lidstaten in het kader van handhaving. Voertuigregistraties laten toe om eigenaren, houders en voertuigen uit te wisselen voor bijvoorbeeld handhavingsdoeleinden.

Dit implementatiemodel beperkt zich tot voertuigregistraties in het kader van handhaving, zoals het uitschrijven van snelheidsboetes bij trajectcontroles en andere automatische systemen die overtredingen kunnen vaststellen. De bevoegde diensten gebruiken de uitgewisselde gegevens om de vaststelling om te zetten in een effectieve boete.

Het implementatiemodel gebruikt OSLO Persoon en OSLO Organisatie voor het beschrijven van de houder en eigenaar van het voertuig; het voertuig zelf is hergebruikt van Schema.org. Specifiekere termen in verband met voertuigregistraties werden opgenomen in een apart vocabularium, los van het implementatiemodel.

Een samenvatting is beschikbaar op het [Standaardenregister](https://data.vlaanderen.be/standaarden/implementatiemodel-magda-voertuigregistraties) en het model zelf op [implementatie.data.vlaanderen.be](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/).

## In deze repository

Deze repository bevat de bronbestanden en de configuratie om de specificaties van het traject te genereren en te publiceren:

- EAP-files met de UML-diagrammen van het informatie- en implementatiemodel, gepubliceerd via het [implementatiemodel Voertuigregistraties](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/).
- De Swagger/OpenAPI-specificatie van de REST-API: [MAGDA-Voertuigregistraties-REST-Swagger.json](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/v0.1.0/resources/swagger/MAGDA-Voertuigregistraties-REST-Swagger.json) en de [herbruikbare OpenAPI-componenten](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/v0.1.0/resources/swagger/components.json).
- De herbruikbare [JSON-LD context](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/v0.1.0/context/voertuigregistratie-im.jsonld) en het [SHACL template](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/v0.1.0/shacl/voertuigregistratie-im-SHACL.ttl) van het implementatiemodel.
- Configuratie en bestanden voor het publiceren van de specs in de folders [`config`](./config), [`site-skeleton`](./site-skeleton) en [`templates`](./templates).
- Een [changelog](https://implementatie.data.vlaanderen.be/doc/implementatiemodel/magda/voertuigregistratie/v0.1.0/resources/CHANGELOG.md) met de wijzigingen ten opzichte van vorige versies.

## Issues

Via de tab [issues](https://github.com/Informatievlaanderen/OSLOthema-trajectcontrole/issues) kan je opmerkingen en feedback over het model geven.

## Publicaties

Uit dit traject vloeit het onderstaande implementatiemodel voort. De licentie voor hergebruik is de [Modellicentie Gratis Hergebruik v1.0](https://data.vlaanderen.be/id/licentie/modellicentie-gratis-hergebruik/v1.0).

| Naam | Status | Uitgiftedatum | IMP |
| ---- | ------ | ------------- | --- |
| Implementatiemodel MAGDA-Voertuigregistraties | Zonder status | 2026-07-24 | [Link](https://data.vlaanderen.be/standaarden/implementatiemodel-magda-voertuigregistraties) |
| Vocabularium MAGDA-Voertuigregistraties | Zonder status | 2026-07-24 | [Link](https://data.vlaanderen.be/standaarden/vocabularium-magda-voertuigregistraties) |
| Vocabularium Voertuigregistraties | Zonder status | 2026-07-24 | [Link](https://data.vlaanderen.be/standaarden/vocabularium-voertuigregistraties) |

