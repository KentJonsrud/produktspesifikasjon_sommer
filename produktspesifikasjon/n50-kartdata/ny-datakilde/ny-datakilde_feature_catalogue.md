#### SOSI_Objekt_PunkterOgLinjer (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er til felles for flere objekttyper med punkt- eller linjegeometri i underpakkene Administrative områder, Arealdekke, Bygninger og anlegg, Restriksjonsområder og Samferdsel i dette applikasjonsskjemaet

Egenskaper

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
      <td>dato for siste endring på objektetdataene<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>kvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse av kvaliteten på stedfestingen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjonskvalitet</td>
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
      <td><strong>kvalitet.målemetode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Målemetode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Genererte data Generalisering – Genererte data: Generalisering</td>
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
      <td><strong>kvalitet.nøyaktighet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Nøyaktighet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- 100000 – Nøyaktigheten varierer med +/-1000 m</td>
    </tr>
  </tbody>
</table>

#### SOSI_Objekt_Hjelpelinjer (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er til felles for KantUtsnitt, Dataavgrensning og FiktivDelelinje i dette applikasjonsskjemaet

Egenskaper

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
      <td>dato for siste endring på objektetdataene<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

#### Dataavgrensning

generell avgrensningslinje, f.eks. mellom datasett med ulik kvalitet, innhold eller detaljering

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Hjelpelinjer

#### SOSI_Objekt_Linjer_Samferdsel (abstrakt)

abstrakt objekt som bærer en rekke egenskaper som er til felles for flere objekttyper i underpakke Samferdsel i dette applikasjonsskjemaet

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>medium</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets beliggenhet i forhold til jordoverflaten<br /><br />Eksempel:<br />På bro, i tunnel, inne i et bygningsmessig anlegg, etc.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>MediumSamferdsel</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/mediumsamferdsel">https://register.geonorge.no/sosi-kodelister/kartdata/mediumsamferdsel</a></td>
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
      <td>dato for siste endring på objektetdataene<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>kvalitet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse av kvaliteten på stedfestingen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Posisjonskvalitet</td>
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
      <td><strong>kvalitet.målemetode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>metode for måling i grunnriss (x,y), og høyde (z) når metoden er den samme som ved måling i grunnriss</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Målemetode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Genererte data Generalisering – Genererte data: Generalisering</td>
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
      <td><strong>kvalitet.nøyaktighet</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>punktstandardavviket i grunnriss for punkter samt tverravvik for linjer<br /><br />Merknad:<br />Oppgitt i cm</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Nøyaktighet</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- 100000 – Nøyaktigheten varierer med +/-1000 m</td>
    </tr>
  </tbody>
</table>

#### KantUtsnitt

avgrensning av et utsnitt

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Hjelpelinjer

#### SOSI_Objekt_Flater (abstrakt)

abstrakt supertype som samler fellesegenskaper og assosiasjoner som gjelder objekttyper som bare har flategeometri

Egenskaper

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
      <td>dato for siste endring på objektetdataene<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Assosiasjoner**
KantUtsnitt – rolle: avgrensesAvKantUtsnitt – kardinalitet: 0..*

#### FiktivDelelinje

linje for å dele opp store flateobjekter<br /><br />Merknad:<br />En del produktspesifikasjoner benytter spesifikke fiktive delelinjer.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Hjelpelinjer

#### Territorialgrense

avgrensning i havet av statens suverenitetsområde, beregnet 12 nm (22 224 m) utenfor og parallelt med grunnlinjen

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Grunnlinje

rette linjer trukket opp mellom punkter på de ytterste nes og skjær som stikker opp av havet ved lavvann (fjære sjø)<br /><br />Merknad:<br />Med rett linje forstås den korteste linje mellom to punkt (såkalt geodetisk linje).

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Kommune

inndeling i administrative og politiske enheter innenfor fylket<br /><br />Merknad: Tilsvarer NUTS 5 og LAU 2 på internasjonalt statistisk nivå

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
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
      <td>nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste<br /><br />Merknad: Det presiseres at kommune alltid skal ha 4 siffer, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 siffer.<br /><br />-- Definition - -<br />numbering of municipalities in accordance with Statistics Norway’s official list<br />Note: It must be following that municipality number always consists of 4 digits, i.e. sometimes with leading zero. Municipality is used for establishing relations to a number of other registers which also use 4 digits.</td>
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
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer">https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer</a></td>
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
      <td>offisielt navn på kommunen</td>
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
      <td><strong>fylkesnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste</td>
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
      <td><strong>fylkesnavn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>offisielt navn på fylket</td>
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
SOSI_Objekt_Flater

**Assosiasjoner**
Territorialgrense – rolle: avgrensesAvTerritorialgrense – kardinalitet: 0..*
Riksgrense – rolle: avgrensesAvRiksgrense – kardinalitet: 0..*
Kommunegrense – rolle: avgrensesAvKommunegrense – kardinalitet: 0..*
Fylkesgrense – rolle: avgrensesAvFylkesgrense – kardinalitet: 0..*

#### Fylkesgrense

avgrensning av fylke

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Kommunegrense

avgrensing av kommune

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Riksgrense

avgrensningen av nasjonen Norge mot andre nasjoner<br /><br />Merknad:<br />Delvis avledet fra norsk svensk riksgrensemodell<br /><br />--Definition--<br />delimitation of the country of Norway over against other countries Note:Partially derived from the Norwegian-Swedish national boundary model

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Lufthavn

land- eller sjøområde (med bygninger, installasjoner og utstyr) som helt eller delvis brukes for luftfartøyers avgang, landing og annen manøvrering på bakken

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
      <td>sted som objektet eksisterer på</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
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
      <td><strong>lufthavntype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse av type lufthavn</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Lufthavntype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/lufthavntype">https://register.geonorge.no/sosi-kodelister/kartdata/lufthavntype</a></td>
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
      <td><strong>trafikktype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>beskrivelse av rutetrafikk</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Trafikktype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/trafikktype">https://register.geonorge.no/sosi-kodelister/kartdata/trafikktype</a></td>
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
      <td><strong>iataKode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>unik kode for lufthavner.<br /><br />Merknad1: Ikke alle lufthavner har IATA kode.<br />Merknad 2: Bare norske lufthavner er tatt med her.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>IATAKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/iatakode">https://register.geonorge.no/sosi-kodelister/kartdata/iatakode</a></td>
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
      <td><strong>icaoKode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse av lufthavn ved kode på fire alfanumeriske tegn.<br /><br />Merknad: Den første bokstaven tilordnes etter kontinent og angir et land eller en gruppe land på det samme kontinentet. Den andre bokstaven angir landet og de to siste angir lufthavn.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>ICAOKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/icaokode">https://register.geonorge.no/sosi-kodelister/kartdata/icaokode</a></td>
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
      <td><strong>lufthavneier</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>eier av lufthavn</td>
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
      <td><strong>navn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på flyplass<br /><br />Merknad: Benyttes spesielt for de flyplasser som ikke har IATA eller ICAO kode</td>
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

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### ElvBekk

mindre vannvei for rennende vann representert ved senterlinje

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>senterlinje</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger objektets sentrale del<br /><br />-- Definition --<br />cource follwed by the central part of the object</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Arealbrukgrense

avgrensning av de ulike arealbruksflatene<br /><br />Merknad:<br />Kode for bruken av arealet legges på flaten, dvs på representasjonspunktet der dette representerer flata.<br /><br /><br />-- Definition --<br />delimitation of the various land use areas Note: Land use code is assigned to the surface, i.e. on the representation point which represents this surface.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Havflate

havområde som avgrenses av Kystkontur, Kystsperre, HavElvSperre og KystkonturTekniskAnlegg<br /><br /><br />-- Definition --<br />sea area which is delimited by Coastline, CoastDelineation, SeaRiverDelineation and ShorelineConstruction

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning<br /><br />-- Definition --<br />area over which an object extends</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Flater

**Assosiasjoner**
Dataavgrensning – rolle: avgrensesAvDataavgrensning – kardinalitet: 0..*
FiktivDelelinje – rolle: avgrensesAvFiktivDelelinje – kardinalitet: 0..*
Kystkontur – rolle: avgrensesAvKystkontur – kardinalitet: 0..*

#### Kystkontur

grense mellom land og sjø, definert som midlere høyvannslinje<br /><br />Merknad:<br />Tilsvarer COALNE i S-57<br /><br /><br />-- Definition --<br />boundary between land and sea, defined as the mean high water line Note: Corresponds to COALNE in S-57

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener<br /><br />-- Definition --<br />course follwing the transition between different real world phenomena</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Innsjøkant

konturlinje mellom land og innsjø<br /><br /><br />-- Definition --<br />Demarkation line between land and lake surface.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener<br /><br />-- Definition --<br />course follwing the transition between different real world phenomena</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Skog

alle typer skogsmark som barskog, lauvskog og blandingsskog<br /><br />Merknad: Også hogstflater - selv om nyplanting ikke er synlig.  Omfatter alle slags skogboniteter, også storvokste vierkrattbelter i Nord-Norge<br /><br /><br />-- Definition --<br />all types of forest land, such as coniferous forest, deciduous forest and mixed forest

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning<br /><br />-- Definition --<br />area over which an object extends</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Flater

**Assosiasjoner**
Dataavgrensning – rolle: avgrensesAvDataavgrensning – kardinalitet: 0..*
FiktivDelelinje – rolle: avgrensesAvFiktivDelelinje – kardinalitet: 0..*
Arealbrukgrense – rolle: avgrensesAvArealbrukgrense – kardinalitet: 0..*
Kystkontur – rolle: avgrensesAvKystkontur – kardinalitet: 0..*
Innsjøkant – rolle: avgrensesAvInnsjøkant – kardinalitet: 0..*

#### ÅpentOmråde

område som ikke er klassifisert som annet tema i henhold til gjeldende produktspesifikasjon

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Flater

**Assosiasjoner**
Dataavgrensning – rolle: avgrensesAvDataavgrensning – kardinalitet: 0..*
FiktivDelelinje – rolle: avgrensesAvFiktivDelelinje – kardinalitet: 0..*
Arealbrukgrense – rolle: avgrensesAvArealbrukgrense – kardinalitet: 0..*
Kystkontur – rolle: avgrensesAvKystkontur – kardinalitet: 0..*
Innsjøkant – rolle: avgrensesAvInnsjøkant – kardinalitet: 0..*

#### SnøIsbre

grense mellom snø eller isbre og barmark der det er usikkert om det er isbre eller snø<br /><br /><br />Merknad:<br />Isbre kan også være en del av evig snø, særlig når breens kantlinje ikke kan defineres (og registreres) som Isbre.  Den gamle koden for isbre er overført til dette objektet !<br /><br /><br />-- Definition --<br />Snow or glacier and bare ground where it is uncertain if it is snow or glacier. Note: A snowfield can also be a part of perpetual snow, especially when the glacier's edge cannot be defined and registered as a glacier.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning<br /><br />-- Definition --<br />area over which an object extends</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Flater

**Assosiasjoner**
Dataavgrensning – rolle: avgrensesAvDataavgrensning – kardinalitet: 0..*
FiktivDelelinje – rolle: avgrensesAvFiktivDelelinje – kardinalitet: 0..*
Arealbrukgrense – rolle: avgrensesAvArealbrukgrense – kardinalitet: 0..*
Kystkontur – rolle: avgrensesAvKystkontur – kardinalitet: 0..*
Innsjøkant – rolle: avgrensesAvInnsjøkant – kardinalitet: 0..*

#### Tettbebyggelse

sammenhengende bebygd område (overveiende boligbegyggelse) hvor husene i hovedsak ligger tettere enn 50 meter<br /><br /><br />-- Definition --<br />continuous, developed area (predominantly residential) where the buildings, for the most part, are closer than 50 metres apart

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
      <td>sted som objektet eksisterer på</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
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
      <td><strong>tettbebyggelsestype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>Klassifisering av tettbebyggelse etter innbyggertall</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Tettbebyggelsestype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/tettbebyggelsestype">https://register.geonorge.no/sosi-kodelister/kartdata/tettbebyggelsestype</a></td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Innsjø

en ferskvannsflate som ikke er renndende vann<br /><br /><br />-- Definition --<br />Freshwater surface which is not running water.

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning<br /><br />-- Definition --<br />area over which an object extends</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
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
      <td><strong>høyde</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>registrert høyde for vannspeilet.</td>
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
SOSI_Objekt_Flater

**Assosiasjoner**
Dataavgrensning – rolle: avgrensesAvDataavgrensning – kardinalitet: 0..*
FiktivDelelinje – rolle: avgrensesAvFiktivDelelinje – kardinalitet: 0..*
Innsjøkant – rolle: avgrensesAvInnsjøkant – kardinalitet: 0..*

#### Naturverngrense

avgrenser et naturvernområde

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>grense</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger overgang mellom ulike fenomener</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### Naturvernområde

naturvernområde

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>område</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>objektets utstrekning</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Surface</td>
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
      <td><strong>vernedato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for vern av området</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>verneform</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>ulike type vern sortert under forskjellige lovverk og med tilhørende restriksjoner</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Verneform</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/verneform">https://register.geonorge.no/sosi-kodelister/kartdata/verneform</a></td>
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
      <td><strong>navn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på naturvernområdet</td>
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
SOSI_Objekt_Flater

**Assosiasjoner**
Naturverngrense – rolle: avgrensesAvNaturverngrense – kardinalitet: 0..*

#### Bane

teoretisk linje som representerer ett enkelt eller flere parallelle spor som del av en banestrekning<br /><br /><br />-- Definition --<br />theoretical line which represents a single or several parallel tracks as part of a railway line<br /><br /><br />-- INSPIRE --<br />Maps to RailwayLink

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>senterlinje</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger objektets sentrale del</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Linjer_Samferdsel

#### Veglenke

Objekttype som representerer lenker i vegnettet<br />Eksempel: NVDB Referanselenkedeler

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>senterlinje</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger objektets sentrale del</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
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
      <td><strong>typeVeg</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>type veg</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TypeVeg</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/typeveg">https://register.geonorge.no/sosi-kodelister/kartdata/typeveg</a></td>
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
      <td><strong>vegsystem</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>definerer hvilke deler av vegnettet som forvaltningsmessig hører sammen</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vegsystem</td>
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
      <td><strong>vegsystem.vegkategori</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kategorisering som angir på hvilket nivå vegmyndigheten for strekningen ligger</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vegkategori</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/vegkategori">https://register.geonorge.no/sosi-kodelister/kartdata/vegkategori</a></td>
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
      <td><strong>vegsystem.vegfase</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angir vegens fase i livet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Vegfase</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/vegfase">https://register.geonorge.no/sosi-kodelister/kartdata/vegfase</a></td>
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
      <td><strong>vegsystem.vegnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angir hvilke deler av vegnettet som rutemessig hører sammen</td>
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
      <td><strong>motorvegtype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>klassifisering av veger etter grad av vilkår med hensyn til f.eks. fart, avkjøringer/kryss og antall kjørefelt</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Motorvegtype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/motorvegtype">https://register.geonorge.no/sosi-kodelister/kartdata/motorvegtype</a></td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_Linjer_Samferdsel

#### Stasjon

representasjonspunkt for stasjon, holdeplass eller godsterminal<br /><br /><br />-- Definition --<br />representation point for station, stopping place or freight terminal

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
      <td>sted som objektet eksisterer på<br /><br />-- Definition --<br />location where the object exists</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Point</td>
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
      <td><strong>navn</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navn på stasjon<br /><br />-- Definition --<br />name of a station</td>
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
SOSI_Objekt_PunkterOgLinjer

#### AnnenBåtrute

båtrute som ikke kan karakteriseres som passasjer- eller bilferje<br /><br /><br />-- Definition --<br />boat route which cannot be characterised as passenger ferry or car ferry

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>senterlinje</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>forløp som følger objektets sentrale del</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
    </tr>
  </tbody>
</table>

Relasjoner

**Arv**
SOSI_Objekt_PunkterOgLinjer

#### StedsnavnTekst

Stedsnavntekst er stedsnavn fra SSR tilpasset visning på kart

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>navneobjekthovedgruppe</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>hovedgruppene følger i hovedsak Inspire "NamedPlaceTypeValue", men populatedPlace og building er samlet under bebyggelse og hydrography er delt mellom sjø og ferskvann.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Navneobjekthovedgruppe</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekthovedgruppe">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekthovedgruppe</a></td>
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
      <td><strong>navneobjektgruppe</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>inndeling i kategorier under hver hovedgruppe.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Navneobjektgruppe</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjektgruppe">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjektgruppe</a></td>
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
      <td><strong>navneobjekttype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>stedets navneobjekttype er en underinndeling av navneobjektgruppene som igjen er inndeling av navneobjekthovedgruppene.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Navneobjekttype</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekttype">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekttype</a></td>
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
      <td><strong>språk</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angir hvilket språk teksten hører til, norsk, kvensk, nordsamisk, lulesamisk, sørsamisk osv.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>SpråkKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kkode">https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kkode</a></td>
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
      <td><strong>stedsnavnnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>stedsnummer, stedsnavnnummer og skrivemåtenummer skal sammen utgjøre en såkalt tematisk id som brukes av registerførere som opplslagsnummer. identifikatoren ligner litt på Gnr/Bnr/Fnr.<br /><br />Stedsnavnnummer er et løpende nummer (starter på 1) systemet gir stedsnavnet som en identifikator. stedsnavnnummeret er kun unikt under ett stedsnummer og kan ikke brukes om igjen for dette stedet.</td>
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
      <td><strong>språkprioritering</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>stedsnavnet sin prioritering i forhold til de ulike språkgruppene</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>SpråkprioriteringKode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kprioriteringkode">https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kprioriteringkode</a></td>
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
      <td><strong>stedsnummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>stedsnummer, stedsnavnsnummer og skrivemåtenummer skal sammen utgjøre en såkalt tematisk id som brukes av registerførere som opplslagsnummer. Identifikatoren ligner litt på Gnr/Bnr/Fnr.<br /><br />Stedsnummeret er et løpende nummer systemet gir stedet som en identifikator. Stedsnummeret er unikt og kan ikke brukes om igjen.</td>
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
      <td><strong>skrivemåtenummer</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>stedsnummer, stedsnavnsnummer og skrivemåtenummer skal sammen utgjøre en såkalt tematisk id som brukes av registerførere som opplslagsnummer. Identifikatoren ligner litt på Gnr/Bnr/Fnr.<br /><br />Skrivemåtenummer er et løpende nummer systemet gir skrivemåten som en identifikator. skrivemåtenummeret er kun unikt under ett stedsnavnsnummer og kan ikke brukes om igjen for dette stedsnavnet.</td>
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
FellesTekst

#### FellesTekst (abstrakt)

abstrakt objekt som bærer en felles egenskaper som brukes på tekstobjektene

Egenskaper

<table class="feature-attribute-table">
  <colgroup>
    <col style="width: 35%;" />
    <col style="width: 65%;" />
  </colgroup>
  <tbody>
    <tr>
      <th scope="row">Navn:</th>
      <td><strong>geometri</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>kurve-geometri på tekstobjekter brukes slik: Punkt nr. 1 på kurva er objektets referansekoordinat. Punkt nr. 2 er tekstens plasseringskoordinat. Punkt nr. 3 angir retning på teksten. Dersom kurva inneholder flere koordinater angir disse forløp på teksten.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>GM_Curve</td>
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
      <td><strong>streng</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>teksten som skal presenteres på kartet</td>
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
      <td><strong>oppdateringsdato</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>dato for siste endring på objektetdataene<br /><br />-Definition-<br />Date and time at which this version of the spatial object was inserted or changed in the spatial data set.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Date</td>
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
      <td><strong>tekstformatering</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>ulike egenskaper til brukt for å presentere teksten på mediumet</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Tekstformatering</td>
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
      <td><strong>tekstformatering.tekstReferansepunkt</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>tekstens referansepunkt er det stedet på teksten hvor en tekstplassering refererer seg til.</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TekstReferansePunkt</td>
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
      <td><strong>tekstformatering.tekstReferansepunkt.tekstReferansePunktNord</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>vertikal plassering av teksten.<br />Merknad: N50 Kartdata plasseres alltid teksten langs bunnlinja, dvs. TRNORD = 0</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TekstReferansePunktNord</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunktnord">https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunktnord</a></td>
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
      <td><strong>tekstformatering.tekstReferansepunkt.tekstReferansePunktØst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>horisontal plassering av teksten</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>TekstReferansePunktØst</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunkt%C3%B8st">https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunkt%C3%B8st</a></td>
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
      <td><strong>tekstformatering.tegnavstand</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>avstanden mellom bokstavene i teksten, enhet er prosent</td>
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
      <td><strong>tekstformatering.skriftkode</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>produktavhengig koplingsnøkkel mot presentasjonsinformasjon</td>
    </tr>
    <tr>
      <th scope="row">Multiplisitet:</th>
      <td>0..1</td>
    </tr>
    <tr>
      <th scope="row">Type:</th>
      <td>Skriftkode</td>
    </tr>
    <tr>
      <th scope="row">Tillatte verdier:</th>
      <td>- Kodeliste: <a href="https://register.geonorge.no/sosi-kodelister/kartdata/skriftkode">https://register.geonorge.no/sosi-kodelister/kartdata/skriftkode</a></td>
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
      <td><strong>tekstformatering.skrifttype</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>angivelse av den skrifttype eller font som skal benyttes. Default skrifttype er ARIAL<br />Merknad: For samiske tegn anbefales SK Sans Serif, nedlastbart fra Statens kartverks nettsider</td>
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
      <td><strong>tekstformatering.referansemålestokk</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>egenskap som beskriver hvilken målestokk (oppgitt som målestokkstall) denne teksten er redigert for, både størrelse og<br />plassering. Kan benyttes for å velge hvilke tekster som skal tegnes ut i ulike målestokker.</td>
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
      <td><strong>fulltekst</strong></td>
    </tr>
    <tr>
      <th scope="row">Definisjon:</th>
      <td>navnet i SSR som skal vises på kartet. Vil i de fleste tilfeller være likt Streng, men kan avvike dersom det av kartografiske hensyn bare vises deler av navnet e.l.</td>
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

### Kodelister

#### «Enumeration» Målemetode

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
      <td>false</td>
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
      <td>Genererte data Generalisering</td>
      <td>Genererte data: Generalisering</td>
      <td></td>
    </tr>
  </tbody>
</table>

#### «Enumeration» Nøyaktighet

**Definisjon:** punktstandardavviket i grunnriss for punkter samt tverravvik for linjer

Merknad:
Oppgitt i cm

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
      <td>Nøyaktigheten varierer med +/-1000 m</td>
      <td>100000</td>
    </tr>
  </tbody>
</table>

#### «CodeList» MediumSamferdsel

**Definisjon:** objektets beliggenhet i forhold til jordoverflaten

Eksempel:
Veg på bro, i tunnel, inne i et bygningsmessig anlegg, etc.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/mediumsamferdsel">https://register.geonorge.no/sosi-kodelister/kartdata/mediumsamferdsel</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Kommunenummer

**Definisjon:** nummerering av kommuner i henhold til Statistisk sentralbyrå sin offisielle liste samt et utvalg av utgåtte numre

Merknad: Det presiseres at kommune alltid skal ha 4 sifre, dvs. eventuelt med ledende null. Kommune benyttes for kopling mot en rekke andre registre som også benytter 4 sifre.

Merknad 2: Modelleringsverktøyet Enterprise Architect håndterer ikke samiske tegn eller tankestrek. Det betyr at det vil forekomme avvik mellom definisjonene i denne lista i SOSI modellregister og definisjonene i offisielt standarddokument.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer">https://register.geonorge.no/sosi-kodelister/inndelinger/inndelingsbase/kommunenummer</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Lufthavntype

**Definisjon:** angivelse av type lufthavn

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/lufthavntype">https://register.geonorge.no/sosi-kodelister/kartdata/lufthavntype</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Trafikktype

**Definisjon:** angivelse av type rutetrafikk

Merknad: Benyttes i N50 Kartdata i forhold til luftfart

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/trafikktype">https://register.geonorge.no/sosi-kodelister/kartdata/trafikktype</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» IATAKode

**Definisjon:** unik kode for lufthavner.

Merknad1: Ikke alle lufthavner har IATA kode.
Merknad 2: Bare norske lufthavner er tatt med her.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/iatakode">https://register.geonorge.no/sosi-kodelister/kartdata/iatakode</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» ICAOKode

**Definisjon:** angivelse av lufthavn ved &lt;a href="C:\\wiki\\Kode"&gt;&lt;font color="#0000ff"&gt;&lt;u&gt;kode&lt;/u&gt;&lt;/font&gt;&lt;/a&gt; på fire &lt;a href="C:\\w\\index.php?title=Alfanumerisk&amp;action=edit&amp;redlink=1"&gt;&lt;font color="#0000ff"&gt;&lt;u&gt;alfanumeriske&lt;/u&gt;&lt;/font&gt;&lt;/a&gt; &lt;a href="C:\\wiki\\Tegn"&gt;&lt;font color="#0000ff"&gt;&lt;u&gt;tegn&lt;/u&gt;&lt;/font&gt;&lt;/a&gt;.

Merknad: Den første bokstaven tilordnes etter kontinent og angir et land eller en gruppe land på det samme kontinentet. Den andre bokstaven angir landet og de to siste angir lufthavn.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/icaokode">https://register.geonorge.no/sosi-kodelister/kartdata/icaokode</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Tettbebyggelsestype

**Definisjon:** Klassifisering av tettbebyggelse etter innbyggertall

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/tettbebyggelsestype">https://register.geonorge.no/sosi-kodelister/kartdata/tettbebyggelsestype</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Verneform

**Definisjon:** verneformer som sorterer under forskjellig lovverk og restriksjoner

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/verneform">https://register.geonorge.no/sosi-kodelister/kartdata/verneform</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» TypeVeg

**Definisjon:** type veg

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/typeveg">https://register.geonorge.no/sosi-kodelister/kartdata/typeveg</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Vegkategori

**Definisjon:** kategorisering som angir på hvilket nivå vegmyndigheten for strekningen ligger

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/vegkategori">https://register.geonorge.no/sosi-kodelister/kartdata/vegkategori</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Vegfase

**Definisjon:** angir vegens fase i livet

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/vegfase">https://register.geonorge.no/sosi-kodelister/kartdata/vegfase</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Motorvegtype

**Definisjon:** klassifisering av veger etter grad av vilkår med hensyn til f.eks. fart, avkjøringer/kryss og antall kjørefelt

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/motorvegtype">https://register.geonorge.no/sosi-kodelister/kartdata/motorvegtype</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Navneobjekthovedgruppe

**Definisjon:** hovedgruppene følger i hovedsak Inspire "NamedPlaceTypeValue", men populatedPlace og building er samlet under bebyggelse og hydrography er delt mellom sjø og ferskvann.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekthovedgruppe">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekthovedgruppe</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Navneobjektgruppe

**Definisjon:** inndeling i kategorier under hver hovedgruppe.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjektgruppe">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjektgruppe</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Navneobjekttype

**Definisjon:** stedets navneobjekttype er en underinndeling av navneobjektgruppene som igjen er inndeling av navneobjekthovedgruppene.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekttype">https://register.geonorge.no/sosi-kodelister/stedsnavn/navneobjekttype</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» SpråkKode

**Definisjon:** subsett av ISO 639-3 som inneholder trebokstavs-koder de språkene som trengs for å konvertere innholdet fra SSR. Kodelisten kan utvides ved behov etter produksjonssetting.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kkode">https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kkode</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» SpråkprioriteringKode

**Definisjon:** kodeliste som angir visningsrekkefølgen til stedsnavn på forskjellig språk.

Det er de første fem verdiene i kodene (de norske språkene) som varierer mellom kodene, ellers er det lik (alfabetisk i forhold til ISO-kodeverdien) rekkefølge på språkene som ikke er aktuelle for behandling etter lov om stadnamn.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kprioriteringkode">https://register.geonorge.no/sosi-kodelister/stedsnavn/spr%C3%A5kprioriteringkode</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» TekstReferansePunktNord

**Definisjon:** vertikal plassering av teksten

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunktnord">https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunktnord</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» TekstReferansePunktØst

**Definisjon:** horisontal plassering av teksten

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunkt%C3%B8st">https://register.geonorge.no/sosi-kodelister/kartdata/tekstreferansepunkt%C3%B8st</a></td>
    </tr>
  </tbody>
</table>

#### «CodeList» Skriftkode

**Definisjon:** koblingsnøkkel mot presentasjonsinformasjon. Forslag til presentasjon av stedsnavn og høydetall basert på skriftkoder. Presentasjonskoden er basert på hovedkartserien 1:50 000/M711 produsert av Kartverket. Kartverket har egne fonter, men oversatt til TimesNewRoman slik at enhver kan presentere dataene tilnærmet presentasjonen til Kartverket. Ved bruk av ESRI FGDB filformat ligger fontinformasjon allerede inne i egenskapstabellen.

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
      <td><a href="https://register.geonorge.no/sosi-kodelister/kartdata/skriftkode">https://register.geonorge.no/sosi-kodelister/kartdata/skriftkode</a></td>
    </tr>
  </tbody>
</table>
