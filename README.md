# Backloganalyse & Trendvoorspelling – Wire Solutions

Deze repository bevat het Jupyter Notebook dat is gebruikt voor de
analyse van de backlogontwikkeling binnen de servicedesk van
Wire Solutions. De analyse is uitgevoerd als onderdeel van het
afstudeeronderzoek en dient als kwantitatieve verdieping van
**Deelvraag 4: Capaciteitsdruk en planningsimpact**.

De focus ligt op het analyseren van de ontwikkeling van de totale
backlog over de tijd en het beoordelen of sprake is van een
structureel capaciteitsprobleem of een tijdelijke mismatch tussen
instroom en afhandelcapaciteit.

---

## Doel van de analyse

Het doel van deze analyse is om inzicht te krijgen in:

- de opbouw en afbouw van de backlog over tijd;
- de verhouding tussen instroom en afhandeling op maandniveau;
- de verwachte ontwikkeling van de backlog bij ongewijzigd beleid.

De backlog wordt hierbij gebruikt als een samenvattende indicator
voor capaciteitswerking over de tijd. Op basis van een eenvoudige
trendanalyse wordt beoordeeld of achterstanden structureel zijn of
tijdelijk van aard.

De analyse is bedoeld ter ondersteuning van het onderzoeksrapport en
vormt geen operationeel voorspellingsmodel.

---

## Inhoud van het notebook

Het notebook bevat onder andere:

- inladen en opschonen van incidentdata;
- parsen en valideren van start- en einddatums;
- berekening van instroom en afhandeling per maand;
- bepaling van de backlog op maandultimo;
- trendanalyse van de backlog met behulp van lineaire regressie;
- een eenvoudige, indicatieve voorspelling van de backlogontwikkeling.

De analyse is bewust beperkt gehouden tot de totale backlog en maakt
geen onderscheid naar incidentcategorie of thema.

---

## Dataset

De gebruikte dataset is geanonimiseerd en niet opgenomen in deze
repository in verband met vertrouwelijkheid. De dataset bevat per
incident minimaal de volgende velden:

- incidentnummer;
- startdatum;
- einddatum.

De analyse is uitgevoerd op volledige maanden over de periode
februari tot en met oktober 2019. De maand november is expliciet
uitgesloten vanwege onvolledige data.

---

## Interpretatie en context

De resultaten van dit notebook worden gebruikt als inhoudelijke
onderbouwing van de capaciteitsanalyse in het onderzoeksrapport.
De trendanalyse laat zien dat de backlog zich in de eerste helft van
de onderzoeksperiode heeft opgebouwd, maar vanaf de zomer afneemt.
Dit nuanceert het beeld van structurele capaciteitsproblemen en wijst
op een tijdelijke mismatch tussen complexiteit en beschikbare
expertise.

De conclusies uit dit notebook dienen ter interpretatie en reflectie
en zijn niet bedoeld als direct sturings- of planningsinstrument.

---

## Technische omgeving

De analyse is uitgevoerd met Python en gangbare data-analysebibliotheken,
waaronder:

- pandas  
- numpy  
- matplotlib  
- scikit-learn  

Het notebook is reproduceerbaar met een vergelijkbare datasetstructuur.

---

### Opmerking

Dit notebook vormt een **aanvullende analyse** binnen het
afstudeeronderzoek en dient in samenhang met het onderzoeksrapport
te worden geïnterpreteerd.
