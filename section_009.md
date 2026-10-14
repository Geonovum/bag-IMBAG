
# Implementatie {#3B455CCD}
<p>De Wet basisregistratie adressen en gebouwen stelt dat een afnemer BAG-gegevens kan afnemen bij zowel bronhouder als Landelijke Voorziening. Belangrijk uitgangspunt is daarbij dat de afnemer bij bronhouder en landelijke voorziening dezelfde gegevens krijgt.</p>
<br/>
<br/>
<p>Om die reden is het van belang om eisen vast te leggen aan de implementatie van bepaalde aspecten die worden toegevoegd bij de implementatie van het conceptuele model in een logisch model. Het logisch model is de basis voor het maken van berichtschema's (StUF) en applicatieschema's (NEN 3610) voor de uitwisseling van BAG-gegevens tussen bronhouders en landelijke voorziening en tussen landelijke voorziening en afnemers. Het betreft eisen aan de implementatie van historie (zie §<a href='#271B8B87'>9.1</a>), in onderzoek (zie § <a href='#720DB17B'>9.2</a>), en formele patronen om de consistentie van deze gegevens in de hele BAG-keten te borgen (zie § <a href='#5B35E175'>9.3</a>).</p>

## Historie {#271B8B87}
<p>In het conceptuele model wordt in de meta-gegevens opgenomen of een attribuut formele en materiële historie opbouwt, bijvoorbeeld het meta-gegeven 'indicatie formele historie' met waarde Ja. </p>
<br/>
<br/>
<p>De specificatie van formele en materiële historie uit het conceptuele model wordt vertaald naar een implementatie, bestaande uit bijbehorende attributen (tijdstippen). Deze implementatie vormt de basis voor de uitwisseling van BAG-gegevens (in bijvoorbeeld StUF of NEN 3610). Deze paragraaf beschrijft met welke attributen (tijdstippen) de BAG de formele en materiële historie implementeert en uitwisselt met de landelijke voorziening en welke aanvullende attributen (tijdstippen) worden bijgehouden in de landelijke voorziening voor de uitwisseling met afnemers.</p>
<br/>
<br/>
<p>Ook worden de regels vastgelegd voor het omgaan met object- en versiehistorie.</p>

### Materiële en formele historie {#21BD6A4F}
<p>De materiële en formele historie worden met de volgende tijdstippen geïmplementeerd in de BAG:</p>
<br/>
<br/>
<p><span style='color: #4472C4;'>Materiële historie</span></p>
<p><b>beginGeldigheid:</b></p>
<p>De datum waarop een versie van een BAG-object geldig is in de werkelijkheid conform de ingangsdatum in het brondocument. Dit tijdstip wordt vastgelegd in de <i>beginGeldigheid</i>. Als er geen expliciete ingangsdatum van geldigheid is opgenomen, wordt de datum van het brondocument overgenomen.</p>
<br/>
<br/>
<p><b>eindGeldigheid:</b></p>
<p>De datum waarop de periode van geldigheid van een versie van een BAG-object eindigt. Bijvoorbeeld als gevolg van de vaststelling van een nieuw brondocument. Wanneer er geen tijdstip is ingevuld, dan is de versie nog geldig. Dit tijdstip wordt vastgelegd in de <i>eindGeldigheid</i>.</p>
<br/>
<br/>
<p>De BAG legt materiële historie (<i>beginGeldigheid</i> en <i>eindGeldigheid</i>) en de datum van het brondocument (documentDatum) vast met de nauwkeurigheid van datum.</p>
<br/>
<br/>
<p><span style='color: #4472C4;'>Formele historie</span></p>
<p><b>tijdstipRegistratie:</b></p>
<p>Het tijdstip waarop een versie van een BAG-object is geregistreerd in de registratie van bronhouder en daarmee authentiek wordt gemaakt. Dit tijdstip wordt vastgelegd in de <i>tijdstipRegistratie</i>.</p>
<br/>
<br/>
<p><b>eindRegistratie:</b></p>
<p>Het tijdstip waarop een versie van een BAG-object is beëindigd in de registratie van bronhouder. Dit tijdstip wordt vastgelegd in de <i>eindRegistratie</i>.</p>
<br/>
<br/>
<p><b>tijdstipRegistratieLV:</b></p>
<p>Dit is het tijdstip waarop een versie van een BAG-object is opgenomen in de registratie van de landelijke voorziening. De gegevens komen daarmee beschikbaar voor afnemers. Dit tijdstip wordt vastgelegd in de <i>tijdstipRegistratieLV</i>.</p>
<br/>
<br/>
<p>De BAG legt formele historie (<i>tijdstipRegistratie</i> en <i>eindRegistratie</i>) en <i>tijdstipRegistratieLV</i> vast met de nauwkeurigheid van datum en tijd in uren, minuten, seconden en milliseconden.</p>

### Object- en versiehistorie {#721EFE6B}
<p>In de BAG ontstaan nieuwe BAG-objecten en worden gegevens van BAG-objecten in de tijd gewijzigd. Deze paragraaf beschrijft de te hanteren regels voor object- en versiehistorie.</p>
<br/>
<br/>
<p>Om historie goed bij te kunnen houden, moet elk object uniek aan te wijzen zijn, moet elke versie van elk object uniek aan te wijzen zijn en moet eenduidig vast te stellen zijn tot welk object een versie behoort. De unieke identificatie van een versie is daarom samengesteld uit de unieke 'objectidentificatie', in combinatie met een kenmerk 'versieidentificatie', die elke versie binnen de context van het object, uniek identificeert. Bijvoorbeeld: objectidentificatie 0100100000001234 en versie 1. De versie-identificatie is een integer, begint bij 1 en wordt steeds met 1 opgehoogd.</p>
<br/>
<br/>
<p>De volgende regels worden gehanteerd bij het ontstaan en wijzigen van een BAG-object:</p>
<ol><li>Als een nieuw BAG-object ontstaat, wordt een nieuw object met een objectidentificatie gecreëerd en ontstaat een versiehistorie. Deze eerste versie van het object krijgt een versie-identificatie 1, een <i>beginGeldigheid</i> en een <i>tijdstipRegistratie</i>.</li>
<li>Wanneer het object wordt geregistreerd in de landelijke voorziening krijgt het object ook een <i>tijdstipRegistratieLV</i>.</li>
<li>Als een attribuut van een object wijzigt, ontstaat er een nieuwe versie: de huidige versie krijgt van de bronhouder een <i>eindGeldigheid</i> en een <i>eindRegistratie</i>. Als een attribuut van een object wijzigt, ontstaat er een nieuwe versie: de vorige versie krijgt van de bronhouder een <i>eindGeldigheid</i>, die aansluit op de <i>beginGeldigheid</i> van de nieuwe versie, en een <i>eindRegistratie</i>.</li>
</ol>
<br/>
<br/>
<p>De bronhouder maakt een nieuwe versie van het object met de nieuwe gegevens aan conform het besluit (brondocument). De nieuwe versie van het object krijgt een unieke versie-identificatie, een <i>beginGeldigheid</i> en een <i>tijdstipRegistratie</i>, waarbij <i>beginGeldigheid</i> gelijk is aan <i>eindGeldigheid</i> van de vorige versie en <i>tijdstipRegistratie</i> gelijk is aan de <i>eindRegistratie</i> van de vorige versie. Na registratie van deze versie van het object in de landelijke voorziening krijgt deze versie van het object een eigen <i>tijdstipRegistratieLV</i>.</p>
<br/>
<br/>
<p>De versie-identificatie is een nummer. Voor een nieuw toe te kennen identificatie wordt altijd het eerstvolgende beschikbare nummer gekozen. Als het eerstvolgende nummer al in gebruik is bij een niet-authentieke versie van een object, dan is deze niet als uniek gegeven beschikbaar en wordt het eerstvolgende wel beschikbare nummer gekozen.</p>
<br/>
<br/>
<p>De identificatie en versie-identificatie samen bepalen een unieke versie van een object. De bronhouder levert altijd de actuele versie van een object aan de landelijke voorziening. Het is niet toegestaan om gegevens te wijzigen die op het moment van wijzigen niet meer geldig zijn.</p>

### Levenscyclus {#742C62A7}
<p>De levenscyclus van een object in de BAG bestaat uit alle versies van een object. Dit zijn alle actieve en alle inactieve versies. Een actieve versie is een versie waarvan tijdstipInactief niet ingevuld is. Een inactieve versie is een versie waarvan tijdstipInactief wel ingevuld is.</p>
<br/>
<br/>
<p>Alleen de gegevens van de actieve versies tellen mee bij de beantwoording van vragen ten aanzien van welke gegevens er geldig zijn. Gegevens in versies die aangemerkt zijn als inactief tellen niet meer mee (maar deden dat eerder wel, toen ze nog actief waren).</p>
<br/>
<br/>
<p><span style='color: #4472C4;'>Actieve levenscyclus</span></p>
<p>De actieve levenscyclus van een object in de BAG bestaat uit alle actieve versies van een object. De volgende regels gelden voor de actieve levenscyclus:</p>
<ol><li>De beginGeldigheid van een versie kan in het verleden of in de toekomst liggen. Wanneer de beginGeldigheid in de toekomst ligt, dan zijn deze gegevens wel geldig, maar nog niet in werking getreden. </li>
<li>Objecten worden in de registratie beëindigd door een eindstatus, zoals Pand gesloopt toe te kennen. Er zal dus altijd een geldige versie blijven bestaan, met een open einddatum.</li>
<li>Op elk moment in de tijd is er één geldige versie in de levenscyclus van een object. Dat wil zeggen: </li>
<li>De geldigheidsperiode loopt vanaf de beginGeldigheid tot de eindGeldigheid. Beide zijn een datum, omdat besluiten ingaan op een bepaalde dag, niet op een bepaald tijdstip.</li>
<li>De eindGeldigheid van een versie sluit naadloos aan op de beginGeldigheid van de volgende versie, door hiervoor altijd dezelfde datum te gebruiken. Bijvoorbeeld: versie 1 met eindGeldigheid 1-1-2018 zal aansluiten op een versie 2 met beginGeldigheid 1-1-2018.</li>
<li>De eindGeldigheid moet geïnterpreteerd worden als geldig tot datum (niet tot en met), oftewel tot het moment dat de volgende versie (met een versie-identificatie dat met 1 wordt opgehoogd) ingaat. Bijvoorbeeld: versie 1 met eindGeldigheid 1-1-2018 heeft een versie 2 met beginGeldigheid 1-1-2018.</li>
<li>Er mogen geen gaten zitten in de tijdslijn. Bijvoorbeeld: een versie met eindGeldigheid 31-12-2017 en een volgende versie met begindatum 2-1-2018. Er is dan een gat op 1-1-2018.</li>
<li>Er mag geen overlap zitten in de tijdslijn. Bijvoorbeeld: een versie met eindGeldigheid 2-1-2018 en een volgende versie met beginGeldigheid 1-1-2018. Op 1-1-2018 zijn dan twee versies tegelijk geldig. (Let op het volgende punt!)</li>
<li>Er kunnen meerdere geldige versies geldig zijn op één dag. Meerdere versies hebben dan dezelfde beginGeldigheid en er is dan een versie met dezelfde beginGeldigheid als de eindGeldigheid. De laatste versie van de dag is dan leidend, herkenbaar aan het hoogste versie-identificatie. Bijvoorbeeld: versie 3 heeft een beginGeldigheid 31-12018 en eindGeldigheid 31-1-2018. Versie 4 heeft een begindatum 31-1-2018 en een open (geen) einddatum. Op 31-1-2018 zijn er twee versies geldig, met elk beginGeldigheid 31-1-2018. Versie 4 heeft het hoogste versie-identificatie en is dus leidend. Versie 3 is en blijft wel geldig. Aan de formele historie, oftewel tijdstipRegistratie en eindRegistratie van versie 3, is te zien wanneer en hoe lang de materiële gegevens van deze versie 3 formeel geldig zijn geweest.</li>
</ol>
<br/>
<br/>
<p><span style='color: #4472C4;'>Gegevens buiten de actieve levenscyclus plaatsen</span></p>
<p>Er zijn situaties waarin een bronhouder een besluit (brondocument) intrekt of herziet. Bijvoorbeeld omdat een besluit beschrijft dat bepaalde gegevens in de toekomst ingaan en er een nieuw besluit wordt genomen die beschrijft dat deze gegevens toch niet in zullen gaan, bijvoorbeeld er wordt besloten om toch een andere straatnaam te hanteren alvorens de eerder besloten straatnaam in werking treedt.</p>
<br/>
<br/>
<p>Zowel het eerste besluit als het laatste besluit zijn brondocument voor de BAG en worden opgevoerd in de BAG-registratie van de bronhouder en aangeleverd aan de landelijke voorziening. Echter, alleen de gegevens van het laatste besluit zullen op enig moment in werking treden, omdat de eerdere gegevens zijn ingetrokken voor de inwerkingtreding.</p>
<br/>
<br/>
<p>Op deze manier kunnen gegevens waarvan de datum beginGeldigheid in de toekomst ligt, buiten de actieve levenscyclus worden geplaatst door de bronhouder, wat wordt aangeduid met de term 'inactief maken'. De bronhouder dient daarbij ook de voorgaande (actieve) versie inactief te maken om een geldige materiële tijdslijn te waarborgen.</p>
<br/>
<br/>
<p>Op het moment dat een bronhouder een versie van een object uit de actieve levenscyclus wil halen, kent de bronhouder een tijdstip (datum en tijd) toe aan het optionele attribuut tijdstipInactief met het moment waarop de bronhouder besluit om deze versie inactief te maken.</p>
<br/>
<br/>
<p>Naast het opgeven van een tijdstipInactief voor de gegevens waarvan de beginGeldigheid in de toekomst ligt, geeft de bronhouder ook voor de voorgaande versie van het object aan dat deze inactief wordt door een datum en tijd te specificeren voor tijdstipInactief. Doordat de versie van het object daar weer voor een eindGeldigheid datum heeft, die niet in de toekomst maar in het verleden ligt, kan er een nieuwe versie worden opgevoerd met een lege eindGeldigheid (de nieuwe actieve en geldige versie).</p>
<br/>
<br/>
<p>Met het opnemen van het attribuut Inactief met een datum-tijd wordt kenbaar gemaakt dat deze versie van het object inactief is. Na het inactief maken van een versie ontstaat er een nieuwe levenscyclus, waar de versie die inactief is gemaakt nog steeds wel deel van uitmaakt. De inactieve versie maakt echter geen deel meer uit van de actieve levenscyclus. Als het attribuut Inactief niet voorkomt bij een versie van een object, dan behoren deze gegevens tot de actieve levenscyclus van het object.</p>

### Samenvatting {#3CF424C5}
<p>Deze paragraaf geeft een samenvatting van de beschrijvingen in paragrafen 9.1.1, 9.1.2 en 9.1.3 van de implementatie van historie in de BAG (zie <a href='#d6aIcFbC'>Tabel 124</a>).</p>
<table id='d6aIcFbC' style='width: 100%;'><caption>Overzicht implementatie historie BAG</caption>
<colgroup><col id='col1-d6aIcFbC' style='width: 25%;'>
<col id='col2-d6aIcFbC' style='width: 25%;'>
<col id='col3-d6aIcFbC' style='width: 18.785871964679913%;'>
<col id='col4-d6aIcFbC' style='width: 31.214128035320087%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4C4E22B2'>Attribuut</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6C95DDCE'>Kardinaliteit</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4C6B0B31'>Type</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='41992B3F'>Opmaak</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6A930982'>versie-identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='25E0C035'>[1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3A3A6E05'>Integer</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7B1B2478'>beginGeldigheid</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='5B52F9FE'>[1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='194D5C6B'>Date</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='47DF31DD'>jjjj-dd-mm</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='112A77DF'>eindGeldigheid</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='25455717'>[0..1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='702AE638'>Date</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='38CEDC85'>jjjj-dd-mm</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='46FB9CD0'>tijdstipRegistratie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3DBBA69D'>[1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='62F3A0B6'>DateTime</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3769517E'>jjjj-dd-mmTuu:mm:ss.sss</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='58D76FA7'>eindRegistratie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='5BE332D5'>[0..1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3621F510'>DateTime</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4FC33EED'>jjjj-dd-mmTuu:mm:ss.sss</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='34231783'>tijdstipRegistratieLV</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4149C233'>[0..1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='45ABEE8D'>DateTime</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6FEB70C2'>jjjj-dd-mmTuu:mm:ss.sss</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='79FF7B05'>tijdstipInactief</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='591F6FD7'>[0..1]</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='26128338'>DateTime</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2F40B557'>jjjj-dd-mmTuu:mm:ss.sss</p></td>
</tr>
</tbody>
</table>


## In onderzoek {#720DB17B}
<p>In § <a href='#0E4B2924'>4.8</a> wordt beschreven welke attributen en relaties van objecten in onderzoek geplaatst kunnen worden. In deze paragraaf wordt gespecificeerd op welke wijze in onderzoek moet worden geïmplementeerd in een logisch model IMBAG.</p>
<br/>
<br/>
<p>In onderzoek wordt geïmplementeerd middels een object Onderzoek. In dit objecttype worden de volgende gegevens van een inonderzoekplaatsing vastgelegd:</p>
<ol><li>De identificatie van het object dat in onderzoek is geplaatst.</li>
<li>De naam van het kenmerk of de attribuutsoort of de relatiesoort van het object dat in onderzoek is geplaatst. Per object kunnen bepaalde attributen en relaties in onderzoek worden geplaatst conform § <a href='#0E4B2924'>4.8</a> van deze catalogus.</li>
<li>Het nummer van het document waarin de grondslag van het onderzoek wordt vastgelegd. Dit wordt vastgelegd in het attribuut documentnummer.</li>
<li>De datum van het document waarin de grondslag van het onderzoek wordt vastgelegd. Dit wordt vastgelegd in het attribuut documentnummer.</li>
<li>De datum waarop het attribuut van een object bij bronhouder in onderzoek is geplaatst. Dit behoort tot de materiële historie van het object Onderzoek en wordt vastgelegd in het attribuut beginGeldigheid (datum).</li>
<li>De datum waarop het onderzoek naar het attribuut door bronhouder is afgerond. Dit behoort tot de materiële historie en wordt vastgelegd in het attribuut eindGeldigheid (datum).</li>
<li>Het tijdstip waarop het onderzoek is geregistreerd bij de bronhouder. Dit behoort tot de formele historie van het object Onderzoek en wordt vastgelegd in het attribuut tijdstipRegistratie (datum/tijd).</li>
<li>Het tijdstip waarop de registratie van het onderzoek is beëindigd bij de bronhouder. Dit behoort tot de formele historie van het object Onderzoek en wordt vastgelegd in het attribuut eindRegistratie (datum/tijd).</li>
<li>Het tijdstip waarop het onderzoek is geregistreerd in de landelijke voorziening. Dit wordt vastgelegd in het attribuut tijdstipRegistratieLV (datum/tijd).</li>
</ol>

## Formele patronen {#5B35E175}
<p>In hoofdstuk 5 en hoofdstuk 8 worden de patronen van attributen in mensleesbare taal</p>
<br/>
<br/>
<p>beschreven. Om interpretatieverschillen en inconsistentie in de BAG-keten te voorkomen specificeert <a href='#d6aIeBe'>Tabel 125</a> deze patronen als formele patronen met behulp van reguliere expressies.</p>
<table id='d6aIeBe' style='width: 100%;'><caption>Formele patronen</caption>
<colgroup><col id='col1-d6aIeBe' style='width: 20.868008005899082%;'>
<col id='col2-d6aIeBe' style='width: 14.916254081955124%;'>
<col id='col3-d6aIeBe' style='width: 37.332771515853786%;'>
<col id='col4-d6aIeBe' style='width: 26.88296639629201%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3104B00A'>Objecttype</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1BE2371E'>Attribuut</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='50693850'>Mensleesbare taal</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6FA23AAA'>Formeel patroon</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='5B53DC27'>Woonplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3B31ADD1'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7BE6091B'>Een natuurlijk getal tussen 0001 en 9999</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='42F85D60'>^[0-9]{3}[1-9] \ | [0-9]{2}[1-9][09] \ | [0-9][1-9][09]{2} \ | [1-9][0-9] {3}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='523A9F30'>Openbare ruimte</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2DF9DA1E'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='65317708'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Tabellen BRP), het(tweecijferig) subdomein 'objecttypecode' en een voor het betreﬀende objecttype binnen een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='35B04858'>^[0-9] {4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='71233EA1'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7026A02B'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='14DB913A'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Tabellen BRP), het (tweecijferig) subdomein 'objecttypecode' en een voor het betreﬀende objecttype binnen een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='465F1E6F'>^[0-9]{4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='16AF00BE'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='52BC3291'>huisnummer</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='18ECD1B3'>Een natuurlijk getal tussen 1 en 99999</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='50357E84'>^[1-9] [0-9] {0,4}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4AC04816'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4D9A52ED'>huisletter</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='346C2D42'>Een hoofdletter (A – Z) of kleine letter (a – z)</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='35110AAE'>^[a-zA-Z]{1}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7077C1AE'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3D4E34D6'>Huisnummer-toevoeging</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7C4DBCB2'>Maximaal vier alfanumerieke tekens bestaande uit een combinatie van hoofdletters (A – Z), kleine letters (a – z) en/of cijfers (0 – 9)</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4D4CF964'>^[0-9azA-Z] {1,4}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='62947E27'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='75B88D22'>postcode</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='440B51EE'>Combinatie van vier cijfers (0 – 9) en twee hoofdletters (A – Z)</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0152E59E'>^[1-9] [0-9]{3} [A-Z]{2}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='72A45463'>Pand</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='254645F0'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='13F5D84A'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Tabellen BRP), het (tweecijferig) subdomein  'objecttypecode' en een voor het betreﬀende objecttype binnen een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='59774907'>^[0-9] {4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='45946361'>Ligplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='68B54971'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0DCF5FA7'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Tabellen BRP), het (tweecijferig) subdomein 'objecttypecode' en een voor het betreﬀende objecttype binnen  een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='679536D9'>^[0-9] {4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='23D1F228'>Standplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4843BC27'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6995F2EA'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Gemeententabel van de Landelijke Tabellen BRP), het (tweecijferig) subdomein 'objecttypecode' en een voor het betreﬀende objecttype binnen een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3894F78A'>^[0-9] {4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='201463A2'>Verblijfsobject</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='493EF9B8'>identificatie</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0FFEE6B5'>Combinatie van het (viercijferig) subdomein 'gemeentecode' (volgens Tabel 33 Gemeententabel van de Landelijke Tabellen BRP), het (tweecijferig) subdomein 'objecttypecode' en een voor het betreﬀende objecttype binnen een gemeente uniek (tiencijferig) subdomein 'objectvolgnummer'</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='40E55F95'>^[0-9] {4}[0-9] {2}[0-9] {10}$</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='779A5FA6'>Verblijfsobject</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='785451AC'>oppervlakte</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='55CE22C0'>Een natuurlijk getal tussen 1 en 999999</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='601815E9'>^[1-9] [0-9] {0,5}$</p></td>
</tr>
</tbody>
</table>

