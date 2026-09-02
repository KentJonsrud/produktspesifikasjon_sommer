#### Matrikkeladresse

offisiell adresse i form av et gårds- og bruksnummer og eventuelt et festenummer, eventuelt også et undernummer (Matrikkelforskriften § 2j)<br /><br />Merknad:<br />Matrikkeladresse er adresseidentifikasjon i et område der det ikke er tildelt vegadresse.<br /><br />Merknad2: Eventuelle bruksenhetsnummer som del av offisiell adresse kan ligge som egenskaper til matrikkeladressen<br /><br />Merknad3: Seksjonsnummer er ikke en del av den logiske identen for matrikkeladresse, - se egenskapen adressetekst.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>undernummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Fortløpende nummerering av matrikkeladresser med samme gårds-, bruks- og festenummer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Adresse

#### Atkomst

punkt som angir atkomst fra vegnett til en adresse.<br />Kommunen skal tillegge atkomstpunkt (koordinater) til adressen når det er nødvendig for å få klarere og mer entydige adresser.<br />Det er 3 lovlige alternativer for registrering av atkomst(er) på adresse:<br />1. Ingen atkomst registrert<br />2. Atkomst<br />3. AtkomstSommer og AtkomstVinter (hvis AtkomstSommer er registrert må også AtkomstVinter registreres og omvendt)<br /><br />Merknad: Atkomstpunktene kan ligge i en annen kommune enn adressepunktet

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>posisjon</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>punkt i nærheten av vegnett som angir atkomst fra vegnett til en adresse.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Punkt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>typeAtkomst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>om atkomstpunktet er en generell atkomst uavhengig av årstid eller om det er en sommeratkomst eller vinteratkomst</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeAtkomst</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- atkomst – generell atkomst, uavhengig av årstid<br />- atkomstSommer – atkomst sommerstid. Kan være en annen enn atkomst vinterstid pga ikke brøytede veger, båt-trafikk eller annet<br />- atkomstVinter – atkomst vinterstid. Kan være en annen enn atkomst sommersstid pga ikke brøytede veger, båt-trafikk eller annet</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adresseId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kobling til adresse i Matrikkelen (Adressens lokalId i matrikkelsystemet)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>uuidAtkomst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Objektidentifikator realisert som UUID, forvaltet av matrikkelsystemet<br /><br />Merknad:<br />UUID på Atkomst er ikke innført i Matrikkelen, men vil komme</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>uuidAdresse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kobling til adresse i Matrikkelen (Adressens id i matrikkelsystemet realisert som UUID)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt-AdresseAtkomst

#### SOSI_Objekt-AdresseAtkomst (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er fagområde-uavhengige og kan benyttes for alle objekttyper<br /><br />Merknad:<br />Spesielt i produktspesifikasjonsarbeid vil en velge egenskaper og av grensningslinjer fra denne klassen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAtkomst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik identifikasjon av et objekt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>IdentifikasjonAtkomst</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAtkomst.atkomstId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br /><br />NOTE: Det er data leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAtkomst.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br /><br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br /><br />Eksempel: NO for Norge.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAtkomst.versjonId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br /><br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>oppdateringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for siste endring på objektetdataene<br /><br />Merknad:<br />Oppdateringsdato kan være forskjellig fra Datafangsdato ved at data som er registrert kan bufres en kortere eller lengre periode før disse legges inn i datasystemet (databasen).<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>datauttaksdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for uttak fra en database<br /><br />Merknad:<br />Skiller seg fra Kopidato ved at en ikke skiller på om det er uttak fra en originaldatabase eller en kopidatabase.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>opphav</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>referanse til opphavsmaterialet, kildematerialet, organisasjons/publiseringskilde<br /><br />Merknad:<br />Kan også beskrive navn på person og årsak til oppdatering</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

#### Vegadresse

Offisiell adresse i form av et adressenavn og et adressenummer (matrikkelforskriften § 2i).<br /><br />Merknad:<br />Vegadresser er enkeltadresser innen en "veg" (adresseområde) i en kommune. Vegadresse identifiseres innen kommunen ved adressekode, husnummer (nummer) og eventuelt bokstav<br /><br />Merknad2: Eventuelle bruksenhetsnummer som del av offisiell adresse kan ligge som egenskaper til Vegadressen

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adressekode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Et nummer som entydig identifiserer adresserbare gater, veger, stier, plasser og områder som er ført i matrikkelen. For hvert adressenavn skal det således foreligge en adressekode, jf. matrikkelforskriften § 51.2.<br />Merknad: Adressekode er unik innenfor kommunen<br /><br />Merknad (teknisk): Avledet fra Veg-objektet i matrikkelsystemet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adressenavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Navn på gate, veg, sti, plass eller område som er ført i matrikkelen. (matrikkelforskriften § 2e)<br /><br />Merknad (teknisk): Avledet fra Veg-objektet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>bokstav</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>del av adressenummer (jfr Matrikkelforskrift § 2f).<br /><br />Ved behov kan det i tillegg til tallet brukes en etterfølgende bokstav. Bokstav skal bare brukes for å unngå omnummerering i tidligere tildelte adresser. Bokstav skal gis i alfabetisk rekkefølge. (matrikkelforskrift § 52 tredje ledd).<br /><br />Merknad: Høyst en bokstav</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>nummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Del av adressenummer som er definert slik i matrikkelforskrift:<br /><br />et nummer og en eventuell bokstav (husnummer) som entydig identifiserer eiendommer, anlegg, bygninger eller innganger til bygninger innenfor en adresserbar gate, veg, sti, plass eller område (Forskrift § 2f).</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Adresse

#### SOSI_Objekt-Adresse (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er fagområde-uavhengige og kan benyttes for alle objekttyper<br /><br />Merknad:<br />Spesielt i produktspesifikasjonsarbeid vil en velge egenskaper og av grensningslinjer fra denne klassen.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAdresse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik identifikasjon av et objekt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>IdentifikasjonAdresse</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAdresse.adresseId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>lokal identifikator, tildelt av dataleverendør/dataforvalter. Den lokale identifikatoren er unik innenfor navnerommet, ingen andre objekter har samme identifikator.<br /><br />NOTE: Det er data-leverendørens ansvar å sørge for at denne lokale identifikatoren er unik innenfor navnerommet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAdresse.navnerom</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnerom som unikt identifiserer datakilden til objektet, starter med to bokstavs kode jfr ISO 3166. Benytter understreking  ("_") dersom data produsenten ikke er assosiert med bare et land.<br /><br />NOTE 1 : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og vil registreres i "INSPIRE external  Object Identifier Namespaces Register"<br /><br />Eksempel: NO for Norge.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>identifikasjonAdresse.versjonId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>identifikasjon av en spesiell versjon av et geografisk objekt (instans), maksimum lengde på 25 karakterers. Dersom spesifikasjonen av et geografisk objekt med en identifikasjon inkludererer livsløpssyklusinformasjon, benyttes denne versjonId for å skille mellom ulike versjoner av samme objekt. versjonId er en unik  identifikasjon av versjonen.<br /><br />NOTE Maksimum lengde er valgt for å tillate tidsregistrering i henhold til  ISO 8601, slik som  "2007-02-12T12:12:12+05:30" som versjonId.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>oppdateringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for siste endring på objektetdataene<br /><br />Merknad:<br />Oppdateringsdato kan være forskjellig fra Datafangsdato ved at data som er registrert kan bufres en kortere eller lengre periode før disse legges inn i datasystemet (databasen).<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>datauttaksdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for uttak fra en database<br /><br />Merknad:<br />Skiller seg fra Kopidato ved at en ikke skiller på om det er uttak fra en originaldatabase eller en kopidatabase.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>DateTime</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>stedfestingVerifisert</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse om stedfestingen (koordinatene) er  kontrollert  og funnet i orden (verifisert)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Boolean</td>
    </tr>
  </tbody>
</table>

#### Adresse (abstrakt)

Matrikkelforskriften § 2d definerer den offisielle adressen som den fullstendige adressen for en<br />bygning, bygningsendring, bruksenhet, eiendom eller annet objekt som er registrert med adresse i matrikkelen.<br />I den offisielle adressen vil bruksenhetsnummer (for bolig eller annen bruksenhet) inngå når dette er nødvendig for å oppnå unik adresse.<br /><br />Merknad: Adresse realiseres enten som Vegadresse eller Matrikkeladresse

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adresseTekst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Del av offisiell adresse, men uten bruksenhetsnummer for adresser som ligger til bruksenheter/boliger<br /><br />Vegadresse:<br />,<br />ev= hvis fins. Hvis ikke skal formateringstegn utgå foran/bak.<br /><br />Matrikkeladresse:<br />, //-<br />ev= hvis fins. Hvis ikke skal formateringstegn utgå foran/bak.<br /><br />Eksempel:<br />"Storgata 2B" eller "123/4-2"<br />Der det i tillegg er adressetilleggsnavn:<br />"Haugen, Storgata 2B" eller "Midtgard, 123/4-2"<br /><br />Merknad:<br />Adressene er unike innenfor en kommune.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adresseTekstUtenAdressetilleggsnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Del av offisiell adresse, men uten bruksenhetsnummer for adresser som ligger til bruksenheter/boliger, - og uten eventuelle adressetilleggsnavn<br /><br />Vegadresse:<br /><br />ev= hvis fins. Hvis ikke skal formateringstegn utgå foran/bak.<br /><br />Matrikkeladresse:<br />//-<br />ev= hvis fins. Hvis ikke skal formateringstegn utgå foran/bak.<br /><br />Eksempel:<br />"Fjellvegen 2B" eller "12/4"<br />"Storgata 3" eller "12/5/3-2"</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adressetilleggsnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Nedarvet bruksnavn, navn på en institusjon eller bygning eller grend brukt som del av den offisielle adressen<br /><br />Merknad:<br />Eier kan kreve og kommunen kan tildele adressetilleggsnavn til en offisiell adresse etter vilkår i matrikkelforskriften § 54  og § 55. Hvilken regel den er tildelt etter skal registreres i matrikkelen (adressetilleggsnavnkilde)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>adressetilleggsnavnKilde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>opprinnelsen til adressetilleggsnavnet (§§ 54 og 55 i matrikkelforskriften)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>AdressetilleggsnavnKildeKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- krevdAvEier – &lt;font color="#333333"&gt;Når adressen gjelder et gårdsbruk, kan den som har grunnbokshjemmel til eiendommen som eier, kreve at den offisielle adressen også skal omfatte gårdens bruksnavn, dersom navnet faller språklig og geografisk sammen med et nedarvet stedsnavn, jf. lov 18. mai 1990 nr. 11 om stadnamn (&lt;/font&gt;matrikkelforskriftens § 54 1. ledd)<br />- anmodetAvHjemmelshaver – &lt;font color="#333333"&gt;Når adressen gjelder en særlig kjent institusjon eller bygning og allmenne hensyn taler for det, kan kommunen på anmodning fra registrert eier fastsette at den offisielle adressen også skal omfatte et navn på institusjonen eller bygningen (&lt;/font&gt;matrikkelforskriftens § 54 2. ledd)<br />- matrikkeladressenavn – &lt;font color="#333333"&gt;Adresser i område med matrikkeladresser som ikke har tildelt et adressetilleggsnavn etter reglene i § 54, kan tilordnes et matrikkeladressenavn etter &lt;/font&gt;matrikkelforskriftens § 55 3. ledd. Hvis det tildeles adressetilleggsnavn etter § 54 strykes matrikkeladressenavnet<br />- ikkeOppgitt – "Ikke oppgitt" brukes på adresser uten adressetilleggsnavn.<br />- tildeltAvKommunen – &lt;font color="#333333"&gt;Kommunen kan tildele adresser innenfor mindre grender, bolig- eller hyttefelt eller andre avgrensede områder et felles adressetilleggsnavn (&lt;/font&gt;Matrikkelforskriftens § 54 3. ledd, men tildeling etter 1. eller 2. ledd går foran 3. ledd)</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>atkomstId</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kobling til atkomst i Matrikkelen (Atkomstens lokalId i matrikkelsystemet)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>bruksenhetsnummerTekst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Del av offisiell adresse (bruksenhetsnummer) til en bruksenhet, f.eks en leilighet i flerboligbygg.<br /><br />Merknad:<br />Bokstaven og de to første tallene angir hvilken etasje leiligheten ligger i, og de to siste angir leilighetens nummer i etasjen, regnet fra venstre mot høyre.<br /><br />Eksempel: "H0102", "K0101"</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grunnkrets</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>adressens knytning til grunnkrets. Grunnkrets er den minste geografiske enhet det blir beregnet statistikk på<br /><br />Merknad:<br />En kommune er delt inn i flere grunnkretser.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GrunnkretsId</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grunnkrets.grunnkretsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>består av 8 siffer, hvor de fire første er kommunenummer, de to neste er delområdenummer og de to siste angir grunnkrets<br /><br />Merknad:<br />Det skal benyttes ledende nuller.<br /><br />Grunnkretskatalogen utgis og ajourføres av SSB, og er den offisielle listen over grunnkretser.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grunnkrets.grunnkretsnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>offisielt navn fra grunnkretskatalogen til SSB</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommunenavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn (norsk) på en kommune</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>kommunenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>nummerering av kommunen i henhold til Statistisk sentralbyrå sin offisielle liste<br /><br />Merknad: Det presiseres at kommunenummer alltid skal ha 4 siffer, dvs. eventuelt med ledende null.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kommunenummer</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer">http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer</a><br />- 0101 – Halden (Utgått 2020-01-01)<br />- 0102 – Sarpsborg (Utgått)<br />- 0103 – Fredrikstad (Utgått)<br />- 0104 – Moss (Utgått 2020-01-01)<br />- 0105 – Sarpsborg (Utgått 2020-01-01)<br />- 0106 – Fredrikstad (Utgått 2020-01-01)<br />- 0111 – Hvaler (Utgått 2020-01-01)<br />- 0113 – Borge (Utgått)<br />- 0114 – Varteig (Utgått)<br />- 0115 – Skjeberg (Utgått)<br />- 0118 – Aremark (Utgått 2020-01-01)<br />- 0119 – Marker (Utgått 2020-01-01)<br />- 0121 – Rømskog (Utgått 2020-01-01)<br />- 0122 – Trøgstad (Utgått 2020-01-01)<br />- 0123 – Spydeberg (Utgått 2020-01-01)<br />- 0124 – Askim (Utgått 2020-01-01)<br />- 0125 – Eidsberg (Utgått 2020-01-01)<br />- 0127 – Skiptvet (Utgått 2020-01-01)<br />- 0128 – Rakkestad (Utgått 2020-01-01)<br />- 0130 – Tune (Utgått)<br />- 0131 – Rolvsøy (Utgått)<br />- 0133 – Kråkerøy (Utgått)<br />- 0134 – Onsøy (Utgått)<br />- 0135 – Råde (Utgått 2020-01-01)<br />- 0136 – Rygge (Utgått 2020-01-01)<br />- 0137 – Våler i Østfold (Utgått 2020-01-01)<br />- 0138 – Hobøl (Utgått 2020-01-01)<br />- 0211 – Vestby (Utgått 2020-01-01)<br />- 0213 – Ski (Utgått 2020-01-01)<br />- 0214 – Ås (Utgått 2020-01-01)<br />- 0215 – Frogn (Utgått 2020-01-01)<br />- 0216 – Nesodden (Utgått 2020-01-01)<br />- 0217 – Oppegård (Utgått 2020-01-01)<br />- 0219 – Bærum (Utgått 2020-01-01)<br />- 0220 – Asker (Utgått 2020-01-01)<br />- 0221 – Aurskog-Høland (Utgått 2020-01-01)<br />- 0226 – Sørum (Utgått 2020-01-01)<br />- 0227 – Fet (Utgått 2020-01-01)<br />- 0228 – Rælingen (Utgått 2020-01-01)<br />- 0229 – Enebakk (Utgått 2020-01-01)<br />- 0230 – Lørenskog (Utgått 2020-01-01)<br />- 0231 – Skedsmo (Utgått 2020-01-01)<br />- 0233 – Nittedal (Utgått 2020-01-01)<br />- 0234 – Gjerdrum (Utgått 2020-01-01)<br />- 0235 – Ullensaker (Utgått 2020-01-01)<br />- 0236 – Nes i Akershus (Utgått 2020-01-01)<br />- 0237 – Eidsvoll (Utgått 2020-01-01)<br />- 0238 – Nannestad (Utgått 2020-01-01)<br />- 0239 – Hurdal (Utgått 2020-01-01)<br />- 0301 – Oslo<br />- 0401 – Hamar (Utgått)<br />- 0402 – Kongsvinger (Utgått 2020-01-01)<br />- 0403 – Hamar (Utgått 2020-01-01)<br />- 0412 – Ringsaker (Utgått 2020-01-01)<br />- 0414 – Vang (Utgått)<br />- 0415 – Løten (Utgått 2020-01-01)<br />- 0417 – Stange (Utgått 2020-01-01)<br />- 0418 – Nord-Odal (Utgått 2020-01-01)<br />- 0419 – Sør-Odal (Utgått 2020-01-01)<br />- 0420 – Eidskog (Utgått 2020-01-01)<br />- 0423 – Grue (Utgått 2020-01-01)<br />- 0425 – Åsnes (Utgått 2020-01-01)<br />- 0426 – Våler i Hedmark (Utgått 2020-01-01)<br />- 0427 – Elverum (Utgått 2020-01-01)<br />- 0428 – Trysil (Utgått 2020-01-01)<br />- 0429 – Åmot (Utgått 2020-01-01)<br />- 0430 – Stor-Elvdal (Utgått 2020-01-01)<br />- 0432 – Rendalen (Utgått 2020-01-01)<br />- 0434 – Engerdal (Utgått 2020-01-01)<br />- 0436 – Tolga (Utgått 2020-01-01)<br />- 0437 – Tynset (Utgått 2020-01-01)<br />- 0438 – Alvdal (Utgått 2020-01-01)<br />- 0439 – Folldal (Utgått 2020-01-01)<br />- 0441 – Os i Hedmark (Utgått 2020-01-01)<br />- 0501 – Lillehammer (Utgått 2020-01-01)<br />- 0502 – Gjøvik (Utgått 2020-01-01)<br />- 0511 – Dovre (Utgått 2020-01-01)<br />- 0512 – Lesja (Utgått 2020-01-01)<br />- 0513 – Skjåk (Utgått 2020-01-01)<br />- 0514 – Lom (Utgått 2020-01-01)<br />- 0515 – Vågå (Utgått 2020-01-01)<br />- 0516 – Nord-Fron (Utgått 2020-01-01)<br />- 0517 – Sel (Utgått 2020-01-01)<br />- 0519 – Sør-Fron (Utgått 2020-01-01)<br />- 0520 – Ringebu (Utgått 2020-01-01)<br />- 0521 – Øyer (Utgått 2020-01-01)<br />- 0522 – Gausdal (Utgått 2020-01-01)<br />- 0528 – Østre Toten (Utgått 2020-01-01)<br />- 0529 – Vestre Toten (Utgått 2020-01-01)<br />- 0532 – Jevnaker (Utgått 2020-01-01)<br />- 0533 – Lunner (Utgått 2020-01-01)<br />- 0534 – Gran (Utgått 2020-01-01)<br />- 0536 – Søndre Land (Utgått 2020-01-01)<br />- 0538 – Nordre Land (Utgått 2020-01-01)<br />- 0540 – Sør-Aurdal (Utgått 2020-01-01)<br />- 0541 – Etnedal (Utgått 2020-01-01)<br />- 0542 – Nord-Aurdal (Utgått 2020-01-01)<br />- 0543 – Vestre Slidre (Utgått 2020-01-01)<br />- 0544 – Øystre Slidre (Utgått 2020-01-01)<br />- 0545 – Vang (Utgått 2020-01-01)<br />- 0602 – Drammen (Utgått 2020-01-01)<br />- 0604 – Kongsberg (Utgått 2020-01-01)<br />- 0605 – Ringerike (Utgått 2020-01-01)<br />- 0612 – Hole (Utgått 2020-01-01)<br />- 0615 – Flå (Utgått 2020-01-01)<br />- 0616 – Nes i Buskerud (Utgått 2020-01-01)<br />- 0617 – Gol (Utgått 2020-01-01)<br />- 0618 – Hemsedal (Utgått 2020-01-01)<br />- 0619 – Ål (Utgått 2020-01-01)<br />- 0620 – Hol (Utgått 2020-01-01)<br />- 0621 – Sigdal (Utgått 2020-01-01)<br />- 0622 – Krødsherad (Utgått 2020-01-01)<br />- 0623 – Modum (Utgått 2020-01-01)<br />- 0624 – Øvre Eiker (Utgått 2020-01-01)<br />- 0625 – Nedre Eiker (Utgått 2020-01-01)<br />- 0626 – Lier (Utgått 2020-01-01)<br />- 0627 – Røyken (Utgått 2020-01-01)<br />- 0628 – Hurum (Utgått 2020-01-01)<br />- 0631 – Flesberg (Utgått 2020-01-01)<br />- 0632 – Rollag (Utgått 2020-01-01)<br />- 0633 – Nore og Uvdal (Utgått 2020-01-01)<br />- 0701 – Horten (Utgått 2020-01-01)<br />- 0702 – Holmestrand (Utgått)<br />- 0703 – Horten (Utgått)<br />- 0704 – Tønsberg (Utgått 2020-01-01)<br />- 0705 – Tønsberg (Utgått)<br />- 0706 – Sandefjord (Utgått)<br />- 0707 – Larvik (Utgått)<br />- 0708 – Stavern (Utgått)<br />- 0709 – Larvik (Utgått)<br />- 0710 – Sandefjord (Utgått 2020-01-01)<br />- 0711 – Svelvik (Utgått 2020-01-01)<br />- 0712 – Larvik (Utgått 2020-01-01)<br />- 0713 – Sande i Vestfold (Utgått 2020-01-01)<br />- 0714 – Hof (Utgått)<br />- 0715 – Holmestrand (Utgått 2020-01-01)<br />- 0716 – Re (Utgått 2020-01-01)<br />- 0717 – Borre (Utgått)<br />- 0718 – Ramnes (Utgått)<br />- 0719 – Andebu (Utgått)<br />- 0720 – Stokke (Utgått)<br />- 0721 – Sem (Utgått)<br />- 0722 – Nøtterøy (Utgått)<br />- 0723 – Tjøme (Utgått)<br />- 0725 – Tjølling (Utgått)<br />- 0726 – Brunlanes (Utgått)<br />- 0727 – Hedrum (Utgått)<br />- 0728 – Lardal (Utgått)<br />- 0729 – Færder (Utgått 2020-01-01)<br />- 0805 – Porsgrunn (Utgått 2020-01-01)<br />- 0806 – Skien (Utgått 2020-01-01)<br />- 0807 – Notodden (Utgått 2020-01-01)<br />- 0811 – Siljan (Utgått 2020-01-01)<br />- 0814 – Bamble (Utgått 2020-01-01)<br />- 0815 – Kragerø (Utgått 2020-01-01)<br />- 0817 – Drangedal (Utgått 2020-01-01)<br />- 0819 – Nome (Utgått 2020-01-01)<br />- 0821 – Bø i Telemark (Utgått 2020-01-01)<br />- 0822 – Sauherad (Utgått 2020-01-01)<br />- 0826 – Tinn (Utgått 2020-01-01)<br />- 0827 – Hjartdal (Utgått 2020-01-01)<br />- 0828 – Seljord (Utgått 2020-01-01)<br />- 0829 – Kviteseid (Utgått 2020-01-01)<br />- 0830 – Nissedal (Utgått 2020-01-01)<br />- 0831 – Fyresdal (Utgått 2020-01-01)<br />- 0833 – Tokke (Utgått 2020-01-01)<br />- 0834 – Vinje (Utgått 2020-01-01)<br />- 0901 – Risør (Utgått 2020-01-01)<br />- 0903 – Arendal (Utgått)<br />- 0904 – Grimstad (Utgått 2020-01-01)<br />- 0906 – Arendal (Utgått 2020-01-01)<br />- 0911 – Gjerstad (Utgått 2020-01-01)<br />- 0912 – Vegårshei (Utgått 2020-01-01)<br />- 0914 – Tvedestrand (Utgått 2020-01-01)<br />- 0918 – Moland (Utgått)<br />- 0919 – Froland (Utgått 2020-01-01)<br />- 0920 – Øyestad (Utgått)<br />- 0921 – Tromøy (Utgått)<br />- 0922 – Hisøy (Utgått)<br />- 0926 – Lillesand (Utgått 2020-01-01)<br />- 0928 – Birkenes (Utgått 2020-01-01)<br />- 0929 – Åmli (Utgått 2020-01-01)<br />- 0935 – Iveland (Utgått 2020-01-01)<br />- 0937 – Evje og Hornnes (Utgått 2020-01-01)<br />- 0938 – Bygland (Utgått 2020-01-01)<br />- 0940 – Valle (Utgått 2020-01-01)<br />- 0941 – Bykle (Utgått 2020-01-01)<br />- 1001 – Kristiansand (Utgått 2020-01-01)<br />- 1002 – Mandal (Utgått 2020-01-01)<br />- 1003 – Farsund (Utgått 2020-01-01)<br />- 1004 – Flekkefjord (Utgått 2020-01-01)<br />- 1014 – Vennesla (Utgått 2020-01-01)<br />- 1017 – Songdalen (Utgått 2020-01-01)<br />- 1018 – Søgne (Utgått 2020-01-01)<br />- 1021 – Marnardal (Utgått 2020-01-01)<br />- 1026 – Åseral (Utgått 2020-01-01)<br />- 1027 – Audnedal (Utgått 2020-01-01)<br />- 1029 – Lindesnes (Utgått 2020-01-01)<br />- 1032 – Lyngdal (Utgått 2020-01-01)<br />- 1034 – Hægebostad (Utgått 2020-01-01)<br />- 1037 – Kvinesdal (Utgått 2020-01-01)<br />- 1046 – Sirdal (Utgått 2020-01-01)<br />- 1101 – Eigersund<br />- 1102 – Sandnes (Utgått 2020-01-01)<br />- 1103 – Stavanger<br />- 1106 – Haugesund<br />- 1108 – Sandnes<br />- 1111 – Sokndal<br />- 1112 – Lund<br />- 1114 – Bjerkreim<br />- 1119 – Hå<br />- 1120 – Klepp<br />- 1121 – Time<br />- 1122 – Gjesdal<br />- 1124 – Sola<br />- 1127 – Randaberg<br />- 1129 – Forsand (Utgått 2020-01-01)<br />- 1130 – Strand<br />- 1133 – Hjelmeland<br />- 1134 – Suldal<br />- 1135 – Sauda<br />- 1141 – Finnøy (Utgått 2020-01-01)<br />- 1142 – Rennesøy (Utgått 2020-01-01)<br />- 1144 – Kvitsøy<br />- 1145 – Bokn<br />- 1146 – Tysvær<br />- 1149 – Karmøy<br />- 1151 – Utsira<br />- 1154 – Vindafjord (Utgått)<br />- 1159 – Ølen (Utgått)<br />- 1160 – Vindafjord<br />- 1201 – Bergen (Utgått 2020-01-01)<br />- 1211 – Etne (Utgått 2020-01-01)<br />- 1214 – Ølen (Utgått)<br />- 1216 – Sveio (Utgått 2020-01-01)<br />- 1219 – Bømlo (Utgått 2020-01-01)<br />- 1221 – Stord (Utgått 2020-01-01)<br />- 1222 – Fitjar (Utgått 2020-01-01)<br />- 1223 – Tysnes (Utgått 2020-01-01)<br />- 1224 – Kvinnherad (Utgått 2020-01-01)<br />- 1227 – Jondal (Utgått 2020-01-01)<br />- 1228 – Odda (Utgått 2020-01-01)<br />- 1231 – Ullensvang (Utgått 2020-01-01)<br />- 1232 – Eidfjord (Utgått 2020-01-01)<br />- 1233 – Ulvik (Utgått 2020-01-01)<br />- 1234 – Granvin (Utgått 2020-01-01)<br />- 1235 – Voss (Utgått 2020-01-01)<br />- 1238 – Kvam (Utgått 2020-01-01)<br />- 1241 – Fusa (Utgått 2020-01-01)<br />- 1242 – Samnanger (Utgått 2020-01-01)<br />- 1243 – Os i Hordaland (Utgått 2020-01-01)<br />- 1244 – Austevoll (Utgått 2020-01-01)<br />- 1245 – Sund (Utgått 2020-01-01)<br />- 1246 – Fjell (Utgått 2020-01-01)<br />- 1247 – Askøy (Utgått 2020-01-01)<br />- 1251 – Vaksdal (Utgått 2020-01-01)<br />- 1252 – Modalen (Utgått 2020-01-01)<br />- 1253 – Osterøy (Utgått 2020-01-01)<br />- 1256 – Meland (Utgått 2020-01-01)<br />- 1259 – Øygarden (Utgått 2020-01-01)<br />- 1260 – Radøy (Utgått 2020-01-01)<br />- 1263 – Lindås (Utgått 2020-01-01)<br />- 1264 – Austrheim (Utgått 2020-01-01)<br />- 1265 – Fedje (Utgått 2020-01-01)<br />- 1266 – Masfjorden (Utgått 2020-01-01)<br />- 1401 – Flora (Utgått 2020-01-01)<br />- 1411 – Gulen (Utgått 2020-01-01)<br />- 1412 – Solund (Utgått 2020-01-01)<br />- 1413 – Hyllestad (Utgått 2020-01-01)<br />- 1416 – Høyanger (Utgått 2020-01-01)<br />- 1417 – Vik (Utgått 2020-01-01)<br />- 1418 – Balestrand (Utgått 2020-01-01)<br />- 1419 – Leikanger (Utgått 2020-01-01)<br />- 1420 – Sogndal (Utgått 2020-01-01)<br />- 1421 – Aurland (Utgått 2020-01-01)<br />- 1422 – Lærdal (Utgått 2020-01-01)<br />- 1424 – Årdal (Utgått 2020-01-01)<br />- 1426 – Luster (Utgått 2020-01-01)<br />- 1428 – Askvoll (Utgått 2020-01-01)<br />- 1429 – Fjaler (Utgått 2020-01-01)<br />- 1430 – Gaular (Utgått 2020-01-01)<br />- 1431 – Jølster (Utgått 2020-01-01)<br />- 1432 – Førde (Utgått 2020-01-01)<br />- 1433 – Naustdal (Utgått 2020-01-01)<br />- 1438 – Bremanger (Utgått 2020-01-01)<br />- 1439 – Vågsøy (Utgått 2020-01-01)<br />- 1441 – Selje (Utgått 2020-01-01)<br />- 1443 – Eid (Utgått 2020-01-01)<br />- 1444 – Hornindal (Utgått 2020-01-01)<br />- 1445 – Gloppen (Utgått 2020-01-01)<br />- 1449 – Stryn (Utgått 2020-01-01)<br />- 1502 – Molde (Utgått 2020-01-01)<br />- 1504 – Ålesund (Utgått 2020-01-01)<br />- 1505 – Kristiansund<br />- 1506 – Molde<br />- 1507 – Ålesund<br />- 1511 – Vanylven<br />- 1514 – Sande i Møre og Romsdal<br />- 1515 – Herøy i Møre og Romsdal<br />- 1516 – Ulstein<br />- 1517 – Hareid<br />- 1519 – Volda (Utgått 2020-01-01)<br />- 1520 – Ørsta<br />- 1523 – Ørskog (Utgått 2020-01-01)<br />- 1524 – Norddal (Utgått 2020-01-01)<br />- 1525 – Stranda<br />- 1526 – Stordal (Utgått 2020-01-01)<br />- 1528 – Sykkylven<br />- 1529 – Skodje (Utgått 2020-01-01)<br />- 1531 – Sula<br />- 1532 – Giske<br />- 1534 – Haram (Utgått 2020-01-01)<br />- 1535 – Vestnes<br />- 1539 – Rauma<br />- 1543 – Nesset (Utgått 2020-01-01)<br />- 1545 – Midsund (Utgått 2020-01-01)<br />- 1546 – Sandøy (Utgått 2020-01-01)<br />- 1547 – Aukra<br />- 1548 – Fræna (Utgått 2020-01-01)<br />- 1551 – Eide (Utgått 2020-01-01)<br />- 1554 – Averøy<br />- 1557 – Gjemnes<br />- 1560 – Tingvoll<br />- 1563 – Sunndal<br />- 1566 – Surnadal<br />- 1567 – Rindal (Utgått)<br />- 1569 – Aure (Utgått)<br />- 1571 – Halsa (Utgått 2020-01-01)<br />- 1572 – Tustna (Utgått)<br />- 1573 – Smøla<br />- 1576 – Aure<br />- 1577 – Volda<br />- 1578 – Fjord<br />- 1579 – Hustadvika<br />- 1601 – Trondheim (Utgått)<br />- 1612 – Hemne (Utgått)<br />- 1613 – Snillfjord (Utgått)<br />- 1617 – Hitra (Utgått)<br />- 1620 – Frøya (Utgått)<br />- 1621 – Ørland (Utgått)<br />- 1622 – Agdenes (Utgått)<br />- 1624 – Rissa (Utgått)<br />- 1627 – Bjugn (Utgått)<br />- 1630 – Åfjord (Utgått)<br />- 1632 – Roan (Utgått)<br />- 1633 – Osen (Utgått)<br />- 1634 – Oppdal (Utgått)<br />- 1635 – Rennebu (Utgått)<br />- 1636 – Meldal (Utgått)<br />- 1638 – Orkdal (Utgått)<br />- 1640 – Røros (Utgått)<br />- 1644 – Holtålen (Utgått)<br />- 1648 – Midtre Gauldal (Utgått)<br />- 1653 – Melhus (Utgått)<br />- 1657 – Skaun (Utgått)<br />- 1662 – Klæbu (Utgått)<br />- 1663 – Malvik (Utgått)<br />- 1664 – Selbu (Utgått)<br />- 1665 – Tydal (Utgått)<br />- 1702 – Steinkjer (Utgått)<br />- 1703 – Namsos (Utgått)<br />- 1711 – Meråker (Utgått)<br />- 1714 – Stjørdal (Utgått)<br />- 1717 – Frosta (Utgått)<br />- 1718 – Leksvik (Utgått)<br />- 1719 – Levanger (Utgått)<br />- 1721 – Verdal (Utgått)<br />- 1723 – Mosvik (Utgått)<br />- 1724 – Verran (Utgått)<br />- 1725 – Namdalseid (Utgått)<br />- 1729 – Inderøy (Utgått)<br />- 1736 – Snåase – Snåsa (Utgått)<br />- 1738 – Lierne (Utgått)<br />- 1739 – Raarvihke – Røyrvik (Utgått)<br />- 1740 – Namsskogan (Utgått)<br />- 1742 – Grong (Utgått)<br />- 1743 – Høylandet (Utgått)<br />- 1744 – Overhalla (Utgått)<br />- 1748 – Fosnes (Utgått)<br />- 1749 – Flatanger (Utgått)<br />- 1750 – Vikna (Utgått)<br />- 1751 – Nærøy (Utgått)<br />- 1755 – Leka (Utgått)<br />- 1756 – Inderøy (Utgått)<br />- 1804 – Bodø<br />- 1805 – Narvik (Utgått 2020-01-01)<br />- 1806 – Narvik<br />- 1811 – Bindal<br />- 1812 – Sømna<br />- 1813 – Brønnøy<br />- 1815 – Vega<br />- 1816 – Vevelstad<br />- 1818 – Herøy i Nordland<br />- 1820 – Alstahaug<br />- 1822 – Leirfjord<br />- 1824 – Vefsn<br />- 1825 – Grane<br />- 1826 – Hattfjelldal<br />- 1827 – Dønna<br />- 1828 – Nesna<br />- 1832 – Hemnes<br />- 1833 – Rana<br />- 1834 – Lurøy<br />- 1835 – Træna<br />- 1836 – Rødøy<br />- 1837 – Meløy<br />- 1838 – Gildeskål<br />- 1839 – Beiarn<br />- 1840 – Saltdal<br />- 1841 – Fauske – Fuossko<br />- 1842 – Skjerstad (Utgått)<br />- 1845 – Sørfold<br />- 1848 – Steigen<br />- 1849 – Hamarøy – Hábmer (Utgått 2020-01-01)<br />- 1850 – Divtasvuodna – Tysfjord (Utgått 2020-01-01)<br />- 1851 – Lødingen<br />- 1852 – Tjeldsund (Utgått 2020-01-01)<br />- 1853 – Evenes<br />- 1854 – Ballangen (Utgått 2020-01-01)<br />- 1856 – Røst<br />- 1857 – Værøy<br />- 1859 – Flakstad<br />- 1860 – Vestvågøy<br />- 1865 – Vågan<br />- 1866 – Hadsel<br />- 1867 – Bø i Nordland<br />- 1868 – Øksnes<br />- 1870 – Sortland – Suortá<br />- 1871 – Andøy<br />- 1874 – Moskenes<br />- 1875 – Hamarøy – Hábmer<br />- 1901 – Harstad (Utgått)<br />- 1902 – Tromsø (Utgått 2020-01-01)<br />- 1903 – Harstad – Hárstták (Utgått 2020-01-01)<br />- 1911 – Kvæfjord (Utgått 2020-01-01)<br />- 1913 – Skånland (Utgått 2020-01-01)<br />- 1915 – Bjarkøy (Utgått)<br />- 1917 – Ibestad (Utgått 2020-01-01)<br />- 1919 – Gratangen (Utgått 2020-01-01)<br />- 1920 – Loabák – Lavangen (Utgått 2020-01-01)<br />- 1922 – Bardu (Utgått 2020-01-01)<br />- 1923 – Salangen (Utgått 2020-01-01)<br />- 1924 – Målselv (Utgått 2020-01-01)<br />- 1925 – Sørreisa (Utgått 2020-01-01)<br />- 1926 – Dyrøy (Utgått 2020-01-01)<br />- 1927 – Tranøy (Utgått 2020-01-01)<br />- 1928 – Torsken (Utgått 2020-01-01)<br />- 1929 – Berg (Utgått 2020-01-01)<br />- 1931 – Lenvik (Utgått 2020-01-01)<br />- 1933 – Balsfjord (Utgått 2020-01-01)<br />- 1936 – Karlsøy (Utgått 2020-01-01)<br />- 1938 – Lyngen (Utgått 2020-01-01)<br />- 1939 – Storfjord – Omasvuotna – Omasvuono (Utgått 2020-01-01)<br />- 1940 – Gáivuotna – Kåfjord – Kaivuono (Utgått 2020-01-01)<br />- 1941 – Skjervøy (Utgått 2020-01-01)<br />- 1942 – Nordreisa - Ráisa - Raisi  (Utgått 2020-01-01)<br />- 1943 – Kvænangen (Utgått 2020-01-01)<br />- 2001 – Hammerfest (Utgått)<br />- 2002 – Vardø (Utgått 2020-01-01)<br />- 2003 – Vadsø (Utgått 2020-01-01)<br />- 2004 – Hammerfest (Utgått 2020-01-01)<br />- 2011 – Guovdageaidnu – Kautokeino (Utgått 2020-01-01)<br />- 2012 – Alta (Utgått 2020-01-01)<br />- 2014 – Loppa (Utgått 2020-01-01)<br />- 2015 – Hasvik (Utgått 2020-01-01)<br />- 2016 – Sørøysund (Utgått)<br />- 2017 – Kvalsund (Utgått 2020-01-01)<br />- 2018 – Måsøy (Utgått 2020-01-01)<br />- 2019 – Nordkapp (Utgått 2020-01-01)<br />- 2020 – Porsanger – Porsáŋgu – Porsanki (Utgått 2020-01-01)<br />- 2021 – Kárášjohka – Karasjok  (Utgått 2020-01-01)<br />- 2022 – Lebesby (Utgått 2020-01-01)<br />- 2023 – Gamvik (Utgått 2020-01-01)<br />- 2024 – Berlevåg (Utgått 2020-01-01)<br />- 2025 – Deatnu – Tana (Utgått 2020-01-01)<br />- 2027 – Unjárga – Nesseby (Utgått 2020-01-01)<br />- 2028 – Båtsfjord (Utgått 2020-01-01)<br />- 2030 – Sør-Varanger (Utgått 2020-01-01)<br />- 3001 – Halden<br />- 3002 – Moss<br />- 3003 – Sarpsborg<br />- 3004 – Fredrikstad<br />- 3005 – Drammen<br />- 3006 – Kongsberg<br />- 3007 – Ringerike<br />- 3011 – Hvaler<br />- 3012 – Aremark<br />- 3013 – Marker<br />- 3014 – Indre Østfold<br />- 3015 – Skiptvet<br />- 3016 – Rakkestad<br />- 3017 – Råde<br />- 3018 – Våler i Viken<br />- 3019 – Vestby<br />- 3020 – Nordre Follo<br />- 3021 – Ås<br />- 3022 – Frogn<br />- 3023 – Nesodden<br />- 3024 – Bærum<br />- 3025 – Asker<br />- 3026 – Aurskog-Høland<br />- 3027 – Rælingen<br />- 3028 – Enebakk<br />- 3029 – Lørenskog<br />- 3030 – Lillestrøm<br />- 3031 – Nittedal<br />- 3032 – Gjerdrum<br />- 3033 – Ullensaker<br />- 3034 – Nes (tidligere Nes i Akershus)<br />- 3035 – Eidsvoll<br />- 3036 – Nannestad<br />- 3037 – Hurdal<br />- 3038 – Hole<br />- 3039 – Flå<br />- 3040 – Nesbyen (tidligere Nes i Buskerud)<br />- 3041 – Gol<br />- 3042 – Hemsedal<br />- 3043 – Ål<br />- 3044 – Hol<br />- 3045 – Sigdal<br />- 3046 – Krødsherad<br />- 3047 – Modum<br />- 3048 – Øvre Eiker<br />- 3049 – Lier<br />- 3050 – Flesberg<br />- 3051 – Rollag<br />- 3052 – Nore og Uvdal<br />- 3053 – Jevnaker<br />- 3054 – Lunner<br />- 3401 – Kongsvinger<br />- 3403 – Hamar<br />- 3405 – Lillehammer<br />- 3407 – Gjøvik<br />- 3411 – Ringsaker<br />- 3412 – Løten<br />- 3413 – Stange<br />- 3414 – Nord-Odal<br />- 3415 – Sør-Odal<br />- 3416 – Eidskog<br />- 3417 – Grue<br />- 3418 – Åsnes<br />- 3419 – Våler i Innlandet<br />- 3420 – Elverum<br />- 3421 – Trysil<br />- 3422 – Åmot<br />- 3423 – Stor-Elvdal<br />- 3424 – Rendalen<br />- 3425 – Engerdal<br />- 3426 – Tolga<br />- 3427 – Tynset<br />- 3428 – Alvdal<br />- 3429 – Folldal<br />- 3430 – Os<br />- 3431 – Dovre<br />- 3432 – Lesja<br />- 3433 – Skjåk<br />- 3434 – Lom<br />- 3435 – Vågå<br />- 3436 – Nord-Fron<br />- 3437 – Sel<br />- 3438 – Sør-Fron<br />- 3439 – Ringebu<br />- 3440 – Øyer<br />- 3441 – Gausdal<br />- 3442 – Østre Toten<br />- 3443 – Vestre Toten<br />- 3446 – Gran<br />- 3447 – Søndre Land<br />- 3448 – Nordre Land<br />- 3449 – Sør-Aurdal<br />- 3450 – Etnedal<br />- 3451 – Nord-Aurdal<br />- 3452 – Vestre Slidre<br />- 3453 – Øystre Slidre<br />- 3454 – Vang<br />- 3801 – Horten<br />- 3802 – Holmestrand<br />- 3803 – Tønsberg<br />- 3804 – Sandefjord<br />- 3805 – Larvik<br />- 3806 – Porsgrunn<br />- 3807 – Skien<br />- 3808 – Notodden<br />- 3811 – Færder<br />- 3812 – Siljan<br />- 3813 – Bamble<br />- 3814 – Kragerø<br />- 3815 – Drangedal<br />- 3816 – Nome<br />- 3817 – Midt-Telemark<br />- 3818 – Tinn<br />- 3819 – Hjartdal<br />- 3820 – Seljord<br />- 3821 – Kviteseid<br />- 3822 – Nissedal<br />- 3823 – Fyresdal<br />- 3824 – Tokke<br />- 3825 – Vinje<br />- 4201 – Risør<br />- 4202 – Grimstad<br />- 4203 – Arendal<br />- 4204 – Kristiansand<br />- 4205 – Lindesnes<br />- 4206 – Farsund<br />- 4207 – Flekkefjord<br />- 4211 – Gjerstad<br />- 4212 – Vegårshei<br />- 4213 – Tvedestrand<br />- 4214 – Froland<br />- 4215 – Lillesand<br />- 4216 – Birkenes<br />- 4217 – Åmli<br />- 4218 – Iveland<br />- 4219 – Evje og Hornnes<br />- 4220 – Bygland<br />- 4221 – Valle<br />- 4222 – Bykle<br />- 4223 – Vennesla<br />- 4224 – Åseral<br />- 4225 – Lyngdal<br />- 4226 – Hægebostad<br />- 4227 – Kvinesdal<br />- 4228 – Sirdal<br />- 4601 – Bergen<br />- 4602 – Kinn<br />- 4611 – Etne<br />- 4612 – Sveio<br />- 4613 – Bømlo<br />- 4614 – Stord<br />- 4615 – Fitjar<br />- 4616 – Tysnes<br />- 4617 – Kvinnherad<br />- 4618 – Ullensvang<br />- 4619 – Eidfjord<br />- 4620 – Ulvik<br />- 4621 – Voss<br />- 4622 – Kvam<br />- 4623 – Samnanger<br />- 4624 – Bjørnafjorden<br />- 4625 – Austevoll<br />- 4626 – Øygarden<br />- 4627 – Askøy<br />- 4628 – Vaksdal<br />- 4629 – Modalen<br />- 4630 – Osterøy<br />- 4631 – Alver<br />- 4632 – Austrheim<br />- 4633 – Fedje<br />- 4634 – Masfjorden<br />- 4635 – Gulen<br />- 4636 – Solund<br />- 4637 – Hyllestad<br />- 4638 – Høyanger<br />- 4639 – Vik<br />- 4640 – Sogndal<br />- 4641 – Aurland<br />- 4642 – Lærdal<br />- 4643 – Årdal<br />- 4644 – Luster<br />- 4645 – Askvoll<br />- 4646 – Fjaler<br />- 4647 – Sunnfjord<br />- 4648 – Bremanger<br />- 4649 – Stad<br />- 4650 – Gloppen<br />- 4651 – Stryn<br />- 5001 – Trondheim<br />- 5004 – Steinkjer (Utgått 2020-01-01)<br />- 5005 – Namsos (Utgått 2020-01-01)<br />- 5006 – Steinkjer<br />- 5007 – Namsos<br />- 5011 – Hemne (Utgått 2020-01-01)<br />- 5012 – Snillfjord (Utgått 2020-01-01)<br />- 5013 – Hitra (Utgått 2020-01-01)<br />- 5014 – Frøya<br />- 5015 – Ørland (Utgått 2020-01-01)<br />- 5016 – Agdenes (Utgått 2020-01-01)<br />- 5017 – Bjugn (Utgått 2020-01-01)<br />- 5018 – Åfjord (Utgått 2020-01-01)<br />- 5019 – Roan (Utgått 2020-01-01)<br />- 5020 – Osen<br />- 5021 – Oppdal<br />- 5022 – Rennebu<br />- 5023 – Meldal (Utgått 2020-01-01)<br />- 5024 – Orkdal (Utgått 2020-01-01)<br />- 5025 – Røros<br />- 5026 – Holtålen<br />- 5027 – Midtre Gauldal<br />- 5028 – Melhus<br />- 5029 – Skaun<br />- 5030 – Klæbu (Utgått 2020-01-01)<br />- 5031 – Malvik<br />- 5032 – Selbu<br />- 5033 – Tydal<br />- 5034 – Meråker<br />- 5035 – Stjørdal<br />- 5036 – Frosta<br />- 5037 – Levanger<br />- 5038 – Verdal<br />- 5039 – Verran (Utgått 2020-01-01)<br />- 5040 – Namdalseid (Utgått 2020-01-01)<br />- 5041 – Snåase – Snåsa<br />- 5042 – Lierne<br />- 5043 – Raarvikhe – Røyrvik<br />- 5044 – Namsskogan<br />- 5045 – Grong<br />- 5046 – Høylandet<br />- 5047 – Overhalla<br />- 5048 – Fosnes (Utgått 2020-01-01)<br />- 5049 – Flatanger<br />- 5050 – Vikna (Utgått 2020-01-01)<br />- 5051 – Nærøy (Utgått 2020-01-01)<br />- 5052 – Leka<br />- 5053 – Inderøy<br />- 5054 – Indre Fosen<br />- 5055 – Heim<br />- 5056 – Hitra<br />- 5057 – Ørland<br />- 5058 – Åfjord<br />- 5059 – Orkland<br />- 5060 – Nærøysund<br />- 5061 – Rindal<br />- 5401 – Tromsø<br />- 5402 – Harstad – Hárstták<br />- 5403 – Alta<br />- 5404 – Vardø<br />- 5405 – Vadsø<br />- 5406 – Hammerfest<br />- 5411 – Kvæfjord<br />- 5412 – Tjeldsund<br />- 5413 – Ibestad<br />- 5414 – Gratangen<br />- 5415 – Loabák - Lavangen<br />- 5416 – Bardu<br />- 5417 – Salangen<br />- 5418 – Målselv<br />- 5419 – Sørreisa<br />- 5420 – Dyrøy<br />- 5421 – Senja<br />- 5422 – Balsfjord<br />- 5423 – Karlsøy<br />- 5424 – Lyngen<br />- 5425 – Storfjord - Omasvuotna - Omasvuono<br />- 5426 – Gáivuotna - Kåfjord - Kaivuono<br />- 5427 – Skjervøy<br />- 5428 – Nordreisa - Ráisa - Raisi<br />- 5429 – Kvænangen<br />- 5430 – Guovdageaidnu - Kautokeino<br />- 5432 – Loppa<br />- 5433 – Hasvik<br />- 5434 – Måsøy<br />- 5435 – Nordkapp<br />- 5436 – Porsanger - Porsáŋgu - Porsanki<br />- 5437 – Kárášjohka - Karasjok<br />- 5438 – Lebesby<br />- 5439 – Gamvik<br />- 5440 – Berlevåg<br />- 5441 – Deatnu - Tana<br />- 5442 – Unjárga - Nesseby<br />- 5443 – Båtsfjord<br />- 5444 – Sør-Varanger<br />- 2100 – Svalbard</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>entydig identifisering av matrikkelenhet innen kommune, definert i matrikkelforskrift § 7e<br /><br />Merknad (teknisk): Hentes fra adresse (link til matrikkelenhet fra adresse i matrikkelen)</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Matrikkelnummer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse.kommunenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste<br /><br />Merknad: Det presiseres at kommune alltid skal ha 4 siffer, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 siffer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Kommunenummer</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer">http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer</a><br />- 0101 – Halden (Utgått 2020-01-01)<br />- 0102 – Sarpsborg (Utgått)<br />- 0103 – Fredrikstad (Utgått)<br />- 0104 – Moss (Utgått 2020-01-01)<br />- 0105 – Sarpsborg (Utgått 2020-01-01)<br />- 0106 – Fredrikstad (Utgått 2020-01-01)<br />- 0111 – Hvaler (Utgått 2020-01-01)<br />- 0113 – Borge (Utgått)<br />- 0114 – Varteig (Utgått)<br />- 0115 – Skjeberg (Utgått)<br />- 0118 – Aremark (Utgått 2020-01-01)<br />- 0119 – Marker (Utgått 2020-01-01)<br />- 0121 – Rømskog (Utgått 2020-01-01)<br />- 0122 – Trøgstad (Utgått 2020-01-01)<br />- 0123 – Spydeberg (Utgått 2020-01-01)<br />- 0124 – Askim (Utgått 2020-01-01)<br />- 0125 – Eidsberg (Utgått 2020-01-01)<br />- 0127 – Skiptvet (Utgått 2020-01-01)<br />- 0128 – Rakkestad (Utgått 2020-01-01)<br />- 0130 – Tune (Utgått)<br />- 0131 – Rolvsøy (Utgått)<br />- 0133 – Kråkerøy (Utgått)<br />- 0134 – Onsøy (Utgått)<br />- 0135 – Råde (Utgått 2020-01-01)<br />- 0136 – Rygge (Utgått 2020-01-01)<br />- 0137 – Våler i Østfold (Utgått 2020-01-01)<br />- 0138 – Hobøl (Utgått 2020-01-01)<br />- 0211 – Vestby (Utgått 2020-01-01)<br />- 0213 – Ski (Utgått 2020-01-01)<br />- 0214 – Ås (Utgått 2020-01-01)<br />- 0215 – Frogn (Utgått 2020-01-01)<br />- 0216 – Nesodden (Utgått 2020-01-01)<br />- 0217 – Oppegård (Utgått 2020-01-01)<br />- 0219 – Bærum (Utgått 2020-01-01)<br />- 0220 – Asker (Utgått 2020-01-01)<br />- 0221 – Aurskog-Høland (Utgått 2020-01-01)<br />- 0226 – Sørum (Utgått 2020-01-01)<br />- 0227 – Fet (Utgått 2020-01-01)<br />- 0228 – Rælingen (Utgått 2020-01-01)<br />- 0229 – Enebakk (Utgått 2020-01-01)<br />- 0230 – Lørenskog (Utgått 2020-01-01)<br />- 0231 – Skedsmo (Utgått 2020-01-01)<br />- 0233 – Nittedal (Utgått 2020-01-01)<br />- 0234 – Gjerdrum (Utgått 2020-01-01)<br />- 0235 – Ullensaker (Utgått 2020-01-01)<br />- 0236 – Nes i Akershus (Utgått 2020-01-01)<br />- 0237 – Eidsvoll (Utgått 2020-01-01)<br />- 0238 – Nannestad (Utgått 2020-01-01)<br />- 0239 – Hurdal (Utgått 2020-01-01)<br />- 0301 – Oslo<br />- 0401 – Hamar (Utgått)<br />- 0402 – Kongsvinger (Utgått 2020-01-01)<br />- 0403 – Hamar (Utgått 2020-01-01)<br />- 0412 – Ringsaker (Utgått 2020-01-01)<br />- 0414 – Vang (Utgått)<br />- 0415 – Løten (Utgått 2020-01-01)<br />- 0417 – Stange (Utgått 2020-01-01)<br />- 0418 – Nord-Odal (Utgått 2020-01-01)<br />- 0419 – Sør-Odal (Utgått 2020-01-01)<br />- 0420 – Eidskog (Utgått 2020-01-01)<br />- 0423 – Grue (Utgått 2020-01-01)<br />- 0425 – Åsnes (Utgått 2020-01-01)<br />- 0426 – Våler i Hedmark (Utgått 2020-01-01)<br />- 0427 – Elverum (Utgått 2020-01-01)<br />- 0428 – Trysil (Utgått 2020-01-01)<br />- 0429 – Åmot (Utgått 2020-01-01)<br />- 0430 – Stor-Elvdal (Utgått 2020-01-01)<br />- 0432 – Rendalen (Utgått 2020-01-01)<br />- 0434 – Engerdal (Utgått 2020-01-01)<br />- 0436 – Tolga (Utgått 2020-01-01)<br />- 0437 – Tynset (Utgått 2020-01-01)<br />- 0438 – Alvdal (Utgått 2020-01-01)<br />- 0439 – Folldal (Utgått 2020-01-01)<br />- 0441 – Os i Hedmark (Utgått 2020-01-01)<br />- 0501 – Lillehammer (Utgått 2020-01-01)<br />- 0502 – Gjøvik (Utgått 2020-01-01)<br />- 0511 – Dovre (Utgått 2020-01-01)<br />- 0512 – Lesja (Utgått 2020-01-01)<br />- 0513 – Skjåk (Utgått 2020-01-01)<br />- 0514 – Lom (Utgått 2020-01-01)<br />- 0515 – Vågå (Utgått 2020-01-01)<br />- 0516 – Nord-Fron (Utgått 2020-01-01)<br />- 0517 – Sel (Utgått 2020-01-01)<br />- 0519 – Sør-Fron (Utgått 2020-01-01)<br />- 0520 – Ringebu (Utgått 2020-01-01)<br />- 0521 – Øyer (Utgått 2020-01-01)<br />- 0522 – Gausdal (Utgått 2020-01-01)<br />- 0528 – Østre Toten (Utgått 2020-01-01)<br />- 0529 – Vestre Toten (Utgått 2020-01-01)<br />- 0532 – Jevnaker (Utgått 2020-01-01)<br />- 0533 – Lunner (Utgått 2020-01-01)<br />- 0534 – Gran (Utgått 2020-01-01)<br />- 0536 – Søndre Land (Utgått 2020-01-01)<br />- 0538 – Nordre Land (Utgått 2020-01-01)<br />- 0540 – Sør-Aurdal (Utgått 2020-01-01)<br />- 0541 – Etnedal (Utgått 2020-01-01)<br />- 0542 – Nord-Aurdal (Utgått 2020-01-01)<br />- 0543 – Vestre Slidre (Utgått 2020-01-01)<br />- 0544 – Øystre Slidre (Utgått 2020-01-01)<br />- 0545 – Vang (Utgått 2020-01-01)<br />- 0602 – Drammen (Utgått 2020-01-01)<br />- 0604 – Kongsberg (Utgått 2020-01-01)<br />- 0605 – Ringerike (Utgått 2020-01-01)<br />- 0612 – Hole (Utgått 2020-01-01)<br />- 0615 – Flå (Utgått 2020-01-01)<br />- 0616 – Nes i Buskerud (Utgått 2020-01-01)<br />- 0617 – Gol (Utgått 2020-01-01)<br />- 0618 – Hemsedal (Utgått 2020-01-01)<br />- 0619 – Ål (Utgått 2020-01-01)<br />- 0620 – Hol (Utgått 2020-01-01)<br />- 0621 – Sigdal (Utgått 2020-01-01)<br />- 0622 – Krødsherad (Utgått 2020-01-01)<br />- 0623 – Modum (Utgått 2020-01-01)<br />- 0624 – Øvre Eiker (Utgått 2020-01-01)<br />- 0625 – Nedre Eiker (Utgått 2020-01-01)<br />- 0626 – Lier (Utgått 2020-01-01)<br />- 0627 – Røyken (Utgått 2020-01-01)<br />- 0628 – Hurum (Utgått 2020-01-01)<br />- 0631 – Flesberg (Utgått 2020-01-01)<br />- 0632 – Rollag (Utgått 2020-01-01)<br />- 0633 – Nore og Uvdal (Utgått 2020-01-01)<br />- 0701 – Horten (Utgått 2020-01-01)<br />- 0702 – Holmestrand (Utgått)<br />- 0703 – Horten (Utgått)<br />- 0704 – Tønsberg (Utgått 2020-01-01)<br />- 0705 – Tønsberg (Utgått)<br />- 0706 – Sandefjord (Utgått)<br />- 0707 – Larvik (Utgått)<br />- 0708 – Stavern (Utgått)<br />- 0709 – Larvik (Utgått)<br />- 0710 – Sandefjord (Utgått 2020-01-01)<br />- 0711 – Svelvik (Utgått 2020-01-01)<br />- 0712 – Larvik (Utgått 2020-01-01)<br />- 0713 – Sande i Vestfold (Utgått 2020-01-01)<br />- 0714 – Hof (Utgått)<br />- 0715 – Holmestrand (Utgått 2020-01-01)<br />- 0716 – Re (Utgått 2020-01-01)<br />- 0717 – Borre (Utgått)<br />- 0718 – Ramnes (Utgått)<br />- 0719 – Andebu (Utgått)<br />- 0720 – Stokke (Utgått)<br />- 0721 – Sem (Utgått)<br />- 0722 – Nøtterøy (Utgått)<br />- 0723 – Tjøme (Utgått)<br />- 0725 – Tjølling (Utgått)<br />- 0726 – Brunlanes (Utgått)<br />- 0727 – Hedrum (Utgått)<br />- 0728 – Lardal (Utgått)<br />- 0729 – Færder (Utgått 2020-01-01)<br />- 0805 – Porsgrunn (Utgått 2020-01-01)<br />- 0806 – Skien (Utgått 2020-01-01)<br />- 0807 – Notodden (Utgått 2020-01-01)<br />- 0811 – Siljan (Utgått 2020-01-01)<br />- 0814 – Bamble (Utgått 2020-01-01)<br />- 0815 – Kragerø (Utgått 2020-01-01)<br />- 0817 – Drangedal (Utgått 2020-01-01)<br />- 0819 – Nome (Utgått 2020-01-01)<br />- 0821 – Bø i Telemark (Utgått 2020-01-01)<br />- 0822 – Sauherad (Utgått 2020-01-01)<br />- 0826 – Tinn (Utgått 2020-01-01)<br />- 0827 – Hjartdal (Utgått 2020-01-01)<br />- 0828 – Seljord (Utgått 2020-01-01)<br />- 0829 – Kviteseid (Utgått 2020-01-01)<br />- 0830 – Nissedal (Utgått 2020-01-01)<br />- 0831 – Fyresdal (Utgått 2020-01-01)<br />- 0833 – Tokke (Utgått 2020-01-01)<br />- 0834 – Vinje (Utgått 2020-01-01)<br />- 0901 – Risør (Utgått 2020-01-01)<br />- 0903 – Arendal (Utgått)<br />- 0904 – Grimstad (Utgått 2020-01-01)<br />- 0906 – Arendal (Utgått 2020-01-01)<br />- 0911 – Gjerstad (Utgått 2020-01-01)<br />- 0912 – Vegårshei (Utgått 2020-01-01)<br />- 0914 – Tvedestrand (Utgått 2020-01-01)<br />- 0918 – Moland (Utgått)<br />- 0919 – Froland (Utgått 2020-01-01)<br />- 0920 – Øyestad (Utgått)<br />- 0921 – Tromøy (Utgått)<br />- 0922 – Hisøy (Utgått)<br />- 0926 – Lillesand (Utgått 2020-01-01)<br />- 0928 – Birkenes (Utgått 2020-01-01)<br />- 0929 – Åmli (Utgått 2020-01-01)<br />- 0935 – Iveland (Utgått 2020-01-01)<br />- 0937 – Evje og Hornnes (Utgått 2020-01-01)<br />- 0938 – Bygland (Utgått 2020-01-01)<br />- 0940 – Valle (Utgått 2020-01-01)<br />- 0941 – Bykle (Utgått 2020-01-01)<br />- 1001 – Kristiansand (Utgått 2020-01-01)<br />- 1002 – Mandal (Utgått 2020-01-01)<br />- 1003 – Farsund (Utgått 2020-01-01)<br />- 1004 – Flekkefjord (Utgått 2020-01-01)<br />- 1014 – Vennesla (Utgått 2020-01-01)<br />- 1017 – Songdalen (Utgått 2020-01-01)<br />- 1018 – Søgne (Utgått 2020-01-01)<br />- 1021 – Marnardal (Utgått 2020-01-01)<br />- 1026 – Åseral (Utgått 2020-01-01)<br />- 1027 – Audnedal (Utgått 2020-01-01)<br />- 1029 – Lindesnes (Utgått 2020-01-01)<br />- 1032 – Lyngdal (Utgått 2020-01-01)<br />- 1034 – Hægebostad (Utgått 2020-01-01)<br />- 1037 – Kvinesdal (Utgått 2020-01-01)<br />- 1046 – Sirdal (Utgått 2020-01-01)<br />- 1101 – Eigersund<br />- 1102 – Sandnes (Utgått 2020-01-01)<br />- 1103 – Stavanger<br />- 1106 – Haugesund<br />- 1108 – Sandnes<br />- 1111 – Sokndal<br />- 1112 – Lund<br />- 1114 – Bjerkreim<br />- 1119 – Hå<br />- 1120 – Klepp<br />- 1121 – Time<br />- 1122 – Gjesdal<br />- 1124 – Sola<br />- 1127 – Randaberg<br />- 1129 – Forsand (Utgått 2020-01-01)<br />- 1130 – Strand<br />- 1133 – Hjelmeland<br />- 1134 – Suldal<br />- 1135 – Sauda<br />- 1141 – Finnøy (Utgått 2020-01-01)<br />- 1142 – Rennesøy (Utgått 2020-01-01)<br />- 1144 – Kvitsøy<br />- 1145 – Bokn<br />- 1146 – Tysvær<br />- 1149 – Karmøy<br />- 1151 – Utsira<br />- 1154 – Vindafjord (Utgått)<br />- 1159 – Ølen (Utgått)<br />- 1160 – Vindafjord<br />- 1201 – Bergen (Utgått 2020-01-01)<br />- 1211 – Etne (Utgått 2020-01-01)<br />- 1214 – Ølen (Utgått)<br />- 1216 – Sveio (Utgått 2020-01-01)<br />- 1219 – Bømlo (Utgått 2020-01-01)<br />- 1221 – Stord (Utgått 2020-01-01)<br />- 1222 – Fitjar (Utgått 2020-01-01)<br />- 1223 – Tysnes (Utgått 2020-01-01)<br />- 1224 – Kvinnherad (Utgått 2020-01-01)<br />- 1227 – Jondal (Utgått 2020-01-01)<br />- 1228 – Odda (Utgått 2020-01-01)<br />- 1231 – Ullensvang (Utgått 2020-01-01)<br />- 1232 – Eidfjord (Utgått 2020-01-01)<br />- 1233 – Ulvik (Utgått 2020-01-01)<br />- 1234 – Granvin (Utgått 2020-01-01)<br />- 1235 – Voss (Utgått 2020-01-01)<br />- 1238 – Kvam (Utgått 2020-01-01)<br />- 1241 – Fusa (Utgått 2020-01-01)<br />- 1242 – Samnanger (Utgått 2020-01-01)<br />- 1243 – Os i Hordaland (Utgått 2020-01-01)<br />- 1244 – Austevoll (Utgått 2020-01-01)<br />- 1245 – Sund (Utgått 2020-01-01)<br />- 1246 – Fjell (Utgått 2020-01-01)<br />- 1247 – Askøy (Utgått 2020-01-01)<br />- 1251 – Vaksdal (Utgått 2020-01-01)<br />- 1252 – Modalen (Utgått 2020-01-01)<br />- 1253 – Osterøy (Utgått 2020-01-01)<br />- 1256 – Meland (Utgått 2020-01-01)<br />- 1259 – Øygarden (Utgått 2020-01-01)<br />- 1260 – Radøy (Utgått 2020-01-01)<br />- 1263 – Lindås (Utgått 2020-01-01)<br />- 1264 – Austrheim (Utgått 2020-01-01)<br />- 1265 – Fedje (Utgått 2020-01-01)<br />- 1266 – Masfjorden (Utgått 2020-01-01)<br />- 1401 – Flora (Utgått 2020-01-01)<br />- 1411 – Gulen (Utgått 2020-01-01)<br />- 1412 – Solund (Utgått 2020-01-01)<br />- 1413 – Hyllestad (Utgått 2020-01-01)<br />- 1416 – Høyanger (Utgått 2020-01-01)<br />- 1417 – Vik (Utgått 2020-01-01)<br />- 1418 – Balestrand (Utgått 2020-01-01)<br />- 1419 – Leikanger (Utgått 2020-01-01)<br />- 1420 – Sogndal (Utgått 2020-01-01)<br />- 1421 – Aurland (Utgått 2020-01-01)<br />- 1422 – Lærdal (Utgått 2020-01-01)<br />- 1424 – Årdal (Utgått 2020-01-01)<br />- 1426 – Luster (Utgått 2020-01-01)<br />- 1428 – Askvoll (Utgått 2020-01-01)<br />- 1429 – Fjaler (Utgått 2020-01-01)<br />- 1430 – Gaular (Utgått 2020-01-01)<br />- 1431 – Jølster (Utgått 2020-01-01)<br />- 1432 – Førde (Utgått 2020-01-01)<br />- 1433 – Naustdal (Utgått 2020-01-01)<br />- 1438 – Bremanger (Utgått 2020-01-01)<br />- 1439 – Vågsøy (Utgått 2020-01-01)<br />- 1441 – Selje (Utgått 2020-01-01)<br />- 1443 – Eid (Utgått 2020-01-01)<br />- 1444 – Hornindal (Utgått 2020-01-01)<br />- 1445 – Gloppen (Utgått 2020-01-01)<br />- 1449 – Stryn (Utgått 2020-01-01)<br />- 1502 – Molde (Utgått 2020-01-01)<br />- 1504 – Ålesund (Utgått 2020-01-01)<br />- 1505 – Kristiansund<br />- 1506 – Molde<br />- 1507 – Ålesund<br />- 1511 – Vanylven<br />- 1514 – Sande i Møre og Romsdal<br />- 1515 – Herøy i Møre og Romsdal<br />- 1516 – Ulstein<br />- 1517 – Hareid<br />- 1519 – Volda (Utgått 2020-01-01)<br />- 1520 – Ørsta<br />- 1523 – Ørskog (Utgått 2020-01-01)<br />- 1524 – Norddal (Utgått 2020-01-01)<br />- 1525 – Stranda<br />- 1526 – Stordal (Utgått 2020-01-01)<br />- 1528 – Sykkylven<br />- 1529 – Skodje (Utgått 2020-01-01)<br />- 1531 – Sula<br />- 1532 – Giske<br />- 1534 – Haram (Utgått 2020-01-01)<br />- 1535 – Vestnes<br />- 1539 – Rauma<br />- 1543 – Nesset (Utgått 2020-01-01)<br />- 1545 – Midsund (Utgått 2020-01-01)<br />- 1546 – Sandøy (Utgått 2020-01-01)<br />- 1547 – Aukra<br />- 1548 – Fræna (Utgått 2020-01-01)<br />- 1551 – Eide (Utgått 2020-01-01)<br />- 1554 – Averøy<br />- 1557 – Gjemnes<br />- 1560 – Tingvoll<br />- 1563 – Sunndal<br />- 1566 – Surnadal<br />- 1567 – Rindal (Utgått)<br />- 1569 – Aure (Utgått)<br />- 1571 – Halsa (Utgått 2020-01-01)<br />- 1572 – Tustna (Utgått)<br />- 1573 – Smøla<br />- 1576 – Aure<br />- 1577 – Volda<br />- 1578 – Fjord<br />- 1579 – Hustadvika<br />- 1601 – Trondheim (Utgått)<br />- 1612 – Hemne (Utgått)<br />- 1613 – Snillfjord (Utgått)<br />- 1617 – Hitra (Utgått)<br />- 1620 – Frøya (Utgått)<br />- 1621 – Ørland (Utgått)<br />- 1622 – Agdenes (Utgått)<br />- 1624 – Rissa (Utgått)<br />- 1627 – Bjugn (Utgått)<br />- 1630 – Åfjord (Utgått)<br />- 1632 – Roan (Utgått)<br />- 1633 – Osen (Utgått)<br />- 1634 – Oppdal (Utgått)<br />- 1635 – Rennebu (Utgått)<br />- 1636 – Meldal (Utgått)<br />- 1638 – Orkdal (Utgått)<br />- 1640 – Røros (Utgått)<br />- 1644 – Holtålen (Utgått)<br />- 1648 – Midtre Gauldal (Utgått)<br />- 1653 – Melhus (Utgått)<br />- 1657 – Skaun (Utgått)<br />- 1662 – Klæbu (Utgått)<br />- 1663 – Malvik (Utgått)<br />- 1664 – Selbu (Utgått)<br />- 1665 – Tydal (Utgått)<br />- 1702 – Steinkjer (Utgått)<br />- 1703 – Namsos (Utgått)<br />- 1711 – Meråker (Utgått)<br />- 1714 – Stjørdal (Utgått)<br />- 1717 – Frosta (Utgått)<br />- 1718 – Leksvik (Utgått)<br />- 1719 – Levanger (Utgått)<br />- 1721 – Verdal (Utgått)<br />- 1723 – Mosvik (Utgått)<br />- 1724 – Verran (Utgått)<br />- 1725 – Namdalseid (Utgått)<br />- 1729 – Inderøy (Utgått)<br />- 1736 – Snåase – Snåsa (Utgått)<br />- 1738 – Lierne (Utgått)<br />- 1739 – Raarvihke – Røyrvik (Utgått)<br />- 1740 – Namsskogan (Utgått)<br />- 1742 – Grong (Utgått)<br />- 1743 – Høylandet (Utgått)<br />- 1744 – Overhalla (Utgått)<br />- 1748 – Fosnes (Utgått)<br />- 1749 – Flatanger (Utgått)<br />- 1750 – Vikna (Utgått)<br />- 1751 – Nærøy (Utgått)<br />- 1755 – Leka (Utgått)<br />- 1756 – Inderøy (Utgått)<br />- 1804 – Bodø<br />- 1805 – Narvik (Utgått 2020-01-01)<br />- 1806 – Narvik<br />- 1811 – Bindal<br />- 1812 – Sømna<br />- 1813 – Brønnøy<br />- 1815 – Vega<br />- 1816 – Vevelstad<br />- 1818 – Herøy i Nordland<br />- 1820 – Alstahaug<br />- 1822 – Leirfjord<br />- 1824 – Vefsn<br />- 1825 – Grane<br />- 1826 – Hattfjelldal<br />- 1827 – Dønna<br />- 1828 – Nesna<br />- 1832 – Hemnes<br />- 1833 – Rana<br />- 1834 – Lurøy<br />- 1835 – Træna<br />- 1836 – Rødøy<br />- 1837 – Meløy<br />- 1838 – Gildeskål<br />- 1839 – Beiarn<br />- 1840 – Saltdal<br />- 1841 – Fauske – Fuossko<br />- 1842 – Skjerstad (Utgått)<br />- 1845 – Sørfold<br />- 1848 – Steigen<br />- 1849 – Hamarøy – Hábmer (Utgått 2020-01-01)<br />- 1850 – Divtasvuodna – Tysfjord (Utgått 2020-01-01)<br />- 1851 – Lødingen<br />- 1852 – Tjeldsund (Utgått 2020-01-01)<br />- 1853 – Evenes<br />- 1854 – Ballangen (Utgått 2020-01-01)<br />- 1856 – Røst<br />- 1857 – Værøy<br />- 1859 – Flakstad<br />- 1860 – Vestvågøy<br />- 1865 – Vågan<br />- 1866 – Hadsel<br />- 1867 – Bø i Nordland<br />- 1868 – Øksnes<br />- 1870 – Sortland – Suortá<br />- 1871 – Andøy<br />- 1874 – Moskenes<br />- 1875 – Hamarøy – Hábmer<br />- 1901 – Harstad (Utgått)<br />- 1902 – Tromsø (Utgått 2020-01-01)<br />- 1903 – Harstad – Hárstták (Utgått 2020-01-01)<br />- 1911 – Kvæfjord (Utgått 2020-01-01)<br />- 1913 – Skånland (Utgått 2020-01-01)<br />- 1915 – Bjarkøy (Utgått)<br />- 1917 – Ibestad (Utgått 2020-01-01)<br />- 1919 – Gratangen (Utgått 2020-01-01)<br />- 1920 – Loabák – Lavangen (Utgått 2020-01-01)<br />- 1922 – Bardu (Utgått 2020-01-01)<br />- 1923 – Salangen (Utgått 2020-01-01)<br />- 1924 – Målselv (Utgått 2020-01-01)<br />- 1925 – Sørreisa (Utgått 2020-01-01)<br />- 1926 – Dyrøy (Utgått 2020-01-01)<br />- 1927 – Tranøy (Utgått 2020-01-01)<br />- 1928 – Torsken (Utgått 2020-01-01)<br />- 1929 – Berg (Utgått 2020-01-01)<br />- 1931 – Lenvik (Utgått 2020-01-01)<br />- 1933 – Balsfjord (Utgått 2020-01-01)<br />- 1936 – Karlsøy (Utgått 2020-01-01)<br />- 1938 – Lyngen (Utgått 2020-01-01)<br />- 1939 – Storfjord – Omasvuotna – Omasvuono (Utgått 2020-01-01)<br />- 1940 – Gáivuotna – Kåfjord – Kaivuono (Utgått 2020-01-01)<br />- 1941 – Skjervøy (Utgått 2020-01-01)<br />- 1942 – Nordreisa - Ráisa - Raisi  (Utgått 2020-01-01)<br />- 1943 – Kvænangen (Utgått 2020-01-01)<br />- 2001 – Hammerfest (Utgått)<br />- 2002 – Vardø (Utgått 2020-01-01)<br />- 2003 – Vadsø (Utgått 2020-01-01)<br />- 2004 – Hammerfest (Utgått 2020-01-01)<br />- 2011 – Guovdageaidnu – Kautokeino (Utgått 2020-01-01)<br />- 2012 – Alta (Utgått 2020-01-01)<br />- 2014 – Loppa (Utgått 2020-01-01)<br />- 2015 – Hasvik (Utgått 2020-01-01)<br />- 2016 – Sørøysund (Utgått)<br />- 2017 – Kvalsund (Utgått 2020-01-01)<br />- 2018 – Måsøy (Utgått 2020-01-01)<br />- 2019 – Nordkapp (Utgått 2020-01-01)<br />- 2020 – Porsanger – Porsáŋgu – Porsanki (Utgått 2020-01-01)<br />- 2021 – Kárášjohka – Karasjok  (Utgått 2020-01-01)<br />- 2022 – Lebesby (Utgått 2020-01-01)<br />- 2023 – Gamvik (Utgått 2020-01-01)<br />- 2024 – Berlevåg (Utgått 2020-01-01)<br />- 2025 – Deatnu – Tana (Utgått 2020-01-01)<br />- 2027 – Unjárga – Nesseby (Utgått 2020-01-01)<br />- 2028 – Båtsfjord (Utgått 2020-01-01)<br />- 2030 – Sør-Varanger (Utgått 2020-01-01)<br />- 3001 – Halden<br />- 3002 – Moss<br />- 3003 – Sarpsborg<br />- 3004 – Fredrikstad<br />- 3005 – Drammen<br />- 3006 – Kongsberg<br />- 3007 – Ringerike<br />- 3011 – Hvaler<br />- 3012 – Aremark<br />- 3013 – Marker<br />- 3014 – Indre Østfold<br />- 3015 – Skiptvet<br />- 3016 – Rakkestad<br />- 3017 – Råde<br />- 3018 – Våler i Viken<br />- 3019 – Vestby<br />- 3020 – Nordre Follo<br />- 3021 – Ås<br />- 3022 – Frogn<br />- 3023 – Nesodden<br />- 3024 – Bærum<br />- 3025 – Asker<br />- 3026 – Aurskog-Høland<br />- 3027 – Rælingen<br />- 3028 – Enebakk<br />- 3029 – Lørenskog<br />- 3030 – Lillestrøm<br />- 3031 – Nittedal<br />- 3032 – Gjerdrum<br />- 3033 – Ullensaker<br />- 3034 – Nes (tidligere Nes i Akershus)<br />- 3035 – Eidsvoll<br />- 3036 – Nannestad<br />- 3037 – Hurdal<br />- 3038 – Hole<br />- 3039 – Flå<br />- 3040 – Nesbyen (tidligere Nes i Buskerud)<br />- 3041 – Gol<br />- 3042 – Hemsedal<br />- 3043 – Ål<br />- 3044 – Hol<br />- 3045 – Sigdal<br />- 3046 – Krødsherad<br />- 3047 – Modum<br />- 3048 – Øvre Eiker<br />- 3049 – Lier<br />- 3050 – Flesberg<br />- 3051 – Rollag<br />- 3052 – Nore og Uvdal<br />- 3053 – Jevnaker<br />- 3054 – Lunner<br />- 3401 – Kongsvinger<br />- 3403 – Hamar<br />- 3405 – Lillehammer<br />- 3407 – Gjøvik<br />- 3411 – Ringsaker<br />- 3412 – Løten<br />- 3413 – Stange<br />- 3414 – Nord-Odal<br />- 3415 – Sør-Odal<br />- 3416 – Eidskog<br />- 3417 – Grue<br />- 3418 – Åsnes<br />- 3419 – Våler i Innlandet<br />- 3420 – Elverum<br />- 3421 – Trysil<br />- 3422 – Åmot<br />- 3423 – Stor-Elvdal<br />- 3424 – Rendalen<br />- 3425 – Engerdal<br />- 3426 – Tolga<br />- 3427 – Tynset<br />- 3428 – Alvdal<br />- 3429 – Folldal<br />- 3430 – Os<br />- 3431 – Dovre<br />- 3432 – Lesja<br />- 3433 – Skjåk<br />- 3434 – Lom<br />- 3435 – Vågå<br />- 3436 – Nord-Fron<br />- 3437 – Sel<br />- 3438 – Sør-Fron<br />- 3439 – Ringebu<br />- 3440 – Øyer<br />- 3441 – Gausdal<br />- 3442 – Østre Toten<br />- 3443 – Vestre Toten<br />- 3446 – Gran<br />- 3447 – Søndre Land<br />- 3448 – Nordre Land<br />- 3449 – Sør-Aurdal<br />- 3450 – Etnedal<br />- 3451 – Nord-Aurdal<br />- 3452 – Vestre Slidre<br />- 3453 – Øystre Slidre<br />- 3454 – Vang<br />- 3801 – Horten<br />- 3802 – Holmestrand<br />- 3803 – Tønsberg<br />- 3804 – Sandefjord<br />- 3805 – Larvik<br />- 3806 – Porsgrunn<br />- 3807 – Skien<br />- 3808 – Notodden<br />- 3811 – Færder<br />- 3812 – Siljan<br />- 3813 – Bamble<br />- 3814 – Kragerø<br />- 3815 – Drangedal<br />- 3816 – Nome<br />- 3817 – Midt-Telemark<br />- 3818 – Tinn<br />- 3819 – Hjartdal<br />- 3820 – Seljord<br />- 3821 – Kviteseid<br />- 3822 – Nissedal<br />- 3823 – Fyresdal<br />- 3824 – Tokke<br />- 3825 – Vinje<br />- 4201 – Risør<br />- 4202 – Grimstad<br />- 4203 – Arendal<br />- 4204 – Kristiansand<br />- 4205 – Lindesnes<br />- 4206 – Farsund<br />- 4207 – Flekkefjord<br />- 4211 – Gjerstad<br />- 4212 – Vegårshei<br />- 4213 – Tvedestrand<br />- 4214 – Froland<br />- 4215 – Lillesand<br />- 4216 – Birkenes<br />- 4217 – Åmli<br />- 4218 – Iveland<br />- 4219 – Evje og Hornnes<br />- 4220 – Bygland<br />- 4221 – Valle<br />- 4222 – Bykle<br />- 4223 – Vennesla<br />- 4224 – Åseral<br />- 4225 – Lyngdal<br />- 4226 – Hægebostad<br />- 4227 – Kvinesdal<br />- 4228 – Sirdal<br />- 4601 – Bergen<br />- 4602 – Kinn<br />- 4611 – Etne<br />- 4612 – Sveio<br />- 4613 – Bømlo<br />- 4614 – Stord<br />- 4615 – Fitjar<br />- 4616 – Tysnes<br />- 4617 – Kvinnherad<br />- 4618 – Ullensvang<br />- 4619 – Eidfjord<br />- 4620 – Ulvik<br />- 4621 – Voss<br />- 4622 – Kvam<br />- 4623 – Samnanger<br />- 4624 – Bjørnafjorden<br />- 4625 – Austevoll<br />- 4626 – Øygarden<br />- 4627 – Askøy<br />- 4628 – Vaksdal<br />- 4629 – Modalen<br />- 4630 – Osterøy<br />- 4631 – Alver<br />- 4632 – Austrheim<br />- 4633 – Fedje<br />- 4634 – Masfjorden<br />- 4635 – Gulen<br />- 4636 – Solund<br />- 4637 – Hyllestad<br />- 4638 – Høyanger<br />- 4639 – Vik<br />- 4640 – Sogndal<br />- 4641 – Aurland<br />- 4642 – Lærdal<br />- 4643 – Årdal<br />- 4644 – Luster<br />- 4645 – Askvoll<br />- 4646 – Fjaler<br />- 4647 – Sunnfjord<br />- 4648 – Bremanger<br />- 4649 – Stad<br />- 4650 – Gloppen<br />- 4651 – Stryn<br />- 5001 – Trondheim<br />- 5004 – Steinkjer (Utgått 2020-01-01)<br />- 5005 – Namsos (Utgått 2020-01-01)<br />- 5006 – Steinkjer<br />- 5007 – Namsos<br />- 5011 – Hemne (Utgått 2020-01-01)<br />- 5012 – Snillfjord (Utgått 2020-01-01)<br />- 5013 – Hitra (Utgått 2020-01-01)<br />- 5014 – Frøya<br />- 5015 – Ørland (Utgått 2020-01-01)<br />- 5016 – Agdenes (Utgått 2020-01-01)<br />- 5017 – Bjugn (Utgått 2020-01-01)<br />- 5018 – Åfjord (Utgått 2020-01-01)<br />- 5019 – Roan (Utgått 2020-01-01)<br />- 5020 – Osen<br />- 5021 – Oppdal<br />- 5022 – Rennebu<br />- 5023 – Meldal (Utgått 2020-01-01)<br />- 5024 – Orkdal (Utgått 2020-01-01)<br />- 5025 – Røros<br />- 5026 – Holtålen<br />- 5027 – Midtre Gauldal<br />- 5028 – Melhus<br />- 5029 – Skaun<br />- 5030 – Klæbu (Utgått 2020-01-01)<br />- 5031 – Malvik<br />- 5032 – Selbu<br />- 5033 – Tydal<br />- 5034 – Meråker<br />- 5035 – Stjørdal<br />- 5036 – Frosta<br />- 5037 – Levanger<br />- 5038 – Verdal<br />- 5039 – Verran (Utgått 2020-01-01)<br />- 5040 – Namdalseid (Utgått 2020-01-01)<br />- 5041 – Snåase – Snåsa<br />- 5042 – Lierne<br />- 5043 – Raarvikhe – Røyrvik<br />- 5044 – Namsskogan<br />- 5045 – Grong<br />- 5046 – Høylandet<br />- 5047 – Overhalla<br />- 5048 – Fosnes (Utgått 2020-01-01)<br />- 5049 – Flatanger<br />- 5050 – Vikna (Utgått 2020-01-01)<br />- 5051 – Nærøy (Utgått 2020-01-01)<br />- 5052 – Leka<br />- 5053 – Inderøy<br />- 5054 – Indre Fosen<br />- 5055 – Heim<br />- 5056 – Hitra<br />- 5057 – Ørland<br />- 5058 – Åfjord<br />- 5059 – Orkland<br />- 5060 – Nærøysund<br />- 5061 – Rindal<br />- 5401 – Tromsø<br />- 5402 – Harstad – Hárstták<br />- 5403 – Alta<br />- 5404 – Vardø<br />- 5405 – Vadsø<br />- 5406 – Hammerfest<br />- 5411 – Kvæfjord<br />- 5412 – Tjeldsund<br />- 5413 – Ibestad<br />- 5414 – Gratangen<br />- 5415 – Loabák - Lavangen<br />- 5416 – Bardu<br />- 5417 – Salangen<br />- 5418 – Målselv<br />- 5419 – Sørreisa<br />- 5420 – Dyrøy<br />- 5421 – Senja<br />- 5422 – Balsfjord<br />- 5423 – Karlsøy<br />- 5424 – Lyngen<br />- 5425 – Storfjord - Omasvuotna - Omasvuono<br />- 5426 – Gáivuotna - Kåfjord - Kaivuono<br />- 5427 – Skjervøy<br />- 5428 – Nordreisa - Ráisa - Raisi<br />- 5429 – Kvænangen<br />- 5430 – Guovdageaidnu - Kautokeino<br />- 5432 – Loppa<br />- 5433 – Hasvik<br />- 5434 – Måsøy<br />- 5435 – Nordkapp<br />- 5436 – Porsanger - Porsáŋgu - Porsanki<br />- 5437 – Kárášjohka - Karasjok<br />- 5438 – Lebesby<br />- 5439 – Gamvik<br />- 5440 – Berlevåg<br />- 5441 – Deatnu - Tana<br />- 5442 – Unjárga - Nesseby<br />- 5443 – Båtsfjord<br />- 5444 – Sør-Varanger<br />- 2100 – Svalbard</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse.gardsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>En kommune er delt inn i flere gårder, og alle matrikkelenheter ligger på en gårdsenhet. Gårdsnummer er nummeret på en gårdsenhet i matrikkelen og er unikt innenfor hver kommune. Forkortelsen er gnr</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse.bruksnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Hver gård er delt opp i et eller flere bruk. Neste ledige bruksnummer innen et gårdsnummer tildeles automatisk. Forkortelsen er bnr</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse.festenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Fortløpende nummerering av fester under gårdsnummer/bruksnummer. Forkortelsen er fnr</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>matrikkelnummerAdresse.seksjonsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Fortløpende nummerering av seksjoner under gårdsnummer/bruksnummer og eventuelt festenummer.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>postnummerområde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>adressens knytning til postnummerområde, geografisk område med felles postnummer, og en underinndeling av postområde</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>PostnummerområdeId</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>postnummerområde.postnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>firesifret kode som identifiserer et postnummerområde<br /><br />Merknad: Det første sifferet angir postsone, de to første sifrene angir postregion, de tre første sifrene angir postområde og alle fire sifrene angir postnummerområde/poststed.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>postnummerområde.poststed</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på poststed i henhold til Postens egne lister</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>representasjonspunkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Representasjonspunkt for adressen. Angir normalt atkomsten til en bygning, bolig eller andre objekter og steder.<br /><br />Merknad:<br />Dersom en adresse kun gjelder en bygning med en adresse, plasseres punktet innenfor bygningens omriss like ved inngang /atkomst.<br />Det samme gjelder dersom det er knyttet flere adresser til flere innganger/atkomster til en bygning. Adressepunktene plasseres like ved de respektive innganger/atkomster innenfor bygningens omriss. For bygg med altangang eller svalgang med atkomst til den enkelte bolig via utvendig atkomsttrapp, plasseres adressepunktet i trapp nærmest terrengnivå<br /><br />For ubebygde eiendommer verifiseres det at punktet er innenfor teigen og ved atkomst.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Punkt</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sokn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>adressens kobling til sokn, den minste geistlige enheten og bestyres av en sokneprest<br /><br />Merknad:<br />Folket som er medlem i Den norske kirke og bosatt innenfor et sokn betegnes som menighet.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>SokneId</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sokn.soknenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik identifikasjon av et sokn i form av 8-sifre<br /><br />Merknad:<br />De to første siffer står for bispedømme, to neste for prosti, to neste for prestegjeld (utgått, men inngår i nummerering) og to siste for sokn.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sokn.organisasjonsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>entydig identifisering av foretak i Brønnøysundregisteret</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Integer</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>sokn.soknenavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på soknet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>tettsted</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>adressens tilknytning til tettsted, område hvor det bor minst 200 personer, og avstanden mellom husene normalt ikke overstiger 50 meter (SSB)<br /><br />Merknad:<br />Hussamlinger som naturlig  hører med til tettstedet, tas med inntil en avstand på 400 meter fra tettstedskjernen.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TettstedId</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>tettsted.tettstednummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>består av en 4-sifret kode<br /><br />Merknad: Det skal benyttes ledende nuller.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>tettsted.tettstednavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på tettsted bestemt av SSB</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>uuidAdresse</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Objektidentifikator realisert som UUID forvaltet av matrikkelsystemet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>valgkrets</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>adressens knytning til valgkrets, valgkretsene har som formål å være en hensiktsmessig inndeling av kommuner ved valg, bl.a. for at velgerne ikke skal få for stor avstand til valglokalet<br /><br />Merknad: Inndelingen skal ivareta administrative formål, men har også i en viss grad blitt nyttet til å samle inn statistikk for planleggingsformål.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>ValgkretsId</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>valgkrets.valgkretsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>løpenummer innenfor valgkretsens kommune</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>valgkrets.valgkretsnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn til valgkrets</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>uuidAtkomst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Kobling til atkomst i Matrikkelen (Atkomstens id realisert som UUID i matrikkelsystemet)<br /><br />Merknad:<br />UUID på Atkomst er ikke innført i Matrikkelen, men vil komme</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..*</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>CharacterString</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt-Adresse

**Assosiasjoner**
Atkomst – rolle: atkomstpunkt – kardinalitet: 0..*

### Kodelister

#### «Enumeration» TypeAtkomst

**Definisjon:** ulike atkomster i forhold til årstid (f.eks ikke vinterbrøytede veger). Senere kan en tenke seg å utvide med atkomst vareleveranse osv

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>atkomst</td>
      <td>generell atkomst, uavhengig av årstid</td>
      <td></td>
    </tr>
    <tr>
      <td>atkomstSommer</td>
      <td>atkomst sommerstid. Kan være en annen enn atkomst vinterstid pga ikke brøytede veger, båt-trafikk eller annet</td>
      <td></td>
    </tr>
    <tr>
      <td>atkomstVinter</td>
      <td>atkomst vinterstid. Kan være en annen enn atkomst sommersstid pga ikke brøytede veger, båt-trafikk eller annet</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» AdressetilleggsnavnKildeKode

**Definisjon:** Kodeliste over opphav til adressetilleggsnavn, som også er årsaken til at de er registrert i matrikkelen.

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>krevdAvEier</td>
      <td>&lt;font color="#333333"&gt;Når adressen gjelder et gårdsbruk, kan den som har grunnbokshjemmel til eiendommen som eier, kreve at den offisielle adressen også skal omfatte gårdens bruksnavn, dersom navnet faller språklig og geografisk sammen med et nedarvet stedsnavn, jf. lov 18. mai 1990 nr. 11 om stadnamn (&lt;/font&gt;matrikkelforskriftens § 54 1. ledd)</td>
      <td></td>
    </tr>
    <tr>
      <td>anmodetAvHjemmelshaver</td>
      <td>&lt;font color="#333333"&gt;Når adressen gjelder en særlig kjent institusjon eller bygning og allmenne hensyn taler for det, kan kommunen på anmodning fra registrert eier fastsette at den offisielle adressen også skal omfatte et navn på institusjonen eller bygningen (&lt;/font&gt;matrikkelforskriftens § 54 2. ledd)</td>
      <td></td>
    </tr>
    <tr>
      <td>matrikkeladressenavn</td>
      <td>&lt;font color="#333333"&gt;Adresser i område med matrikkeladresser som ikke har tildelt et adressetilleggsnavn etter reglene i § 54, kan tilordnes et matrikkeladressenavn etter &lt;/font&gt;matrikkelforskriftens § 55 3. ledd. Hvis det tildeles adressetilleggsnavn etter § 54 strykes matrikkeladressenavnet</td>
      <td></td>
    </tr>
    <tr>
      <td>ikkeOppgitt</td>
      <td>"Ikke oppgitt" brukes på adresser uten adressetilleggsnavn.</td>
      <td></td>
    </tr>
    <tr>
      <td>tildeltAvKommunen</td>
      <td>&lt;font color="#333333"&gt;Kommunen kan tildele adresser innenfor mindre grender, bolig- eller hyttefelt eller andre avgrensede områder et felles adressetilleggsnavn (&lt;/font&gt;Matrikkelforskriftens § 54 3. ledd, men tildeling etter 1. eller 2. ledd går foran 3. ledd)</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Kommunenummer

**Definisjon:** nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste samt et utvalg av utgåtte numre
Merknad: Det presiseres at kommune alltid skal ha 4 sifre, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 sifre.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>false</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer">http://skjema.geonorge.no/SOSI/kodeliste/AdmEnheter/2020/Kommunenummer</a></td>
    </tr>
  </tbody>
</table>

Koder

<table class="code-list-table">
  <thead>
    <tr>
      <th>Kodenavn:</th>
      <th>Definisjon:</th>
      <th>Kodeverdi:</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td></td>
      <td>Halden (Utgått 2020-01-01)</td>
      <td>0101</td>
    </tr>
    <tr>
      <td></td>
      <td>Sarpsborg (Utgått)</td>
      <td>0102</td>
    </tr>
    <tr>
      <td></td>
      <td>Fredrikstad (Utgått)</td>
      <td>0103</td>
    </tr>
    <tr>
      <td></td>
      <td>Moss (Utgått 2020-01-01)</td>
      <td>0104</td>
    </tr>
    <tr>
      <td></td>
      <td>Sarpsborg (Utgått 2020-01-01)</td>
      <td>0105</td>
    </tr>
    <tr>
      <td></td>
      <td>Fredrikstad (Utgått 2020-01-01)</td>
      <td>0106</td>
    </tr>
    <tr>
      <td></td>
      <td>Hvaler (Utgått 2020-01-01)</td>
      <td>0111</td>
    </tr>
    <tr>
      <td></td>
      <td>Borge (Utgått)</td>
      <td>0113</td>
    </tr>
    <tr>
      <td></td>
      <td>Varteig (Utgått)</td>
      <td>0114</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjeberg (Utgått)</td>
      <td>0115</td>
    </tr>
    <tr>
      <td></td>
      <td>Aremark (Utgått 2020-01-01)</td>
      <td>0118</td>
    </tr>
    <tr>
      <td></td>
      <td>Marker (Utgått 2020-01-01)</td>
      <td>0119</td>
    </tr>
    <tr>
      <td></td>
      <td>Rømskog (Utgått 2020-01-01)</td>
      <td>0121</td>
    </tr>
    <tr>
      <td></td>
      <td>Trøgstad (Utgått 2020-01-01)</td>
      <td>0122</td>
    </tr>
    <tr>
      <td></td>
      <td>Spydeberg (Utgått 2020-01-01)</td>
      <td>0123</td>
    </tr>
    <tr>
      <td></td>
      <td>Askim (Utgått 2020-01-01)</td>
      <td>0124</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidsberg (Utgått 2020-01-01)</td>
      <td>0125</td>
    </tr>
    <tr>
      <td></td>
      <td>Skiptvet (Utgått 2020-01-01)</td>
      <td>0127</td>
    </tr>
    <tr>
      <td></td>
      <td>Rakkestad (Utgått 2020-01-01)</td>
      <td>0128</td>
    </tr>
    <tr>
      <td></td>
      <td>Tune (Utgått)</td>
      <td>0130</td>
    </tr>
    <tr>
      <td></td>
      <td>Rolvsøy (Utgått)</td>
      <td>0131</td>
    </tr>
    <tr>
      <td></td>
      <td>Kråkerøy (Utgått)</td>
      <td>0133</td>
    </tr>
    <tr>
      <td></td>
      <td>Onsøy (Utgått)</td>
      <td>0134</td>
    </tr>
    <tr>
      <td></td>
      <td>Råde (Utgått 2020-01-01)</td>
      <td>0135</td>
    </tr>
    <tr>
      <td></td>
      <td>Rygge (Utgått 2020-01-01)</td>
      <td>0136</td>
    </tr>
    <tr>
      <td></td>
      <td>Våler i Østfold (Utgått 2020-01-01)</td>
      <td>0137</td>
    </tr>
    <tr>
      <td></td>
      <td>Hobøl (Utgått 2020-01-01)</td>
      <td>0138</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestby (Utgått 2020-01-01)</td>
      <td>0211</td>
    </tr>
    <tr>
      <td></td>
      <td>Ski (Utgått 2020-01-01)</td>
      <td>0213</td>
    </tr>
    <tr>
      <td></td>
      <td>Ås (Utgått 2020-01-01)</td>
      <td>0214</td>
    </tr>
    <tr>
      <td></td>
      <td>Frogn (Utgått 2020-01-01)</td>
      <td>0215</td>
    </tr>
    <tr>
      <td></td>
      <td>Nesodden (Utgått 2020-01-01)</td>
      <td>0216</td>
    </tr>
    <tr>
      <td></td>
      <td>Oppegård (Utgått 2020-01-01)</td>
      <td>0217</td>
    </tr>
    <tr>
      <td></td>
      <td>Bærum (Utgått 2020-01-01)</td>
      <td>0219</td>
    </tr>
    <tr>
      <td></td>
      <td>Asker (Utgått 2020-01-01)</td>
      <td>0220</td>
    </tr>
    <tr>
      <td></td>
      <td>Aurskog-Høland (Utgått 2020-01-01)</td>
      <td>0221</td>
    </tr>
    <tr>
      <td></td>
      <td>Sørum (Utgått 2020-01-01)</td>
      <td>0226</td>
    </tr>
    <tr>
      <td></td>
      <td>Fet (Utgått 2020-01-01)</td>
      <td>0227</td>
    </tr>
    <tr>
      <td></td>
      <td>Rælingen (Utgått 2020-01-01)</td>
      <td>0228</td>
    </tr>
    <tr>
      <td></td>
      <td>Enebakk (Utgått 2020-01-01)</td>
      <td>0229</td>
    </tr>
    <tr>
      <td></td>
      <td>Lørenskog (Utgått 2020-01-01)</td>
      <td>0230</td>
    </tr>
    <tr>
      <td></td>
      <td>Skedsmo (Utgått 2020-01-01)</td>
      <td>0231</td>
    </tr>
    <tr>
      <td></td>
      <td>Nittedal (Utgått 2020-01-01)</td>
      <td>0233</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjerdrum (Utgått 2020-01-01)</td>
      <td>0234</td>
    </tr>
    <tr>
      <td></td>
      <td>Ullensaker (Utgått 2020-01-01)</td>
      <td>0235</td>
    </tr>
    <tr>
      <td></td>
      <td>Nes i Akershus (Utgått 2020-01-01)</td>
      <td>0236</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidsvoll (Utgått 2020-01-01)</td>
      <td>0237</td>
    </tr>
    <tr>
      <td></td>
      <td>Nannestad (Utgått 2020-01-01)</td>
      <td>0238</td>
    </tr>
    <tr>
      <td></td>
      <td>Hurdal (Utgått 2020-01-01)</td>
      <td>0239</td>
    </tr>
    <tr>
      <td></td>
      <td>Oslo</td>
      <td>0301</td>
    </tr>
    <tr>
      <td></td>
      <td>Hamar (Utgått)</td>
      <td>0401</td>
    </tr>
    <tr>
      <td></td>
      <td>Kongsvinger (Utgått 2020-01-01)</td>
      <td>0402</td>
    </tr>
    <tr>
      <td></td>
      <td>Hamar (Utgått 2020-01-01)</td>
      <td>0403</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringsaker (Utgått 2020-01-01)</td>
      <td>0412</td>
    </tr>
    <tr>
      <td></td>
      <td>Vang (Utgått)</td>
      <td>0414</td>
    </tr>
    <tr>
      <td></td>
      <td>Løten (Utgått 2020-01-01)</td>
      <td>0415</td>
    </tr>
    <tr>
      <td></td>
      <td>Stange (Utgått 2020-01-01)</td>
      <td>0417</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Odal (Utgått 2020-01-01)</td>
      <td>0418</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Odal (Utgått 2020-01-01)</td>
      <td>0419</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidskog (Utgått 2020-01-01)</td>
      <td>0420</td>
    </tr>
    <tr>
      <td></td>
      <td>Grue (Utgått 2020-01-01)</td>
      <td>0423</td>
    </tr>
    <tr>
      <td></td>
      <td>Åsnes (Utgått 2020-01-01)</td>
      <td>0425</td>
    </tr>
    <tr>
      <td></td>
      <td>Våler i Hedmark (Utgått 2020-01-01)</td>
      <td>0426</td>
    </tr>
    <tr>
      <td></td>
      <td>Elverum (Utgått 2020-01-01)</td>
      <td>0427</td>
    </tr>
    <tr>
      <td></td>
      <td>Trysil (Utgått 2020-01-01)</td>
      <td>0428</td>
    </tr>
    <tr>
      <td></td>
      <td>Åmot (Utgått 2020-01-01)</td>
      <td>0429</td>
    </tr>
    <tr>
      <td></td>
      <td>Stor-Elvdal (Utgått 2020-01-01)</td>
      <td>0430</td>
    </tr>
    <tr>
      <td></td>
      <td>Rendalen (Utgått 2020-01-01)</td>
      <td>0432</td>
    </tr>
    <tr>
      <td></td>
      <td>Engerdal (Utgått 2020-01-01)</td>
      <td>0434</td>
    </tr>
    <tr>
      <td></td>
      <td>Tolga (Utgått 2020-01-01)</td>
      <td>0436</td>
    </tr>
    <tr>
      <td></td>
      <td>Tynset (Utgått 2020-01-01)</td>
      <td>0437</td>
    </tr>
    <tr>
      <td></td>
      <td>Alvdal (Utgått 2020-01-01)</td>
      <td>0438</td>
    </tr>
    <tr>
      <td></td>
      <td>Folldal (Utgått 2020-01-01)</td>
      <td>0439</td>
    </tr>
    <tr>
      <td></td>
      <td>Os i Hedmark (Utgått 2020-01-01)</td>
      <td>0441</td>
    </tr>
    <tr>
      <td></td>
      <td>Lillehammer (Utgått 2020-01-01)</td>
      <td>0501</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjøvik (Utgått 2020-01-01)</td>
      <td>0502</td>
    </tr>
    <tr>
      <td></td>
      <td>Dovre (Utgått 2020-01-01)</td>
      <td>0511</td>
    </tr>
    <tr>
      <td></td>
      <td>Lesja (Utgått 2020-01-01)</td>
      <td>0512</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjåk (Utgått 2020-01-01)</td>
      <td>0513</td>
    </tr>
    <tr>
      <td></td>
      <td>Lom (Utgått 2020-01-01)</td>
      <td>0514</td>
    </tr>
    <tr>
      <td></td>
      <td>Vågå (Utgått 2020-01-01)</td>
      <td>0515</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Fron (Utgått 2020-01-01)</td>
      <td>0516</td>
    </tr>
    <tr>
      <td></td>
      <td>Sel (Utgått 2020-01-01)</td>
      <td>0517</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Fron (Utgått 2020-01-01)</td>
      <td>0519</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringebu (Utgått 2020-01-01)</td>
      <td>0520</td>
    </tr>
    <tr>
      <td></td>
      <td>Øyer (Utgått 2020-01-01)</td>
      <td>0521</td>
    </tr>
    <tr>
      <td></td>
      <td>Gausdal (Utgått 2020-01-01)</td>
      <td>0522</td>
    </tr>
    <tr>
      <td></td>
      <td>Østre Toten (Utgått 2020-01-01)</td>
      <td>0528</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestre Toten (Utgått 2020-01-01)</td>
      <td>0529</td>
    </tr>
    <tr>
      <td></td>
      <td>Jevnaker (Utgått 2020-01-01)</td>
      <td>0532</td>
    </tr>
    <tr>
      <td></td>
      <td>Lunner (Utgått 2020-01-01)</td>
      <td>0533</td>
    </tr>
    <tr>
      <td></td>
      <td>Gran (Utgått 2020-01-01)</td>
      <td>0534</td>
    </tr>
    <tr>
      <td></td>
      <td>Søndre Land (Utgått 2020-01-01)</td>
      <td>0536</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordre Land (Utgått 2020-01-01)</td>
      <td>0538</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Aurdal (Utgått 2020-01-01)</td>
      <td>0540</td>
    </tr>
    <tr>
      <td></td>
      <td>Etnedal (Utgått 2020-01-01)</td>
      <td>0541</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Aurdal (Utgått 2020-01-01)</td>
      <td>0542</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestre Slidre (Utgått 2020-01-01)</td>
      <td>0543</td>
    </tr>
    <tr>
      <td></td>
      <td>Øystre Slidre (Utgått 2020-01-01)</td>
      <td>0544</td>
    </tr>
    <tr>
      <td></td>
      <td>Vang (Utgått 2020-01-01)</td>
      <td>0545</td>
    </tr>
    <tr>
      <td></td>
      <td>Drammen (Utgått 2020-01-01)</td>
      <td>0602</td>
    </tr>
    <tr>
      <td></td>
      <td>Kongsberg (Utgått 2020-01-01)</td>
      <td>0604</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringerike (Utgått 2020-01-01)</td>
      <td>0605</td>
    </tr>
    <tr>
      <td></td>
      <td>Hole (Utgått 2020-01-01)</td>
      <td>0612</td>
    </tr>
    <tr>
      <td></td>
      <td>Flå (Utgått 2020-01-01)</td>
      <td>0615</td>
    </tr>
    <tr>
      <td></td>
      <td>Nes i Buskerud (Utgått 2020-01-01)</td>
      <td>0616</td>
    </tr>
    <tr>
      <td></td>
      <td>Gol (Utgått 2020-01-01)</td>
      <td>0617</td>
    </tr>
    <tr>
      <td></td>
      <td>Hemsedal (Utgått 2020-01-01)</td>
      <td>0618</td>
    </tr>
    <tr>
      <td></td>
      <td>Ål (Utgått 2020-01-01)</td>
      <td>0619</td>
    </tr>
    <tr>
      <td></td>
      <td>Hol (Utgått 2020-01-01)</td>
      <td>0620</td>
    </tr>
    <tr>
      <td></td>
      <td>Sigdal (Utgått 2020-01-01)</td>
      <td>0621</td>
    </tr>
    <tr>
      <td></td>
      <td>Krødsherad (Utgått 2020-01-01)</td>
      <td>0622</td>
    </tr>
    <tr>
      <td></td>
      <td>Modum (Utgått 2020-01-01)</td>
      <td>0623</td>
    </tr>
    <tr>
      <td></td>
      <td>Øvre Eiker (Utgått 2020-01-01)</td>
      <td>0624</td>
    </tr>
    <tr>
      <td></td>
      <td>Nedre Eiker (Utgått 2020-01-01)</td>
      <td>0625</td>
    </tr>
    <tr>
      <td></td>
      <td>Lier (Utgått 2020-01-01)</td>
      <td>0626</td>
    </tr>
    <tr>
      <td></td>
      <td>Røyken (Utgått 2020-01-01)</td>
      <td>0627</td>
    </tr>
    <tr>
      <td></td>
      <td>Hurum (Utgått 2020-01-01)</td>
      <td>0628</td>
    </tr>
    <tr>
      <td></td>
      <td>Flesberg (Utgått 2020-01-01)</td>
      <td>0631</td>
    </tr>
    <tr>
      <td></td>
      <td>Rollag (Utgått 2020-01-01)</td>
      <td>0632</td>
    </tr>
    <tr>
      <td></td>
      <td>Nore og Uvdal (Utgått 2020-01-01)</td>
      <td>0633</td>
    </tr>
    <tr>
      <td></td>
      <td>Horten (Utgått 2020-01-01)</td>
      <td>0701</td>
    </tr>
    <tr>
      <td></td>
      <td>Holmestrand (Utgått)</td>
      <td>0702</td>
    </tr>
    <tr>
      <td></td>
      <td>Horten (Utgått)</td>
      <td>0703</td>
    </tr>
    <tr>
      <td></td>
      <td>Tønsberg (Utgått 2020-01-01)</td>
      <td>0704</td>
    </tr>
    <tr>
      <td></td>
      <td>Tønsberg (Utgått)</td>
      <td>0705</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandefjord (Utgått)</td>
      <td>0706</td>
    </tr>
    <tr>
      <td></td>
      <td>Larvik (Utgått)</td>
      <td>0707</td>
    </tr>
    <tr>
      <td></td>
      <td>Stavern (Utgått)</td>
      <td>0708</td>
    </tr>
    <tr>
      <td></td>
      <td>Larvik (Utgått)</td>
      <td>0709</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandefjord (Utgått 2020-01-01)</td>
      <td>0710</td>
    </tr>
    <tr>
      <td></td>
      <td>Svelvik (Utgått 2020-01-01)</td>
      <td>0711</td>
    </tr>
    <tr>
      <td></td>
      <td>Larvik (Utgått 2020-01-01)</td>
      <td>0712</td>
    </tr>
    <tr>
      <td></td>
      <td>Sande i Vestfold (Utgått 2020-01-01)</td>
      <td>0713</td>
    </tr>
    <tr>
      <td></td>
      <td>Hof (Utgått)</td>
      <td>0714</td>
    </tr>
    <tr>
      <td></td>
      <td>Holmestrand (Utgått 2020-01-01)</td>
      <td>0715</td>
    </tr>
    <tr>
      <td></td>
      <td>Re (Utgått 2020-01-01)</td>
      <td>0716</td>
    </tr>
    <tr>
      <td></td>
      <td>Borre (Utgått)</td>
      <td>0717</td>
    </tr>
    <tr>
      <td></td>
      <td>Ramnes (Utgått)</td>
      <td>0718</td>
    </tr>
    <tr>
      <td></td>
      <td>Andebu (Utgått)</td>
      <td>0719</td>
    </tr>
    <tr>
      <td></td>
      <td>Stokke (Utgått)</td>
      <td>0720</td>
    </tr>
    <tr>
      <td></td>
      <td>Sem (Utgått)</td>
      <td>0721</td>
    </tr>
    <tr>
      <td></td>
      <td>Nøtterøy (Utgått)</td>
      <td>0722</td>
    </tr>
    <tr>
      <td></td>
      <td>Tjøme (Utgått)</td>
      <td>0723</td>
    </tr>
    <tr>
      <td></td>
      <td>Tjølling (Utgått)</td>
      <td>0725</td>
    </tr>
    <tr>
      <td></td>
      <td>Brunlanes (Utgått)</td>
      <td>0726</td>
    </tr>
    <tr>
      <td></td>
      <td>Hedrum (Utgått)</td>
      <td>0727</td>
    </tr>
    <tr>
      <td></td>
      <td>Lardal (Utgått)</td>
      <td>0728</td>
    </tr>
    <tr>
      <td></td>
      <td>Færder (Utgått 2020-01-01)</td>
      <td>0729</td>
    </tr>
    <tr>
      <td></td>
      <td>Porsgrunn (Utgått 2020-01-01)</td>
      <td>0805</td>
    </tr>
    <tr>
      <td></td>
      <td>Skien (Utgått 2020-01-01)</td>
      <td>0806</td>
    </tr>
    <tr>
      <td></td>
      <td>Notodden (Utgått 2020-01-01)</td>
      <td>0807</td>
    </tr>
    <tr>
      <td></td>
      <td>Siljan (Utgått 2020-01-01)</td>
      <td>0811</td>
    </tr>
    <tr>
      <td></td>
      <td>Bamble (Utgått 2020-01-01)</td>
      <td>0814</td>
    </tr>
    <tr>
      <td></td>
      <td>Kragerø (Utgått 2020-01-01)</td>
      <td>0815</td>
    </tr>
    <tr>
      <td></td>
      <td>Drangedal (Utgått 2020-01-01)</td>
      <td>0817</td>
    </tr>
    <tr>
      <td></td>
      <td>Nome (Utgått 2020-01-01)</td>
      <td>0819</td>
    </tr>
    <tr>
      <td></td>
      <td>Bø i Telemark (Utgått 2020-01-01)</td>
      <td>0821</td>
    </tr>
    <tr>
      <td></td>
      <td>Sauherad (Utgått 2020-01-01)</td>
      <td>0822</td>
    </tr>
    <tr>
      <td></td>
      <td>Tinn (Utgått 2020-01-01)</td>
      <td>0826</td>
    </tr>
    <tr>
      <td></td>
      <td>Hjartdal (Utgått 2020-01-01)</td>
      <td>0827</td>
    </tr>
    <tr>
      <td></td>
      <td>Seljord (Utgått 2020-01-01)</td>
      <td>0828</td>
    </tr>
    <tr>
      <td></td>
      <td>Kviteseid (Utgått 2020-01-01)</td>
      <td>0829</td>
    </tr>
    <tr>
      <td></td>
      <td>Nissedal (Utgått 2020-01-01)</td>
      <td>0830</td>
    </tr>
    <tr>
      <td></td>
      <td>Fyresdal (Utgått 2020-01-01)</td>
      <td>0831</td>
    </tr>
    <tr>
      <td></td>
      <td>Tokke (Utgått 2020-01-01)</td>
      <td>0833</td>
    </tr>
    <tr>
      <td></td>
      <td>Vinje (Utgått 2020-01-01)</td>
      <td>0834</td>
    </tr>
    <tr>
      <td></td>
      <td>Risør (Utgått 2020-01-01)</td>
      <td>0901</td>
    </tr>
    <tr>
      <td></td>
      <td>Arendal (Utgått)</td>
      <td>0903</td>
    </tr>
    <tr>
      <td></td>
      <td>Grimstad (Utgått 2020-01-01)</td>
      <td>0904</td>
    </tr>
    <tr>
      <td></td>
      <td>Arendal (Utgått 2020-01-01)</td>
      <td>0906</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjerstad (Utgått 2020-01-01)</td>
      <td>0911</td>
    </tr>
    <tr>
      <td></td>
      <td>Vegårshei (Utgått 2020-01-01)</td>
      <td>0912</td>
    </tr>
    <tr>
      <td></td>
      <td>Tvedestrand (Utgått 2020-01-01)</td>
      <td>0914</td>
    </tr>
    <tr>
      <td></td>
      <td>Moland (Utgått)</td>
      <td>0918</td>
    </tr>
    <tr>
      <td></td>
      <td>Froland (Utgått 2020-01-01)</td>
      <td>0919</td>
    </tr>
    <tr>
      <td></td>
      <td>Øyestad (Utgått)</td>
      <td>0920</td>
    </tr>
    <tr>
      <td></td>
      <td>Tromøy (Utgått)</td>
      <td>0921</td>
    </tr>
    <tr>
      <td></td>
      <td>Hisøy (Utgått)</td>
      <td>0922</td>
    </tr>
    <tr>
      <td></td>
      <td>Lillesand (Utgått 2020-01-01)</td>
      <td>0926</td>
    </tr>
    <tr>
      <td></td>
      <td>Birkenes (Utgått 2020-01-01)</td>
      <td>0928</td>
    </tr>
    <tr>
      <td></td>
      <td>Åmli (Utgått 2020-01-01)</td>
      <td>0929</td>
    </tr>
    <tr>
      <td></td>
      <td>Iveland (Utgått 2020-01-01)</td>
      <td>0935</td>
    </tr>
    <tr>
      <td></td>
      <td>Evje og Hornnes (Utgått 2020-01-01)</td>
      <td>0937</td>
    </tr>
    <tr>
      <td></td>
      <td>Bygland (Utgått 2020-01-01)</td>
      <td>0938</td>
    </tr>
    <tr>
      <td></td>
      <td>Valle (Utgått 2020-01-01)</td>
      <td>0940</td>
    </tr>
    <tr>
      <td></td>
      <td>Bykle (Utgått 2020-01-01)</td>
      <td>0941</td>
    </tr>
    <tr>
      <td></td>
      <td>Kristiansand (Utgått 2020-01-01)</td>
      <td>1001</td>
    </tr>
    <tr>
      <td></td>
      <td>Mandal (Utgått 2020-01-01)</td>
      <td>1002</td>
    </tr>
    <tr>
      <td></td>
      <td>Farsund (Utgått 2020-01-01)</td>
      <td>1003</td>
    </tr>
    <tr>
      <td></td>
      <td>Flekkefjord (Utgått 2020-01-01)</td>
      <td>1004</td>
    </tr>
    <tr>
      <td></td>
      <td>Vennesla (Utgått 2020-01-01)</td>
      <td>1014</td>
    </tr>
    <tr>
      <td></td>
      <td>Songdalen (Utgått 2020-01-01)</td>
      <td>1017</td>
    </tr>
    <tr>
      <td></td>
      <td>Søgne (Utgått 2020-01-01)</td>
      <td>1018</td>
    </tr>
    <tr>
      <td></td>
      <td>Marnardal (Utgått 2020-01-01)</td>
      <td>1021</td>
    </tr>
    <tr>
      <td></td>
      <td>Åseral (Utgått 2020-01-01)</td>
      <td>1026</td>
    </tr>
    <tr>
      <td></td>
      <td>Audnedal (Utgått 2020-01-01)</td>
      <td>1027</td>
    </tr>
    <tr>
      <td></td>
      <td>Lindesnes (Utgått 2020-01-01)</td>
      <td>1029</td>
    </tr>
    <tr>
      <td></td>
      <td>Lyngdal (Utgått 2020-01-01)</td>
      <td>1032</td>
    </tr>
    <tr>
      <td></td>
      <td>Hægebostad (Utgått 2020-01-01)</td>
      <td>1034</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvinesdal (Utgått 2020-01-01)</td>
      <td>1037</td>
    </tr>
    <tr>
      <td></td>
      <td>Sirdal (Utgått 2020-01-01)</td>
      <td>1046</td>
    </tr>
    <tr>
      <td></td>
      <td>Eigersund</td>
      <td>1101</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandnes (Utgått 2020-01-01)</td>
      <td>1102</td>
    </tr>
    <tr>
      <td></td>
      <td>Stavanger</td>
      <td>1103</td>
    </tr>
    <tr>
      <td></td>
      <td>Haugesund</td>
      <td>1106</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandnes</td>
      <td>1108</td>
    </tr>
    <tr>
      <td></td>
      <td>Sokndal</td>
      <td>1111</td>
    </tr>
    <tr>
      <td></td>
      <td>Lund</td>
      <td>1112</td>
    </tr>
    <tr>
      <td></td>
      <td>Bjerkreim</td>
      <td>1114</td>
    </tr>
    <tr>
      <td></td>
      <td>Hå</td>
      <td>1119</td>
    </tr>
    <tr>
      <td></td>
      <td>Klepp</td>
      <td>1120</td>
    </tr>
    <tr>
      <td></td>
      <td>Time</td>
      <td>1121</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjesdal</td>
      <td>1122</td>
    </tr>
    <tr>
      <td></td>
      <td>Sola</td>
      <td>1124</td>
    </tr>
    <tr>
      <td></td>
      <td>Randaberg</td>
      <td>1127</td>
    </tr>
    <tr>
      <td></td>
      <td>Forsand (Utgått 2020-01-01)</td>
      <td>1129</td>
    </tr>
    <tr>
      <td></td>
      <td>Strand</td>
      <td>1130</td>
    </tr>
    <tr>
      <td></td>
      <td>Hjelmeland</td>
      <td>1133</td>
    </tr>
    <tr>
      <td></td>
      <td>Suldal</td>
      <td>1134</td>
    </tr>
    <tr>
      <td></td>
      <td>Sauda</td>
      <td>1135</td>
    </tr>
    <tr>
      <td></td>
      <td>Finnøy (Utgått 2020-01-01)</td>
      <td>1141</td>
    </tr>
    <tr>
      <td></td>
      <td>Rennesøy (Utgått 2020-01-01)</td>
      <td>1142</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvitsøy</td>
      <td>1144</td>
    </tr>
    <tr>
      <td></td>
      <td>Bokn</td>
      <td>1145</td>
    </tr>
    <tr>
      <td></td>
      <td>Tysvær</td>
      <td>1146</td>
    </tr>
    <tr>
      <td></td>
      <td>Karmøy</td>
      <td>1149</td>
    </tr>
    <tr>
      <td></td>
      <td>Utsira</td>
      <td>1151</td>
    </tr>
    <tr>
      <td></td>
      <td>Vindafjord (Utgått)</td>
      <td>1154</td>
    </tr>
    <tr>
      <td></td>
      <td>Ølen (Utgått)</td>
      <td>1159</td>
    </tr>
    <tr>
      <td></td>
      <td>Vindafjord</td>
      <td>1160</td>
    </tr>
    <tr>
      <td></td>
      <td>Bergen (Utgått 2020-01-01)</td>
      <td>1201</td>
    </tr>
    <tr>
      <td></td>
      <td>Etne (Utgått 2020-01-01)</td>
      <td>1211</td>
    </tr>
    <tr>
      <td></td>
      <td>Ølen (Utgått)</td>
      <td>1214</td>
    </tr>
    <tr>
      <td></td>
      <td>Sveio (Utgått 2020-01-01)</td>
      <td>1216</td>
    </tr>
    <tr>
      <td></td>
      <td>Bømlo (Utgått 2020-01-01)</td>
      <td>1219</td>
    </tr>
    <tr>
      <td></td>
      <td>Stord (Utgått 2020-01-01)</td>
      <td>1221</td>
    </tr>
    <tr>
      <td></td>
      <td>Fitjar (Utgått 2020-01-01)</td>
      <td>1222</td>
    </tr>
    <tr>
      <td></td>
      <td>Tysnes (Utgått 2020-01-01)</td>
      <td>1223</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvinnherad (Utgått 2020-01-01)</td>
      <td>1224</td>
    </tr>
    <tr>
      <td></td>
      <td>Jondal (Utgått 2020-01-01)</td>
      <td>1227</td>
    </tr>
    <tr>
      <td></td>
      <td>Odda (Utgått 2020-01-01)</td>
      <td>1228</td>
    </tr>
    <tr>
      <td></td>
      <td>Ullensvang (Utgått 2020-01-01)</td>
      <td>1231</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidfjord (Utgått 2020-01-01)</td>
      <td>1232</td>
    </tr>
    <tr>
      <td></td>
      <td>Ulvik (Utgått 2020-01-01)</td>
      <td>1233</td>
    </tr>
    <tr>
      <td></td>
      <td>Granvin (Utgått 2020-01-01)</td>
      <td>1234</td>
    </tr>
    <tr>
      <td></td>
      <td>Voss (Utgått 2020-01-01)</td>
      <td>1235</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvam (Utgått 2020-01-01)</td>
      <td>1238</td>
    </tr>
    <tr>
      <td></td>
      <td>Fusa (Utgått 2020-01-01)</td>
      <td>1241</td>
    </tr>
    <tr>
      <td></td>
      <td>Samnanger (Utgått 2020-01-01)</td>
      <td>1242</td>
    </tr>
    <tr>
      <td></td>
      <td>Os i Hordaland (Utgått 2020-01-01)</td>
      <td>1243</td>
    </tr>
    <tr>
      <td></td>
      <td>Austevoll (Utgått 2020-01-01)</td>
      <td>1244</td>
    </tr>
    <tr>
      <td></td>
      <td>Sund (Utgått 2020-01-01)</td>
      <td>1245</td>
    </tr>
    <tr>
      <td></td>
      <td>Fjell (Utgått 2020-01-01)</td>
      <td>1246</td>
    </tr>
    <tr>
      <td></td>
      <td>Askøy (Utgått 2020-01-01)</td>
      <td>1247</td>
    </tr>
    <tr>
      <td></td>
      <td>Vaksdal (Utgått 2020-01-01)</td>
      <td>1251</td>
    </tr>
    <tr>
      <td></td>
      <td>Modalen (Utgått 2020-01-01)</td>
      <td>1252</td>
    </tr>
    <tr>
      <td></td>
      <td>Osterøy (Utgått 2020-01-01)</td>
      <td>1253</td>
    </tr>
    <tr>
      <td></td>
      <td>Meland (Utgått 2020-01-01)</td>
      <td>1256</td>
    </tr>
    <tr>
      <td></td>
      <td>Øygarden (Utgått 2020-01-01)</td>
      <td>1259</td>
    </tr>
    <tr>
      <td></td>
      <td>Radøy (Utgått 2020-01-01)</td>
      <td>1260</td>
    </tr>
    <tr>
      <td></td>
      <td>Lindås (Utgått 2020-01-01)</td>
      <td>1263</td>
    </tr>
    <tr>
      <td></td>
      <td>Austrheim (Utgått 2020-01-01)</td>
      <td>1264</td>
    </tr>
    <tr>
      <td></td>
      <td>Fedje (Utgått 2020-01-01)</td>
      <td>1265</td>
    </tr>
    <tr>
      <td></td>
      <td>Masfjorden (Utgått 2020-01-01)</td>
      <td>1266</td>
    </tr>
    <tr>
      <td></td>
      <td>Flora (Utgått 2020-01-01)</td>
      <td>1401</td>
    </tr>
    <tr>
      <td></td>
      <td>Gulen (Utgått 2020-01-01)</td>
      <td>1411</td>
    </tr>
    <tr>
      <td></td>
      <td>Solund (Utgått 2020-01-01)</td>
      <td>1412</td>
    </tr>
    <tr>
      <td></td>
      <td>Hyllestad (Utgått 2020-01-01)</td>
      <td>1413</td>
    </tr>
    <tr>
      <td></td>
      <td>Høyanger (Utgått 2020-01-01)</td>
      <td>1416</td>
    </tr>
    <tr>
      <td></td>
      <td>Vik (Utgått 2020-01-01)</td>
      <td>1417</td>
    </tr>
    <tr>
      <td></td>
      <td>Balestrand (Utgått 2020-01-01)</td>
      <td>1418</td>
    </tr>
    <tr>
      <td></td>
      <td>Leikanger (Utgått 2020-01-01)</td>
      <td>1419</td>
    </tr>
    <tr>
      <td></td>
      <td>Sogndal (Utgått 2020-01-01)</td>
      <td>1420</td>
    </tr>
    <tr>
      <td></td>
      <td>Aurland (Utgått 2020-01-01)</td>
      <td>1421</td>
    </tr>
    <tr>
      <td></td>
      <td>Lærdal (Utgått 2020-01-01)</td>
      <td>1422</td>
    </tr>
    <tr>
      <td></td>
      <td>Årdal (Utgått 2020-01-01)</td>
      <td>1424</td>
    </tr>
    <tr>
      <td></td>
      <td>Luster (Utgått 2020-01-01)</td>
      <td>1426</td>
    </tr>
    <tr>
      <td></td>
      <td>Askvoll (Utgått 2020-01-01)</td>
      <td>1428</td>
    </tr>
    <tr>
      <td></td>
      <td>Fjaler (Utgått 2020-01-01)</td>
      <td>1429</td>
    </tr>
    <tr>
      <td></td>
      <td>Gaular (Utgått 2020-01-01)</td>
      <td>1430</td>
    </tr>
    <tr>
      <td></td>
      <td>Jølster (Utgått 2020-01-01)</td>
      <td>1431</td>
    </tr>
    <tr>
      <td></td>
      <td>Førde (Utgått 2020-01-01)</td>
      <td>1432</td>
    </tr>
    <tr>
      <td></td>
      <td>Naustdal (Utgått 2020-01-01)</td>
      <td>1433</td>
    </tr>
    <tr>
      <td></td>
      <td>Bremanger (Utgått 2020-01-01)</td>
      <td>1438</td>
    </tr>
    <tr>
      <td></td>
      <td>Vågsøy (Utgått 2020-01-01)</td>
      <td>1439</td>
    </tr>
    <tr>
      <td></td>
      <td>Selje (Utgått 2020-01-01)</td>
      <td>1441</td>
    </tr>
    <tr>
      <td></td>
      <td>Eid (Utgått 2020-01-01)</td>
      <td>1443</td>
    </tr>
    <tr>
      <td></td>
      <td>Hornindal (Utgått 2020-01-01)</td>
      <td>1444</td>
    </tr>
    <tr>
      <td></td>
      <td>Gloppen (Utgått 2020-01-01)</td>
      <td>1445</td>
    </tr>
    <tr>
      <td></td>
      <td>Stryn (Utgått 2020-01-01)</td>
      <td>1449</td>
    </tr>
    <tr>
      <td></td>
      <td>Molde (Utgått 2020-01-01)</td>
      <td>1502</td>
    </tr>
    <tr>
      <td></td>
      <td>Ålesund (Utgått 2020-01-01)</td>
      <td>1504</td>
    </tr>
    <tr>
      <td></td>
      <td>Kristiansund</td>
      <td>1505</td>
    </tr>
    <tr>
      <td></td>
      <td>Molde</td>
      <td>1506</td>
    </tr>
    <tr>
      <td></td>
      <td>Ålesund</td>
      <td>1507</td>
    </tr>
    <tr>
      <td></td>
      <td>Vanylven</td>
      <td>1511</td>
    </tr>
    <tr>
      <td></td>
      <td>Sande i Møre og Romsdal</td>
      <td>1514</td>
    </tr>
    <tr>
      <td></td>
      <td>Herøy i Møre og Romsdal</td>
      <td>1515</td>
    </tr>
    <tr>
      <td></td>
      <td>Ulstein</td>
      <td>1516</td>
    </tr>
    <tr>
      <td></td>
      <td>Hareid</td>
      <td>1517</td>
    </tr>
    <tr>
      <td></td>
      <td>Volda (Utgått 2020-01-01)</td>
      <td>1519</td>
    </tr>
    <tr>
      <td></td>
      <td>Ørsta</td>
      <td>1520</td>
    </tr>
    <tr>
      <td></td>
      <td>Ørskog (Utgått 2020-01-01)</td>
      <td>1523</td>
    </tr>
    <tr>
      <td></td>
      <td>Norddal (Utgått 2020-01-01)</td>
      <td>1524</td>
    </tr>
    <tr>
      <td></td>
      <td>Stranda</td>
      <td>1525</td>
    </tr>
    <tr>
      <td></td>
      <td>Stordal (Utgått 2020-01-01)</td>
      <td>1526</td>
    </tr>
    <tr>
      <td></td>
      <td>Sykkylven</td>
      <td>1528</td>
    </tr>
    <tr>
      <td></td>
      <td>Skodje (Utgått 2020-01-01)</td>
      <td>1529</td>
    </tr>
    <tr>
      <td></td>
      <td>Sula</td>
      <td>1531</td>
    </tr>
    <tr>
      <td></td>
      <td>Giske</td>
      <td>1532</td>
    </tr>
    <tr>
      <td></td>
      <td>Haram (Utgått 2020-01-01)</td>
      <td>1534</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestnes</td>
      <td>1535</td>
    </tr>
    <tr>
      <td></td>
      <td>Rauma</td>
      <td>1539</td>
    </tr>
    <tr>
      <td></td>
      <td>Nesset (Utgått 2020-01-01)</td>
      <td>1543</td>
    </tr>
    <tr>
      <td></td>
      <td>Midsund (Utgått 2020-01-01)</td>
      <td>1545</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandøy (Utgått 2020-01-01)</td>
      <td>1546</td>
    </tr>
    <tr>
      <td></td>
      <td>Aukra</td>
      <td>1547</td>
    </tr>
    <tr>
      <td></td>
      <td>Fræna (Utgått 2020-01-01)</td>
      <td>1548</td>
    </tr>
    <tr>
      <td></td>
      <td>Eide (Utgått 2020-01-01)</td>
      <td>1551</td>
    </tr>
    <tr>
      <td></td>
      <td>Averøy</td>
      <td>1554</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjemnes</td>
      <td>1557</td>
    </tr>
    <tr>
      <td></td>
      <td>Tingvoll</td>
      <td>1560</td>
    </tr>
    <tr>
      <td></td>
      <td>Sunndal</td>
      <td>1563</td>
    </tr>
    <tr>
      <td></td>
      <td>Surnadal</td>
      <td>1566</td>
    </tr>
    <tr>
      <td></td>
      <td>Rindal (Utgått)</td>
      <td>1567</td>
    </tr>
    <tr>
      <td></td>
      <td>Aure (Utgått)</td>
      <td>1569</td>
    </tr>
    <tr>
      <td></td>
      <td>Halsa (Utgått 2020-01-01)</td>
      <td>1571</td>
    </tr>
    <tr>
      <td></td>
      <td>Tustna (Utgått)</td>
      <td>1572</td>
    </tr>
    <tr>
      <td></td>
      <td>Smøla</td>
      <td>1573</td>
    </tr>
    <tr>
      <td></td>
      <td>Aure</td>
      <td>1576</td>
    </tr>
    <tr>
      <td></td>
      <td>Volda</td>
      <td>1577</td>
    </tr>
    <tr>
      <td></td>
      <td>Fjord</td>
      <td>1578</td>
    </tr>
    <tr>
      <td></td>
      <td>Hustadvika</td>
      <td>1579</td>
    </tr>
    <tr>
      <td></td>
      <td>Trondheim (Utgått)</td>
      <td>1601</td>
    </tr>
    <tr>
      <td></td>
      <td>Hemne (Utgått)</td>
      <td>1612</td>
    </tr>
    <tr>
      <td></td>
      <td>Snillfjord (Utgått)</td>
      <td>1613</td>
    </tr>
    <tr>
      <td></td>
      <td>Hitra (Utgått)</td>
      <td>1617</td>
    </tr>
    <tr>
      <td></td>
      <td>Frøya (Utgått)</td>
      <td>1620</td>
    </tr>
    <tr>
      <td></td>
      <td>Ørland (Utgått)</td>
      <td>1621</td>
    </tr>
    <tr>
      <td></td>
      <td>Agdenes (Utgått)</td>
      <td>1622</td>
    </tr>
    <tr>
      <td></td>
      <td>Rissa (Utgått)</td>
      <td>1624</td>
    </tr>
    <tr>
      <td></td>
      <td>Bjugn (Utgått)</td>
      <td>1627</td>
    </tr>
    <tr>
      <td></td>
      <td>Åfjord (Utgått)</td>
      <td>1630</td>
    </tr>
    <tr>
      <td></td>
      <td>Roan (Utgått)</td>
      <td>1632</td>
    </tr>
    <tr>
      <td></td>
      <td>Osen (Utgått)</td>
      <td>1633</td>
    </tr>
    <tr>
      <td></td>
      <td>Oppdal (Utgått)</td>
      <td>1634</td>
    </tr>
    <tr>
      <td></td>
      <td>Rennebu (Utgått)</td>
      <td>1635</td>
    </tr>
    <tr>
      <td></td>
      <td>Meldal (Utgått)</td>
      <td>1636</td>
    </tr>
    <tr>
      <td></td>
      <td>Orkdal (Utgått)</td>
      <td>1638</td>
    </tr>
    <tr>
      <td></td>
      <td>Røros (Utgått)</td>
      <td>1640</td>
    </tr>
    <tr>
      <td></td>
      <td>Holtålen (Utgått)</td>
      <td>1644</td>
    </tr>
    <tr>
      <td></td>
      <td>Midtre Gauldal (Utgått)</td>
      <td>1648</td>
    </tr>
    <tr>
      <td></td>
      <td>Melhus (Utgått)</td>
      <td>1653</td>
    </tr>
    <tr>
      <td></td>
      <td>Skaun (Utgått)</td>
      <td>1657</td>
    </tr>
    <tr>
      <td></td>
      <td>Klæbu (Utgått)</td>
      <td>1662</td>
    </tr>
    <tr>
      <td></td>
      <td>Malvik (Utgått)</td>
      <td>1663</td>
    </tr>
    <tr>
      <td></td>
      <td>Selbu (Utgått)</td>
      <td>1664</td>
    </tr>
    <tr>
      <td></td>
      <td>Tydal (Utgått)</td>
      <td>1665</td>
    </tr>
    <tr>
      <td></td>
      <td>Steinkjer (Utgått)</td>
      <td>1702</td>
    </tr>
    <tr>
      <td></td>
      <td>Namsos (Utgått)</td>
      <td>1703</td>
    </tr>
    <tr>
      <td></td>
      <td>Meråker (Utgått)</td>
      <td>1711</td>
    </tr>
    <tr>
      <td></td>
      <td>Stjørdal (Utgått)</td>
      <td>1714</td>
    </tr>
    <tr>
      <td></td>
      <td>Frosta (Utgått)</td>
      <td>1717</td>
    </tr>
    <tr>
      <td></td>
      <td>Leksvik (Utgått)</td>
      <td>1718</td>
    </tr>
    <tr>
      <td></td>
      <td>Levanger (Utgått)</td>
      <td>1719</td>
    </tr>
    <tr>
      <td></td>
      <td>Verdal (Utgått)</td>
      <td>1721</td>
    </tr>
    <tr>
      <td></td>
      <td>Mosvik (Utgått)</td>
      <td>1723</td>
    </tr>
    <tr>
      <td></td>
      <td>Verran (Utgått)</td>
      <td>1724</td>
    </tr>
    <tr>
      <td></td>
      <td>Namdalseid (Utgått)</td>
      <td>1725</td>
    </tr>
    <tr>
      <td></td>
      <td>Inderøy (Utgått)</td>
      <td>1729</td>
    </tr>
    <tr>
      <td></td>
      <td>Snåase – Snåsa (Utgått)</td>
      <td>1736</td>
    </tr>
    <tr>
      <td></td>
      <td>Lierne (Utgått)</td>
      <td>1738</td>
    </tr>
    <tr>
      <td></td>
      <td>Raarvihke – Røyrvik (Utgått)</td>
      <td>1739</td>
    </tr>
    <tr>
      <td></td>
      <td>Namsskogan (Utgått)</td>
      <td>1740</td>
    </tr>
    <tr>
      <td></td>
      <td>Grong (Utgått)</td>
      <td>1742</td>
    </tr>
    <tr>
      <td></td>
      <td>Høylandet (Utgått)</td>
      <td>1743</td>
    </tr>
    <tr>
      <td></td>
      <td>Overhalla (Utgått)</td>
      <td>1744</td>
    </tr>
    <tr>
      <td></td>
      <td>Fosnes (Utgått)</td>
      <td>1748</td>
    </tr>
    <tr>
      <td></td>
      <td>Flatanger (Utgått)</td>
      <td>1749</td>
    </tr>
    <tr>
      <td></td>
      <td>Vikna (Utgått)</td>
      <td>1750</td>
    </tr>
    <tr>
      <td></td>
      <td>Nærøy (Utgått)</td>
      <td>1751</td>
    </tr>
    <tr>
      <td></td>
      <td>Leka (Utgått)</td>
      <td>1755</td>
    </tr>
    <tr>
      <td></td>
      <td>Inderøy (Utgått)</td>
      <td>1756</td>
    </tr>
    <tr>
      <td></td>
      <td>Bodø</td>
      <td>1804</td>
    </tr>
    <tr>
      <td></td>
      <td>Narvik (Utgått 2020-01-01)</td>
      <td>1805</td>
    </tr>
    <tr>
      <td></td>
      <td>Narvik</td>
      <td>1806</td>
    </tr>
    <tr>
      <td></td>
      <td>Bindal</td>
      <td>1811</td>
    </tr>
    <tr>
      <td></td>
      <td>Sømna</td>
      <td>1812</td>
    </tr>
    <tr>
      <td></td>
      <td>Brønnøy</td>
      <td>1813</td>
    </tr>
    <tr>
      <td></td>
      <td>Vega</td>
      <td>1815</td>
    </tr>
    <tr>
      <td></td>
      <td>Vevelstad</td>
      <td>1816</td>
    </tr>
    <tr>
      <td></td>
      <td>Herøy i Nordland</td>
      <td>1818</td>
    </tr>
    <tr>
      <td></td>
      <td>Alstahaug</td>
      <td>1820</td>
    </tr>
    <tr>
      <td></td>
      <td>Leirfjord</td>
      <td>1822</td>
    </tr>
    <tr>
      <td></td>
      <td>Vefsn</td>
      <td>1824</td>
    </tr>
    <tr>
      <td></td>
      <td>Grane</td>
      <td>1825</td>
    </tr>
    <tr>
      <td></td>
      <td>Hattfjelldal</td>
      <td>1826</td>
    </tr>
    <tr>
      <td></td>
      <td>Dønna</td>
      <td>1827</td>
    </tr>
    <tr>
      <td></td>
      <td>Nesna</td>
      <td>1828</td>
    </tr>
    <tr>
      <td></td>
      <td>Hemnes</td>
      <td>1832</td>
    </tr>
    <tr>
      <td></td>
      <td>Rana</td>
      <td>1833</td>
    </tr>
    <tr>
      <td></td>
      <td>Lurøy</td>
      <td>1834</td>
    </tr>
    <tr>
      <td></td>
      <td>Træna</td>
      <td>1835</td>
    </tr>
    <tr>
      <td></td>
      <td>Rødøy</td>
      <td>1836</td>
    </tr>
    <tr>
      <td></td>
      <td>Meløy</td>
      <td>1837</td>
    </tr>
    <tr>
      <td></td>
      <td>Gildeskål</td>
      <td>1838</td>
    </tr>
    <tr>
      <td></td>
      <td>Beiarn</td>
      <td>1839</td>
    </tr>
    <tr>
      <td></td>
      <td>Saltdal</td>
      <td>1840</td>
    </tr>
    <tr>
      <td></td>
      <td>Fauske – Fuossko</td>
      <td>1841</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjerstad (Utgått)</td>
      <td>1842</td>
    </tr>
    <tr>
      <td></td>
      <td>Sørfold</td>
      <td>1845</td>
    </tr>
    <tr>
      <td></td>
      <td>Steigen</td>
      <td>1848</td>
    </tr>
    <tr>
      <td></td>
      <td>Hamarøy – Hábmer (Utgått 2020-01-01)</td>
      <td>1849</td>
    </tr>
    <tr>
      <td></td>
      <td>Divtasvuodna – Tysfjord (Utgått 2020-01-01)</td>
      <td>1850</td>
    </tr>
    <tr>
      <td></td>
      <td>Lødingen</td>
      <td>1851</td>
    </tr>
    <tr>
      <td></td>
      <td>Tjeldsund (Utgått 2020-01-01)</td>
      <td>1852</td>
    </tr>
    <tr>
      <td></td>
      <td>Evenes</td>
      <td>1853</td>
    </tr>
    <tr>
      <td></td>
      <td>Ballangen (Utgått 2020-01-01)</td>
      <td>1854</td>
    </tr>
    <tr>
      <td></td>
      <td>Røst</td>
      <td>1856</td>
    </tr>
    <tr>
      <td></td>
      <td>Værøy</td>
      <td>1857</td>
    </tr>
    <tr>
      <td></td>
      <td>Flakstad</td>
      <td>1859</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestvågøy</td>
      <td>1860</td>
    </tr>
    <tr>
      <td></td>
      <td>Vågan</td>
      <td>1865</td>
    </tr>
    <tr>
      <td></td>
      <td>Hadsel</td>
      <td>1866</td>
    </tr>
    <tr>
      <td></td>
      <td>Bø i Nordland</td>
      <td>1867</td>
    </tr>
    <tr>
      <td></td>
      <td>Øksnes</td>
      <td>1868</td>
    </tr>
    <tr>
      <td></td>
      <td>Sortland – Suortá</td>
      <td>1870</td>
    </tr>
    <tr>
      <td></td>
      <td>Andøy</td>
      <td>1871</td>
    </tr>
    <tr>
      <td></td>
      <td>Moskenes</td>
      <td>1874</td>
    </tr>
    <tr>
      <td></td>
      <td>Hamarøy – Hábmer</td>
      <td>1875</td>
    </tr>
    <tr>
      <td></td>
      <td>Harstad (Utgått)</td>
      <td>1901</td>
    </tr>
    <tr>
      <td></td>
      <td>Tromsø (Utgått 2020-01-01)</td>
      <td>1902</td>
    </tr>
    <tr>
      <td></td>
      <td>Harstad – Hárstták (Utgått 2020-01-01)</td>
      <td>1903</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvæfjord (Utgått 2020-01-01)</td>
      <td>1911</td>
    </tr>
    <tr>
      <td></td>
      <td>Skånland (Utgått 2020-01-01)</td>
      <td>1913</td>
    </tr>
    <tr>
      <td></td>
      <td>Bjarkøy (Utgått)</td>
      <td>1915</td>
    </tr>
    <tr>
      <td></td>
      <td>Ibestad (Utgått 2020-01-01)</td>
      <td>1917</td>
    </tr>
    <tr>
      <td></td>
      <td>Gratangen (Utgått 2020-01-01)</td>
      <td>1919</td>
    </tr>
    <tr>
      <td></td>
      <td>Loabák – Lavangen (Utgått 2020-01-01)</td>
      <td>1920</td>
    </tr>
    <tr>
      <td></td>
      <td>Bardu (Utgått 2020-01-01)</td>
      <td>1922</td>
    </tr>
    <tr>
      <td></td>
      <td>Salangen (Utgått 2020-01-01)</td>
      <td>1923</td>
    </tr>
    <tr>
      <td></td>
      <td>Målselv (Utgått 2020-01-01)</td>
      <td>1924</td>
    </tr>
    <tr>
      <td></td>
      <td>Sørreisa (Utgått 2020-01-01)</td>
      <td>1925</td>
    </tr>
    <tr>
      <td></td>
      <td>Dyrøy (Utgått 2020-01-01)</td>
      <td>1926</td>
    </tr>
    <tr>
      <td></td>
      <td>Tranøy (Utgått 2020-01-01)</td>
      <td>1927</td>
    </tr>
    <tr>
      <td></td>
      <td>Torsken (Utgått 2020-01-01)</td>
      <td>1928</td>
    </tr>
    <tr>
      <td></td>
      <td>Berg (Utgått 2020-01-01)</td>
      <td>1929</td>
    </tr>
    <tr>
      <td></td>
      <td>Lenvik (Utgått 2020-01-01)</td>
      <td>1931</td>
    </tr>
    <tr>
      <td></td>
      <td>Balsfjord (Utgått 2020-01-01)</td>
      <td>1933</td>
    </tr>
    <tr>
      <td></td>
      <td>Karlsøy (Utgått 2020-01-01)</td>
      <td>1936</td>
    </tr>
    <tr>
      <td></td>
      <td>Lyngen (Utgått 2020-01-01)</td>
      <td>1938</td>
    </tr>
    <tr>
      <td></td>
      <td>Storfjord – Omasvuotna – Omasvuono (Utgått 2020-01-01)</td>
      <td>1939</td>
    </tr>
    <tr>
      <td></td>
      <td>Gáivuotna – Kåfjord – Kaivuono (Utgått 2020-01-01)</td>
      <td>1940</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjervøy (Utgått 2020-01-01)</td>
      <td>1941</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordreisa - Ráisa - Raisi  (Utgått 2020-01-01)</td>
      <td>1942</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvænangen (Utgått 2020-01-01)</td>
      <td>1943</td>
    </tr>
    <tr>
      <td></td>
      <td>Hammerfest (Utgått)</td>
      <td>2001</td>
    </tr>
    <tr>
      <td></td>
      <td>Vardø (Utgått 2020-01-01)</td>
      <td>2002</td>
    </tr>
    <tr>
      <td></td>
      <td>Vadsø (Utgått 2020-01-01)</td>
      <td>2003</td>
    </tr>
    <tr>
      <td></td>
      <td>Hammerfest (Utgått 2020-01-01)</td>
      <td>2004</td>
    </tr>
    <tr>
      <td></td>
      <td>Guovdageaidnu – Kautokeino (Utgått 2020-01-01)</td>
      <td>2011</td>
    </tr>
    <tr>
      <td></td>
      <td>Alta (Utgått 2020-01-01)</td>
      <td>2012</td>
    </tr>
    <tr>
      <td></td>
      <td>Loppa (Utgått 2020-01-01)</td>
      <td>2014</td>
    </tr>
    <tr>
      <td></td>
      <td>Hasvik (Utgått 2020-01-01)</td>
      <td>2015</td>
    </tr>
    <tr>
      <td></td>
      <td>Sørøysund (Utgått)</td>
      <td>2016</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvalsund (Utgått 2020-01-01)</td>
      <td>2017</td>
    </tr>
    <tr>
      <td></td>
      <td>Måsøy (Utgått 2020-01-01)</td>
      <td>2018</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordkapp (Utgått 2020-01-01)</td>
      <td>2019</td>
    </tr>
    <tr>
      <td></td>
      <td>Porsanger – Porsáŋgu – Porsanki (Utgått 2020-01-01)</td>
      <td>2020</td>
    </tr>
    <tr>
      <td></td>
      <td>Kárášjohka – Karasjok  (Utgått 2020-01-01)</td>
      <td>2021</td>
    </tr>
    <tr>
      <td></td>
      <td>Lebesby (Utgått 2020-01-01)</td>
      <td>2022</td>
    </tr>
    <tr>
      <td></td>
      <td>Gamvik (Utgått 2020-01-01)</td>
      <td>2023</td>
    </tr>
    <tr>
      <td></td>
      <td>Berlevåg (Utgått 2020-01-01)</td>
      <td>2024</td>
    </tr>
    <tr>
      <td></td>
      <td>Deatnu – Tana (Utgått 2020-01-01)</td>
      <td>2025</td>
    </tr>
    <tr>
      <td></td>
      <td>Unjárga – Nesseby (Utgått 2020-01-01)</td>
      <td>2027</td>
    </tr>
    <tr>
      <td></td>
      <td>Båtsfjord (Utgått 2020-01-01)</td>
      <td>2028</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Varanger (Utgått 2020-01-01)</td>
      <td>2030</td>
    </tr>
    <tr>
      <td></td>
      <td>Halden</td>
      <td>3001</td>
    </tr>
    <tr>
      <td></td>
      <td>Moss</td>
      <td>3002</td>
    </tr>
    <tr>
      <td></td>
      <td>Sarpsborg</td>
      <td>3003</td>
    </tr>
    <tr>
      <td></td>
      <td>Fredrikstad</td>
      <td>3004</td>
    </tr>
    <tr>
      <td></td>
      <td>Drammen</td>
      <td>3005</td>
    </tr>
    <tr>
      <td></td>
      <td>Kongsberg</td>
      <td>3006</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringerike</td>
      <td>3007</td>
    </tr>
    <tr>
      <td></td>
      <td>Hvaler</td>
      <td>3011</td>
    </tr>
    <tr>
      <td></td>
      <td>Aremark</td>
      <td>3012</td>
    </tr>
    <tr>
      <td></td>
      <td>Marker</td>
      <td>3013</td>
    </tr>
    <tr>
      <td></td>
      <td>Indre Østfold</td>
      <td>3014</td>
    </tr>
    <tr>
      <td></td>
      <td>Skiptvet</td>
      <td>3015</td>
    </tr>
    <tr>
      <td></td>
      <td>Rakkestad</td>
      <td>3016</td>
    </tr>
    <tr>
      <td></td>
      <td>Råde</td>
      <td>3017</td>
    </tr>
    <tr>
      <td></td>
      <td>Våler i Viken</td>
      <td>3018</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestby</td>
      <td>3019</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordre Follo</td>
      <td>3020</td>
    </tr>
    <tr>
      <td></td>
      <td>Ås</td>
      <td>3021</td>
    </tr>
    <tr>
      <td></td>
      <td>Frogn</td>
      <td>3022</td>
    </tr>
    <tr>
      <td></td>
      <td>Nesodden</td>
      <td>3023</td>
    </tr>
    <tr>
      <td></td>
      <td>Bærum</td>
      <td>3024</td>
    </tr>
    <tr>
      <td></td>
      <td>Asker</td>
      <td>3025</td>
    </tr>
    <tr>
      <td></td>
      <td>Aurskog-Høland</td>
      <td>3026</td>
    </tr>
    <tr>
      <td></td>
      <td>Rælingen</td>
      <td>3027</td>
    </tr>
    <tr>
      <td></td>
      <td>Enebakk</td>
      <td>3028</td>
    </tr>
    <tr>
      <td></td>
      <td>Lørenskog</td>
      <td>3029</td>
    </tr>
    <tr>
      <td></td>
      <td>Lillestrøm</td>
      <td>3030</td>
    </tr>
    <tr>
      <td></td>
      <td>Nittedal</td>
      <td>3031</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjerdrum</td>
      <td>3032</td>
    </tr>
    <tr>
      <td></td>
      <td>Ullensaker</td>
      <td>3033</td>
    </tr>
    <tr>
      <td></td>
      <td>Nes (tidligere Nes i Akershus)</td>
      <td>3034</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidsvoll</td>
      <td>3035</td>
    </tr>
    <tr>
      <td></td>
      <td>Nannestad</td>
      <td>3036</td>
    </tr>
    <tr>
      <td></td>
      <td>Hurdal</td>
      <td>3037</td>
    </tr>
    <tr>
      <td></td>
      <td>Hole</td>
      <td>3038</td>
    </tr>
    <tr>
      <td></td>
      <td>Flå</td>
      <td>3039</td>
    </tr>
    <tr>
      <td></td>
      <td>Nesbyen (tidligere Nes i Buskerud)</td>
      <td>3040</td>
    </tr>
    <tr>
      <td></td>
      <td>Gol</td>
      <td>3041</td>
    </tr>
    <tr>
      <td></td>
      <td>Hemsedal</td>
      <td>3042</td>
    </tr>
    <tr>
      <td></td>
      <td>Ål</td>
      <td>3043</td>
    </tr>
    <tr>
      <td></td>
      <td>Hol</td>
      <td>3044</td>
    </tr>
    <tr>
      <td></td>
      <td>Sigdal</td>
      <td>3045</td>
    </tr>
    <tr>
      <td></td>
      <td>Krødsherad</td>
      <td>3046</td>
    </tr>
    <tr>
      <td></td>
      <td>Modum</td>
      <td>3047</td>
    </tr>
    <tr>
      <td></td>
      <td>Øvre Eiker</td>
      <td>3048</td>
    </tr>
    <tr>
      <td></td>
      <td>Lier</td>
      <td>3049</td>
    </tr>
    <tr>
      <td></td>
      <td>Flesberg</td>
      <td>3050</td>
    </tr>
    <tr>
      <td></td>
      <td>Rollag</td>
      <td>3051</td>
    </tr>
    <tr>
      <td></td>
      <td>Nore og Uvdal</td>
      <td>3052</td>
    </tr>
    <tr>
      <td></td>
      <td>Jevnaker</td>
      <td>3053</td>
    </tr>
    <tr>
      <td></td>
      <td>Lunner</td>
      <td>3054</td>
    </tr>
    <tr>
      <td></td>
      <td>Kongsvinger</td>
      <td>3401</td>
    </tr>
    <tr>
      <td></td>
      <td>Hamar</td>
      <td>3403</td>
    </tr>
    <tr>
      <td></td>
      <td>Lillehammer</td>
      <td>3405</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjøvik</td>
      <td>3407</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringsaker</td>
      <td>3411</td>
    </tr>
    <tr>
      <td></td>
      <td>Løten</td>
      <td>3412</td>
    </tr>
    <tr>
      <td></td>
      <td>Stange</td>
      <td>3413</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Odal</td>
      <td>3414</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Odal</td>
      <td>3415</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidskog</td>
      <td>3416</td>
    </tr>
    <tr>
      <td></td>
      <td>Grue</td>
      <td>3417</td>
    </tr>
    <tr>
      <td></td>
      <td>Åsnes</td>
      <td>3418</td>
    </tr>
    <tr>
      <td></td>
      <td>Våler i Innlandet</td>
      <td>3419</td>
    </tr>
    <tr>
      <td></td>
      <td>Elverum</td>
      <td>3420</td>
    </tr>
    <tr>
      <td></td>
      <td>Trysil</td>
      <td>3421</td>
    </tr>
    <tr>
      <td></td>
      <td>Åmot</td>
      <td>3422</td>
    </tr>
    <tr>
      <td></td>
      <td>Stor-Elvdal</td>
      <td>3423</td>
    </tr>
    <tr>
      <td></td>
      <td>Rendalen</td>
      <td>3424</td>
    </tr>
    <tr>
      <td></td>
      <td>Engerdal</td>
      <td>3425</td>
    </tr>
    <tr>
      <td></td>
      <td>Tolga</td>
      <td>3426</td>
    </tr>
    <tr>
      <td></td>
      <td>Tynset</td>
      <td>3427</td>
    </tr>
    <tr>
      <td></td>
      <td>Alvdal</td>
      <td>3428</td>
    </tr>
    <tr>
      <td></td>
      <td>Folldal</td>
      <td>3429</td>
    </tr>
    <tr>
      <td></td>
      <td>Os</td>
      <td>3430</td>
    </tr>
    <tr>
      <td></td>
      <td>Dovre</td>
      <td>3431</td>
    </tr>
    <tr>
      <td></td>
      <td>Lesja</td>
      <td>3432</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjåk</td>
      <td>3433</td>
    </tr>
    <tr>
      <td></td>
      <td>Lom</td>
      <td>3434</td>
    </tr>
    <tr>
      <td></td>
      <td>Vågå</td>
      <td>3435</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Fron</td>
      <td>3436</td>
    </tr>
    <tr>
      <td></td>
      <td>Sel</td>
      <td>3437</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Fron</td>
      <td>3438</td>
    </tr>
    <tr>
      <td></td>
      <td>Ringebu</td>
      <td>3439</td>
    </tr>
    <tr>
      <td></td>
      <td>Øyer</td>
      <td>3440</td>
    </tr>
    <tr>
      <td></td>
      <td>Gausdal</td>
      <td>3441</td>
    </tr>
    <tr>
      <td></td>
      <td>Østre Toten</td>
      <td>3442</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestre Toten</td>
      <td>3443</td>
    </tr>
    <tr>
      <td></td>
      <td>Gran</td>
      <td>3446</td>
    </tr>
    <tr>
      <td></td>
      <td>Søndre Land</td>
      <td>3447</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordre Land</td>
      <td>3448</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Aurdal</td>
      <td>3449</td>
    </tr>
    <tr>
      <td></td>
      <td>Etnedal</td>
      <td>3450</td>
    </tr>
    <tr>
      <td></td>
      <td>Nord-Aurdal</td>
      <td>3451</td>
    </tr>
    <tr>
      <td></td>
      <td>Vestre Slidre</td>
      <td>3452</td>
    </tr>
    <tr>
      <td></td>
      <td>Øystre Slidre</td>
      <td>3453</td>
    </tr>
    <tr>
      <td></td>
      <td>Vang</td>
      <td>3454</td>
    </tr>
    <tr>
      <td></td>
      <td>Horten</td>
      <td>3801</td>
    </tr>
    <tr>
      <td></td>
      <td>Holmestrand</td>
      <td>3802</td>
    </tr>
    <tr>
      <td></td>
      <td>Tønsberg</td>
      <td>3803</td>
    </tr>
    <tr>
      <td></td>
      <td>Sandefjord</td>
      <td>3804</td>
    </tr>
    <tr>
      <td></td>
      <td>Larvik</td>
      <td>3805</td>
    </tr>
    <tr>
      <td></td>
      <td>Porsgrunn</td>
      <td>3806</td>
    </tr>
    <tr>
      <td></td>
      <td>Skien</td>
      <td>3807</td>
    </tr>
    <tr>
      <td></td>
      <td>Notodden</td>
      <td>3808</td>
    </tr>
    <tr>
      <td></td>
      <td>Færder</td>
      <td>3811</td>
    </tr>
    <tr>
      <td></td>
      <td>Siljan</td>
      <td>3812</td>
    </tr>
    <tr>
      <td></td>
      <td>Bamble</td>
      <td>3813</td>
    </tr>
    <tr>
      <td></td>
      <td>Kragerø</td>
      <td>3814</td>
    </tr>
    <tr>
      <td></td>
      <td>Drangedal</td>
      <td>3815</td>
    </tr>
    <tr>
      <td></td>
      <td>Nome</td>
      <td>3816</td>
    </tr>
    <tr>
      <td></td>
      <td>Midt-Telemark</td>
      <td>3817</td>
    </tr>
    <tr>
      <td></td>
      <td>Tinn</td>
      <td>3818</td>
    </tr>
    <tr>
      <td></td>
      <td>Hjartdal</td>
      <td>3819</td>
    </tr>
    <tr>
      <td></td>
      <td>Seljord</td>
      <td>3820</td>
    </tr>
    <tr>
      <td></td>
      <td>Kviteseid</td>
      <td>3821</td>
    </tr>
    <tr>
      <td></td>
      <td>Nissedal</td>
      <td>3822</td>
    </tr>
    <tr>
      <td></td>
      <td>Fyresdal</td>
      <td>3823</td>
    </tr>
    <tr>
      <td></td>
      <td>Tokke</td>
      <td>3824</td>
    </tr>
    <tr>
      <td></td>
      <td>Vinje</td>
      <td>3825</td>
    </tr>
    <tr>
      <td></td>
      <td>Risør</td>
      <td>4201</td>
    </tr>
    <tr>
      <td></td>
      <td>Grimstad</td>
      <td>4202</td>
    </tr>
    <tr>
      <td></td>
      <td>Arendal</td>
      <td>4203</td>
    </tr>
    <tr>
      <td></td>
      <td>Kristiansand</td>
      <td>4204</td>
    </tr>
    <tr>
      <td></td>
      <td>Lindesnes</td>
      <td>4205</td>
    </tr>
    <tr>
      <td></td>
      <td>Farsund</td>
      <td>4206</td>
    </tr>
    <tr>
      <td></td>
      <td>Flekkefjord</td>
      <td>4207</td>
    </tr>
    <tr>
      <td></td>
      <td>Gjerstad</td>
      <td>4211</td>
    </tr>
    <tr>
      <td></td>
      <td>Vegårshei</td>
      <td>4212</td>
    </tr>
    <tr>
      <td></td>
      <td>Tvedestrand</td>
      <td>4213</td>
    </tr>
    <tr>
      <td></td>
      <td>Froland</td>
      <td>4214</td>
    </tr>
    <tr>
      <td></td>
      <td>Lillesand</td>
      <td>4215</td>
    </tr>
    <tr>
      <td></td>
      <td>Birkenes</td>
      <td>4216</td>
    </tr>
    <tr>
      <td></td>
      <td>Åmli</td>
      <td>4217</td>
    </tr>
    <tr>
      <td></td>
      <td>Iveland</td>
      <td>4218</td>
    </tr>
    <tr>
      <td></td>
      <td>Evje og Hornnes</td>
      <td>4219</td>
    </tr>
    <tr>
      <td></td>
      <td>Bygland</td>
      <td>4220</td>
    </tr>
    <tr>
      <td></td>
      <td>Valle</td>
      <td>4221</td>
    </tr>
    <tr>
      <td></td>
      <td>Bykle</td>
      <td>4222</td>
    </tr>
    <tr>
      <td></td>
      <td>Vennesla</td>
      <td>4223</td>
    </tr>
    <tr>
      <td></td>
      <td>Åseral</td>
      <td>4224</td>
    </tr>
    <tr>
      <td></td>
      <td>Lyngdal</td>
      <td>4225</td>
    </tr>
    <tr>
      <td></td>
      <td>Hægebostad</td>
      <td>4226</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvinesdal</td>
      <td>4227</td>
    </tr>
    <tr>
      <td></td>
      <td>Sirdal</td>
      <td>4228</td>
    </tr>
    <tr>
      <td></td>
      <td>Bergen</td>
      <td>4601</td>
    </tr>
    <tr>
      <td></td>
      <td>Kinn</td>
      <td>4602</td>
    </tr>
    <tr>
      <td></td>
      <td>Etne</td>
      <td>4611</td>
    </tr>
    <tr>
      <td></td>
      <td>Sveio</td>
      <td>4612</td>
    </tr>
    <tr>
      <td></td>
      <td>Bømlo</td>
      <td>4613</td>
    </tr>
    <tr>
      <td></td>
      <td>Stord</td>
      <td>4614</td>
    </tr>
    <tr>
      <td></td>
      <td>Fitjar</td>
      <td>4615</td>
    </tr>
    <tr>
      <td></td>
      <td>Tysnes</td>
      <td>4616</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvinnherad</td>
      <td>4617</td>
    </tr>
    <tr>
      <td></td>
      <td>Ullensvang</td>
      <td>4618</td>
    </tr>
    <tr>
      <td></td>
      <td>Eidfjord</td>
      <td>4619</td>
    </tr>
    <tr>
      <td></td>
      <td>Ulvik</td>
      <td>4620</td>
    </tr>
    <tr>
      <td></td>
      <td>Voss</td>
      <td>4621</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvam</td>
      <td>4622</td>
    </tr>
    <tr>
      <td></td>
      <td>Samnanger</td>
      <td>4623</td>
    </tr>
    <tr>
      <td></td>
      <td>Bjørnafjorden</td>
      <td>4624</td>
    </tr>
    <tr>
      <td></td>
      <td>Austevoll</td>
      <td>4625</td>
    </tr>
    <tr>
      <td></td>
      <td>Øygarden</td>
      <td>4626</td>
    </tr>
    <tr>
      <td></td>
      <td>Askøy</td>
      <td>4627</td>
    </tr>
    <tr>
      <td></td>
      <td>Vaksdal</td>
      <td>4628</td>
    </tr>
    <tr>
      <td></td>
      <td>Modalen</td>
      <td>4629</td>
    </tr>
    <tr>
      <td></td>
      <td>Osterøy</td>
      <td>4630</td>
    </tr>
    <tr>
      <td></td>
      <td>Alver</td>
      <td>4631</td>
    </tr>
    <tr>
      <td></td>
      <td>Austrheim</td>
      <td>4632</td>
    </tr>
    <tr>
      <td></td>
      <td>Fedje</td>
      <td>4633</td>
    </tr>
    <tr>
      <td></td>
      <td>Masfjorden</td>
      <td>4634</td>
    </tr>
    <tr>
      <td></td>
      <td>Gulen</td>
      <td>4635</td>
    </tr>
    <tr>
      <td></td>
      <td>Solund</td>
      <td>4636</td>
    </tr>
    <tr>
      <td></td>
      <td>Hyllestad</td>
      <td>4637</td>
    </tr>
    <tr>
      <td></td>
      <td>Høyanger</td>
      <td>4638</td>
    </tr>
    <tr>
      <td></td>
      <td>Vik</td>
      <td>4639</td>
    </tr>
    <tr>
      <td></td>
      <td>Sogndal</td>
      <td>4640</td>
    </tr>
    <tr>
      <td></td>
      <td>Aurland</td>
      <td>4641</td>
    </tr>
    <tr>
      <td></td>
      <td>Lærdal</td>
      <td>4642</td>
    </tr>
    <tr>
      <td></td>
      <td>Årdal</td>
      <td>4643</td>
    </tr>
    <tr>
      <td></td>
      <td>Luster</td>
      <td>4644</td>
    </tr>
    <tr>
      <td></td>
      <td>Askvoll</td>
      <td>4645</td>
    </tr>
    <tr>
      <td></td>
      <td>Fjaler</td>
      <td>4646</td>
    </tr>
    <tr>
      <td></td>
      <td>Sunnfjord</td>
      <td>4647</td>
    </tr>
    <tr>
      <td></td>
      <td>Bremanger</td>
      <td>4648</td>
    </tr>
    <tr>
      <td></td>
      <td>Stad</td>
      <td>4649</td>
    </tr>
    <tr>
      <td></td>
      <td>Gloppen</td>
      <td>4650</td>
    </tr>
    <tr>
      <td></td>
      <td>Stryn</td>
      <td>4651</td>
    </tr>
    <tr>
      <td></td>
      <td>Trondheim</td>
      <td>5001</td>
    </tr>
    <tr>
      <td></td>
      <td>Steinkjer (Utgått 2020-01-01)</td>
      <td>5004</td>
    </tr>
    <tr>
      <td></td>
      <td>Namsos (Utgått 2020-01-01)</td>
      <td>5005</td>
    </tr>
    <tr>
      <td></td>
      <td>Steinkjer</td>
      <td>5006</td>
    </tr>
    <tr>
      <td></td>
      <td>Namsos</td>
      <td>5007</td>
    </tr>
    <tr>
      <td></td>
      <td>Hemne (Utgått 2020-01-01)</td>
      <td>5011</td>
    </tr>
    <tr>
      <td></td>
      <td>Snillfjord (Utgått 2020-01-01)</td>
      <td>5012</td>
    </tr>
    <tr>
      <td></td>
      <td>Hitra (Utgått 2020-01-01)</td>
      <td>5013</td>
    </tr>
    <tr>
      <td></td>
      <td>Frøya</td>
      <td>5014</td>
    </tr>
    <tr>
      <td></td>
      <td>Ørland (Utgått 2020-01-01)</td>
      <td>5015</td>
    </tr>
    <tr>
      <td></td>
      <td>Agdenes (Utgått 2020-01-01)</td>
      <td>5016</td>
    </tr>
    <tr>
      <td></td>
      <td>Bjugn (Utgått 2020-01-01)</td>
      <td>5017</td>
    </tr>
    <tr>
      <td></td>
      <td>Åfjord (Utgått 2020-01-01)</td>
      <td>5018</td>
    </tr>
    <tr>
      <td></td>
      <td>Roan (Utgått 2020-01-01)</td>
      <td>5019</td>
    </tr>
    <tr>
      <td></td>
      <td>Osen</td>
      <td>5020</td>
    </tr>
    <tr>
      <td></td>
      <td>Oppdal</td>
      <td>5021</td>
    </tr>
    <tr>
      <td></td>
      <td>Rennebu</td>
      <td>5022</td>
    </tr>
    <tr>
      <td></td>
      <td>Meldal (Utgått 2020-01-01)</td>
      <td>5023</td>
    </tr>
    <tr>
      <td></td>
      <td>Orkdal (Utgått 2020-01-01)</td>
      <td>5024</td>
    </tr>
    <tr>
      <td></td>
      <td>Røros</td>
      <td>5025</td>
    </tr>
    <tr>
      <td></td>
      <td>Holtålen</td>
      <td>5026</td>
    </tr>
    <tr>
      <td></td>
      <td>Midtre Gauldal</td>
      <td>5027</td>
    </tr>
    <tr>
      <td></td>
      <td>Melhus</td>
      <td>5028</td>
    </tr>
    <tr>
      <td></td>
      <td>Skaun</td>
      <td>5029</td>
    </tr>
    <tr>
      <td></td>
      <td>Klæbu (Utgått 2020-01-01)</td>
      <td>5030</td>
    </tr>
    <tr>
      <td></td>
      <td>Malvik</td>
      <td>5031</td>
    </tr>
    <tr>
      <td></td>
      <td>Selbu</td>
      <td>5032</td>
    </tr>
    <tr>
      <td></td>
      <td>Tydal</td>
      <td>5033</td>
    </tr>
    <tr>
      <td></td>
      <td>Meråker</td>
      <td>5034</td>
    </tr>
    <tr>
      <td></td>
      <td>Stjørdal</td>
      <td>5035</td>
    </tr>
    <tr>
      <td></td>
      <td>Frosta</td>
      <td>5036</td>
    </tr>
    <tr>
      <td></td>
      <td>Levanger</td>
      <td>5037</td>
    </tr>
    <tr>
      <td></td>
      <td>Verdal</td>
      <td>5038</td>
    </tr>
    <tr>
      <td></td>
      <td>Verran (Utgått 2020-01-01)</td>
      <td>5039</td>
    </tr>
    <tr>
      <td></td>
      <td>Namdalseid (Utgått 2020-01-01)</td>
      <td>5040</td>
    </tr>
    <tr>
      <td></td>
      <td>Snåase – Snåsa</td>
      <td>5041</td>
    </tr>
    <tr>
      <td></td>
      <td>Lierne</td>
      <td>5042</td>
    </tr>
    <tr>
      <td></td>
      <td>Raarvikhe – Røyrvik</td>
      <td>5043</td>
    </tr>
    <tr>
      <td></td>
      <td>Namsskogan</td>
      <td>5044</td>
    </tr>
    <tr>
      <td></td>
      <td>Grong</td>
      <td>5045</td>
    </tr>
    <tr>
      <td></td>
      <td>Høylandet</td>
      <td>5046</td>
    </tr>
    <tr>
      <td></td>
      <td>Overhalla</td>
      <td>5047</td>
    </tr>
    <tr>
      <td></td>
      <td>Fosnes (Utgått 2020-01-01)</td>
      <td>5048</td>
    </tr>
    <tr>
      <td></td>
      <td>Flatanger</td>
      <td>5049</td>
    </tr>
    <tr>
      <td></td>
      <td>Vikna (Utgått 2020-01-01)</td>
      <td>5050</td>
    </tr>
    <tr>
      <td></td>
      <td>Nærøy (Utgått 2020-01-01)</td>
      <td>5051</td>
    </tr>
    <tr>
      <td></td>
      <td>Leka</td>
      <td>5052</td>
    </tr>
    <tr>
      <td></td>
      <td>Inderøy</td>
      <td>5053</td>
    </tr>
    <tr>
      <td></td>
      <td>Indre Fosen</td>
      <td>5054</td>
    </tr>
    <tr>
      <td></td>
      <td>Heim</td>
      <td>5055</td>
    </tr>
    <tr>
      <td></td>
      <td>Hitra</td>
      <td>5056</td>
    </tr>
    <tr>
      <td></td>
      <td>Ørland</td>
      <td>5057</td>
    </tr>
    <tr>
      <td></td>
      <td>Åfjord</td>
      <td>5058</td>
    </tr>
    <tr>
      <td></td>
      <td>Orkland</td>
      <td>5059</td>
    </tr>
    <tr>
      <td></td>
      <td>Nærøysund</td>
      <td>5060</td>
    </tr>
    <tr>
      <td></td>
      <td>Rindal</td>
      <td>5061</td>
    </tr>
    <tr>
      <td></td>
      <td>Tromsø</td>
      <td>5401</td>
    </tr>
    <tr>
      <td></td>
      <td>Harstad – Hárstták</td>
      <td>5402</td>
    </tr>
    <tr>
      <td></td>
      <td>Alta</td>
      <td>5403</td>
    </tr>
    <tr>
      <td></td>
      <td>Vardø</td>
      <td>5404</td>
    </tr>
    <tr>
      <td></td>
      <td>Vadsø</td>
      <td>5405</td>
    </tr>
    <tr>
      <td></td>
      <td>Hammerfest</td>
      <td>5406</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvæfjord</td>
      <td>5411</td>
    </tr>
    <tr>
      <td></td>
      <td>Tjeldsund</td>
      <td>5412</td>
    </tr>
    <tr>
      <td></td>
      <td>Ibestad</td>
      <td>5413</td>
    </tr>
    <tr>
      <td></td>
      <td>Gratangen</td>
      <td>5414</td>
    </tr>
    <tr>
      <td></td>
      <td>Loabák - Lavangen</td>
      <td>5415</td>
    </tr>
    <tr>
      <td></td>
      <td>Bardu</td>
      <td>5416</td>
    </tr>
    <tr>
      <td></td>
      <td>Salangen</td>
      <td>5417</td>
    </tr>
    <tr>
      <td></td>
      <td>Målselv</td>
      <td>5418</td>
    </tr>
    <tr>
      <td></td>
      <td>Sørreisa</td>
      <td>5419</td>
    </tr>
    <tr>
      <td></td>
      <td>Dyrøy</td>
      <td>5420</td>
    </tr>
    <tr>
      <td></td>
      <td>Senja</td>
      <td>5421</td>
    </tr>
    <tr>
      <td></td>
      <td>Balsfjord</td>
      <td>5422</td>
    </tr>
    <tr>
      <td></td>
      <td>Karlsøy</td>
      <td>5423</td>
    </tr>
    <tr>
      <td></td>
      <td>Lyngen</td>
      <td>5424</td>
    </tr>
    <tr>
      <td></td>
      <td>Storfjord - Omasvuotna - Omasvuono</td>
      <td>5425</td>
    </tr>
    <tr>
      <td></td>
      <td>Gáivuotna - Kåfjord - Kaivuono</td>
      <td>5426</td>
    </tr>
    <tr>
      <td></td>
      <td>Skjervøy</td>
      <td>5427</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordreisa - Ráisa - Raisi</td>
      <td>5428</td>
    </tr>
    <tr>
      <td></td>
      <td>Kvænangen</td>
      <td>5429</td>
    </tr>
    <tr>
      <td></td>
      <td>Guovdageaidnu - Kautokeino</td>
      <td>5430</td>
    </tr>
    <tr>
      <td></td>
      <td>Loppa</td>
      <td>5432</td>
    </tr>
    <tr>
      <td></td>
      <td>Hasvik</td>
      <td>5433</td>
    </tr>
    <tr>
      <td></td>
      <td>Måsøy</td>
      <td>5434</td>
    </tr>
    <tr>
      <td></td>
      <td>Nordkapp</td>
      <td>5435</td>
    </tr>
    <tr>
      <td></td>
      <td>Porsanger - Porsáŋgu - Porsanki</td>
      <td>5436</td>
    </tr>
    <tr>
      <td></td>
      <td>Kárášjohka - Karasjok</td>
      <td>5437</td>
    </tr>
    <tr>
      <td></td>
      <td>Lebesby</td>
      <td>5438</td>
    </tr>
    <tr>
      <td></td>
      <td>Gamvik</td>
      <td>5439</td>
    </tr>
    <tr>
      <td></td>
      <td>Berlevåg</td>
      <td>5440</td>
    </tr>
    <tr>
      <td></td>
      <td>Deatnu - Tana</td>
      <td>5441</td>
    </tr>
    <tr>
      <td></td>
      <td>Unjárga - Nesseby</td>
      <td>5442</td>
    </tr>
    <tr>
      <td></td>
      <td>Båtsfjord</td>
      <td>5443</td>
    </tr>
    <tr>
      <td></td>
      <td>Sør-Varanger</td>
      <td>5444</td>
    </tr>
    <tr>
      <td></td>
      <td>Svalbard</td>
      <td>2100</td>
    </tr>
  </tbody>
</table>
