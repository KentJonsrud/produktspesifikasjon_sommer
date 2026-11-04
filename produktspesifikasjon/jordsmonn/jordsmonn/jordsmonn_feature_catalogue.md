#### JordsmonnGrense

grensen for jordsmonnflata<br />-- Definition --<br />the boundary of an expanse of soil

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>grense</td>
      <td>forløp som følger overgang mellom ulike fenomener<br />-- Definition --<br />course follwing the transition between different real world phenomena</td>
      <td>GM_<wbr />Curve</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

#### Jordsmonn

geografisk område med tilnærmet enhetlige egenskaper i jordsmonnet<br />-- Definition --<br />geographic area with approximately uniform soil characteristics

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>område</td>
      <td>objektets utstrekning<br />-- Definition --<br />area over which an object extends</td>
      <td>GM_<wbr />Surface</td>
      <td>1</td>
    </tr>
    <tr>
      <td>dominerende<wbr />Tekstur<wbr />Overflatesjikt</td>
      <td>Viser arealets dominerende tekstur (og grusinnhold) i overflatesjikt registrert under jordkartlegging i felt.<br />-- Definition --<br />category for the dominant texture in the surface layer recorded during fieldwork.</td>
      <td><a href="#kodeliste-dominerendeteksturoverflatesjikt">Dominerende<wbr />Tekstur<wbr />Overflatesjikt</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>forstyrrelser</td>
      <td>Viser hva slags menneskelig aktivitet, utover vanlig jordarbeiding/grøfting, som har forstyrret arealet.</td>
      <td><a href="#kodeliste-forstyrrelser">Forstyrrelser</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>helling</td>
      <td>Viser dominerende helling på arealet.<br />-- Definition --<br />inclination class for the soil figure</td>
      <td><a href="#kodeliste-helling">Helling</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>jordsmonnklassifikasjon</td>
      <td>Viser hvilken jordgruppe som dominerer på arealet<br />-- Definition --<br />Shows which soiltype which is dominating the area.</td>
      <td><a href="#kodeliste-jordsmonnklassifikasjon">Jordsmonnklassifikasjon</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kartleggingsmetodikk</td>
      <td>Viser hvilken opprinnelig kartleggingsmetodikk som er brukt under jordsmonnkartlegging.<br />--Definition--<br />Displays the methodolgy used during field mapping.</td>
      <td><a href="#kodeliste-kartleggingsmetodikk">Kartleggingsmetodikk</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kartleggingsår</td>
      <td>Viser årstall for når jordsmonnkartlegging er utført.<br />-- Definition --<br />year of mapping</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>mest<wbr />Begrensende<wbr />Jordegenskap</td>
      <td>Viser den jordegenskapen som er mest begrensende for bruken av arealet</td>
      <td><a href="#kodeliste-mestbegrensendejordegenskap">Mest<wbr />Begrensende<wbr />Jordegenskap</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>naturlige<wbr />Dreneringsforhold</td>
      <td>Viser jordsmonnets naturlige evne til å bli kvitt overflødig vann.</td>
      <td><a href="#kodeliste-naturligedreneringsforhold">Naturlige<wbr />Dreneringsforhold</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>organisk<wbr />Materiale</td>
      <td>Viser jordsmonnets innhold av organisk materiale i overflatesjiktet, samt tykkelse på organisk jord der denne finnes.</td>
      <td><a href="#kodeliste-organiskmateriale">Organisk<wbr />Materiale</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>stein<wbr />Blokk</td>
      <td>Viser stein- og blokkinnhold (0–50 cm) på arealet på kartleggingstidspunktet</td>
      <td><a href="#kodeliste-steinblokk">Stein<wbr />Blokk</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>tilleggsinformasjon</td>
      <td>Viser tilleggsinformasjon om andre egenskaper ved arealet.</td>
      <td><a href="#kodeliste-tilleggsinformasjon">Tilleggsinformasjon</a><br />(kodeliste)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>opprinnelig<wbr />Lokal<wbr />Id</td>
      <td>Opprinnelig id i databasen<br />— Definition —<br />Original ID in the soil database</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr class="inherited-from">
      <th colspan="4" scope="rowgroup">Arvet fra Jordsmonn_Fellesegenskaper</th>
    </tr>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kopidata</td>
      <td>angivelse av at objektet er hentet fra et kopidatasett og ikke fra originaldatasettet<br /><br />Merknad: Inneholder informasjon om når kopidatasettet ble kopiert fra originaldatasettet og hvem som er originaldataansvarlig</td>
      <td>Kopidata<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- område<wbr />Id</td>
      <td>identifikasjon av område som dataene dekker<br />Merknad: Kan angis med kommunenummer eller fylkesnummer. Disse bør spesifiseres nærmere.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- original<wbr />Datavert</td>
      <td>ansvarlig etat for forvaltning av data</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- kopidato</td>
      <td>dato når objektet ble kopiert fra originaldatasettet<br /><br />Merknad:<br />Er en del av egenskapen Kopidata. Brukes i de tilfeller hvor en kopidatabase brukes til distribusjon.<br />Å kopiere et datasett til en kopidatabase skal ikke føre til at Oppdateringsdato blir endret.<br />Eventuell redigering av data i et kopidatasett medfører ny Oppdateringsdato, Datafangstdato og/eller Verifiseringsdato.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Beskrivelse av kvaliteten på stedfestingen.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>verifiseringsdato</td>
      <td>dato når dataene er fastslått å være i samsvar med virkeligheten<br />Merknad: Verifiseringsdato er identisk med ..DATO i tidligere versjoner av SOSI</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
Jordsmonn_Fellesegenskaper

**Assosiasjoner**
JordsmonnGrense – rolle: avgrensesAvJordsmonngrense – kardinalitet: 0..*

#### Jordsmonn_Fellesegenskaper (abstrakt)

abstrakt objekttype som bærer sentrale egenskaper som er anbefalt for bruk i produktspesifikasjoner.<br />Merknad: Disse egenskapene skal derfor ikke modelleres inn i fagområdemodeller.

Egenskaper

<table class="feature-attribute-table">
  <thead>
    <tr>
      <th>Egenskap</th>
      <th>Beskrivelse</th>
      <th>Type</th>
      <th>Multiplisitet</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>identifikasjon</td>
      <td>unik identifikasjon av et objekt</td>
      <td>Identifikasjon<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- lokal<wbr />Id</td>
      <td>lokal identifikator av et objekt<br />Merknad: Det er dataleverendørens ansvar å sørge for at den lokale identifikatoren er unik innenfor navnerommet.</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- navnerom</td>
      <td>navnerom som unikt identifiserer datakilden til et objekt, anbefales å være en http-URI<br />Eksempel: <a href="http://data.geonorge.no/SentraltStedsnavnsregister/1.0">http://data.geonorge.no/SentraltStedsnavnsregister/1.0</a><br />Merknad : Verdien for nanverom vil eies av den dataprodusent som har ansvar for de unike identifikatorene og må være registrert i data.geonorge.no eller data.norge.no</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kopidata</td>
      <td>angivelse av at objektet er hentet fra et kopidatasett og ikke fra originaldatasettet<br /><br />Merknad: Inneholder informasjon om når kopidatasettet ble kopiert fra originaldatasettet og hvem som er originaldataansvarlig</td>
      <td>Kopidata<br />(datatype)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- område<wbr />Id</td>
      <td>identifikasjon av område som dataene dekker<br />Merknad: Kan angis med kommunenummer eller fylkesnummer. Disse bør spesifiseres nærmere.</td>
      <td>Integer</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- original<wbr />Datavert</td>
      <td>ansvarlig etat for forvaltning av data</td>
      <td>Character<wbr />String</td>
      <td>1</td>
    </tr>
    <tr>
      <td>- kopidato</td>
      <td>dato når objektet ble kopiert fra originaldatasettet<br /><br />Merknad:<br />Er en del av egenskapen Kopidata. Brukes i de tilfeller hvor en kopidatabase brukes til distribusjon.<br />Å kopiere et datasett til en kopidatabase skal ikke føre til at Oppdateringsdato blir endret.<br />Eventuell redigering av data i et kopidatasett medfører ny Oppdateringsdato, Datafangstdato og/eller Verifiseringsdato.</td>
      <td>Date<wbr />Time</td>
      <td>1</td>
    </tr>
    <tr>
      <td>kvalitet</td>
      <td>Beskrivelse av kvaliteten på stedfestingen.</td>
      <td>Posisjonskvalitet<br />(datatype)</td>
      <td>0..1</td>
    </tr>
    <tr>
      <td>- målemetode</td>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
      <td><a href="#kodeliste-målemetode">Målemetode</a><br />(kodeliste)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>verifiseringsdato</td>
      <td>dato når dataene er fastslått å være i samsvar med virkeligheten<br />Merknad: Verifiseringsdato er identisk med ..DATO i tidligere versjoner av SOSI</td>
      <td>Date<wbr />Time</td>
      <td>0..1</td>
    </tr>
  </tbody>
</table>

### Kodelister

#### <a id="kodeliste-dominerendeteksturoverflatesjikt"></a>«CodeList» DominerendeTeksturOverflatesjikt

**Definisjon:** Viser arealets dominerende tekstur (og grusinnhold) i overflatesjikt registrert under jordkartlegging i felt.
-- Definition - -
category for the dominant texture in the surface layer recorded during fieldwork.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/dominerendeteksturoverflatesjikt">https://register.geonorge.no/sosi-kodelister/jordsmonn/dominerendeteksturoverflatesjikt</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-forstyrrelser"></a>«CodeList» Forstyrrelser

**Definisjon:** Viser hva slags menneskelig aktivitet, utover vanlig jordarbeiding/grøfting, som har forstyrret arealet.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/forstyrrelser">https://register.geonorge.no/sosi-kodelister/jordsmonn/forstyrrelser</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-helling"></a>«CodeList» Helling

**Definisjon:** Viser dominerende helling på arealet.
-- Definition --
inclination class for the soil figure

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/helling">https://register.geonorge.no/sosi-kodelister/jordsmonn/helling</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-jordsmonnklassifikasjon"></a>«CodeList» Jordsmonnklassifikasjon

**Definisjon:** Viser hvilken jordgruppe som dominerer på arealet
-- Definition --
Shows which soiltype which is dominating the area.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/jordsmonnklassifikasjon">https://register.geonorge.no/sosi-kodelister/jordsmonn/jordsmonnklassifikasjon</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-kartleggingsmetodikk"></a>«CodeList» Kartleggingsmetodikk

**Definisjon:** Viser hvilken opprinnelig kartleggingsmetodikk som er brukt under jordsmonnkartlegging.
--Definition--
Displays the methodolgy used during field mapping.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/kartleggingsmetodikk">https://register.geonorge.no/sosi-kodelister/jordsmonn/kartleggingsmetodikk</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-mestbegrensendejordegenskap"></a>«CodeList» MestBegrensendeJordegenskap

**Definisjon:** Viser den jordegenskapen som er mest begrensende for bruken av arealet

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/mestbegrensendejordegenskap">https://register.geonorge.no/sosi-kodelister/jordsmonn/mestbegrensendejordegenskap</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-naturligedreneringsforhold"></a>«CodeList» NaturligeDreneringsforhold

**Definisjon:** Viser jordsmonnets naturlige evne til å bli kvitt overflødig vann.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/naturligedreneringsforhold">https://register.geonorge.no/sosi-kodelister/jordsmonn/naturligedreneringsforhold</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-organiskmateriale"></a>«CodeList» OrganiskMateriale

**Definisjon:** Viser jordsmonnets innhold av organisk materiale i overflatesjiktet, samt tykkelse på organisk jord der denne finnes.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/organiskmateriale">https://register.geonorge.no/sosi-kodelister/jordsmonn/organiskmateriale</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-steinblokk"></a>«CodeList» SteinBlokk

**Definisjon:** Viser stein- og blokkinnhold (0–50 cm) på arealet på kartleggingstidspunktet

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/steinblokk">https://register.geonorge.no/sosi-kodelister/jordsmonn/steinblokk</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-tilleggsinformasjon"></a>«CodeList» Tilleggsinformasjon

**Definisjon:** Viser tilleggsinformasjon om andre egenskaper ved arealet.

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/jordsmonn/tilleggsinformasjon">https://register.geonorge.no/sosi-kodelister/jordsmonn/tilleggsinformasjon</a></td>
    </tr>
  </tbody>
</table>

#### <a id="kodeliste-målemetode"></a>«CodeList» Målemetode

**Definisjon:** metode som ligger til grunn for registrering av posisjon
-- Definition - -
method on which registration of position is based

Profilparametre i tagged values

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">asDictionary</th>
      <td>true</td>
    </tr>
    <tr>
      <th scope="row">codeList</th>
      <td><a href="https://register.geonorge.no/sosi-kodelister/generelle-konsepter/4.5/m%C3%A5lemetodekode">https://register.geonorge.no/sosi-kodelister/generelle-konsepter/4.5/m%C3%A5lemetodekode</a></td>
    </tr>
  </tbody>
</table>
