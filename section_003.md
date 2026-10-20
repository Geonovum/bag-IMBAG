
# Algemene principes {#559231F8}
<p id='560E4419'>Dit hoofdstuk beschrijft algemene principes die gelden voor de inhoud van de BAG.</p>

<p id='3910AB80'>Deze algemene principes hebben betrekking op:</p>
<ul><li>bronhouders (zie §<a href='#73B2A517'>3.1</a>);</li>
<li>coördinatenstelsel (zie §<a href='#6640BE1A'>3.2</a>);</li>
<li>geometrie en oppervlakte (zie §<a href='#3C6054E3'>3.3</a>);</li>
<li>relaties tussen BAG-objecten (zie §<a href='#02B253FB'>3.4</a>);</li>
<li>topologie (zie §<a href='#48C73D30'>3.5</a>);</li>
<li>levenscyclus (zie §<a href='#3688B20B'>3.6</a>);</li>
<li>identificatie en historie (zie §<a href='#4FF275BF'>3.7</a>);</li>
<li>gebruiksdoel (zie §<a href='#1E54126F'>3.8</a>).</li>
</ul>

## Bronhouders {#73B2A517}
<p id='017A5C4B'>Elke gemeente is bronhouder van de BAG binnen de eigen gemeentegrenzen. Het grondgebied van de gemeente waarop een object is gelegen, bepaalt dus welke gemeente het object registreert. Het maakt hierbij geen verschil als gerelateerde objecten in een andere gemeente liggen en daarom een andere bronhouder hebben. De nummeraanduiding wordt opgevat als eigenschap van een adresseerbaar object en geregistreerd in de gemeente waarin het adresseerbare object is gelegen. In het bijzondere geval dat een pand of verblijfsobject is gelegen op de grens van twee of meer gemeenten, worden dat pand en de eventuele verblijfsobjecten geregistreerd in de gemeente op wier grondgebied het grootste gedeelte van het pand is gelegen.</p>

## Coördinatenstelsel {#6640BE1A}
<p id='704A387F'>Het toegepaste coördinatenstelsel voor de BAG is dat van de Rijksdriehoeksmeting (Rdstelsel<span class='noot'>[8]<span class='noottekst'>Het stelsel van de Rijksdriehoeksmeting (RD) is het coördinatensysteem van Nederland. http://www.kada ster.nl/web/Themas/Registraties/Rijksdriehoeksmeting/Rijksdriehoeksstelsel.htm<br/>
</span></span>). De coördinaten zijn op de millimeter nauwkeurig en de eenheid is meter. Elk coördinaat heeft maximaal drie decimalen. Zo nodig wordt daarvoor afgerond, zodanig dat als de vierde decimaal de waarde 0, 1, 2, 3 of 4 heeft, de derde decimaal niet wijzigt en als de vierde decimaal de waarde 5, 6, 7, 8 of 9 heeft, de derde decimaal met één wordt verhoogd. Als de op te hogen decimaal de waarde 9 had (en dus 10 zou moeten worden), herhaalt deze regel zich voor de voorliggende decimalen. Bijvoorbeeld een coördinaat 155004,329098765 komt in de BAG als 155004.329 en een coördinaat 155004,329598765 als 155004.330.</p>

## Geometrie en oppervlakte {#3C6054E3}
<p id='1745F4AF'>Deze paragraaf beschrijft algemene principes die gelden voor de inhoud van de BAG en die betrekking hebben op geometrie (zie §<a href='#25E05EE3'>3.3.1</a>) en op gebruiksoppervlakte (zie §<a href='#3DB002BE'>3.3.2</a>).</p>

### Geometrie {#25E05EE3}
<p id='298BDFBA'>De geometrie is een eigenschap van vijf van de zeven BAG-objecttypen. Deze geometrie betreft het loodrechte bovenaanzicht van het object met de ware vorm, afmeting en oriëntatie en positie ten opzichte van de aarde, inclusief alle zichtbare en onzichtbare delen boven en onder de grond, maar exclusief alle delen die kunnen bewegen ten opzichte van de aarde.</p>

<p id='127D70F3'>De geometrische representatie van de objecttypen in de BAG, waaronder de geldige geometrietypen, de geldige ruimtelijke dimensies van de geometrie en de geldige ruimtelijke dimensies van de coördinaten van de geometrie, is afhankelijk van het objecttype (zie <a href='#d6aCeCbE'>Tabel 1</a>).</p>
<table id='d6aCeCbE' style='width: 100%;'><caption><span class='tblno'>Tabel 1</span>   De geometrische representatie van de objecttypen in de BAG</caption>
<colgroup><col id='col1-d6aCeCbE' style='width: 25%;'>
<col id='col2-d6aCeCbE' style='width: 25%;'>
<col id='col3-d6aCeCbE' style='width: 25%;'>
<col id='col4-d6aCeCbE' style='width: 25%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='753DDCFB'>Objecttype</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='61537BF9'>Geometrietype</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='5AC7E3C9'>Dimensie van de geometrie</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='417A782D'>Dimensie van de coördinaten</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3537B679'>Nummeraanduiding</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='35601168'>n.v.t.</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='41888744'>n.v.t.</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2DBA164B'>n.v.t.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='374C38EB'>Openbare ruimte</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='02306159'>n.v.t.</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='15133BDF'>n.v.t.</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1DEC97C2'>n.v.t.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='01691057'>Woonplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='36A48F41'>Vlak of multivlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='62188C8D'>2D</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='62D4DDA7'>2D</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3EDC9ED1'>Ligplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='30C580C2'>Vlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='23E95B3C'>2D</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4A5DCE95'>2D</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='092732F5'>Pand</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3FDA83B2'>Vlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3CFB2153'>2D</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='093A48F1'>2D of 3D</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3BA89176'>Standplaats</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4CE133D5'>Vlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='768E55A8'>2D</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4D7901B8'>2D</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6437F23E'>Verblijfsobject</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='515510E9'>Punt of vlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4776930F'>0D of 2D</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2AF48D2D'>2D of 3D</p></td>
</tr>
</tbody>
</table>

<p id='65DAE457'>De geometrie van openbare ruimten is niet opgenomen in de BAG. De gemeente dient het bij het benoemen van nieuwe openbare ruimten alsmede bij het wijzigen van bestaande openbare ruimten een voldoende gedetailleerde omschrijving of grafische weergave op te nemen die de ligging van de buitenruimte op enigerlei wijze aanwijst. De ligging van openbare ruimten is dus wel opgenomen in het brondocument, maar niet in de BAG-registratie.</p>

<p id='2088346B'>De geometrie van nummeraanduidingen is niet opgenomen in de BAG. De nummeraanduidingen worden opgevat als eigenschap van een adresseerbaar object, waarvan de geometrie wel is opgenomen in de BAG.</p>

<p id='73AF1E97'>De geometrie van een BAG-object heeft tweedimensionale coördinaten bij de objecttypen Woonplaats, Standplaats en Ligplaats en allemaal twee- of allemaal driedimensionale coördinaten bij de objecttypen Pand en Verblijfsobject. Dit geldt voor elke geldige ruimtelijke dimensie van de geometrie. Elke vlakgeometrie moet een plat vlak zonder enige kromming (oftewel: planair) zijn, ook als deze driedimensionale coördinaten heeft.</p>

<p id='05A313DD'>Voor de beschrijving van geometrieën geldt het ISO 19107 Spatial Schema. Voor de beschrijving van geometrieën geldt het ISO 19107 Spatial Schema. Voor de uitwisseling wordt gebruik gemaakt van Geography Markup Language (GML) versie 3.1.1. In de BAG zijn de geometrieën conform het Simple Features profile versie 1.0 toegestaan<span class='noot'>[9]<span class='noottekst'>Open Geospatial Consortium (2011, 2012) Geography Markup Language (GML) simple features profile (with Corrigendum), OGC® 10-100r3. https://portal.opengeospatial.org/files/?artifact_id=42729<br/>
</span></span>. Voor de representatie van boogvormen wordt de benadering van de boog met lineaire lijnsegmenten toegepast, de zogenaamde gestrookte boog. De geometrietypen worden in het informatiemodel met hun ISO 19107-naam aangeduid (zie <a href='#d6aCeCbO'>Tabel 2</a>).</p>
<table id='d6aCeCbO' style='width: 100%;'><caption><span class='tblno'>Tabel 2</span>   De geometrietypen in de BAG</caption>
<colgroup><col id='col1-d6aCeCbO' style='width: 50%;'>
<col id='col2-d6aCeCbO' style='width: 50%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='533B7F52'>BAG-benaming</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2C904116'>ISO 19107-naam</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4E054260'>Punt</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3AD035BE'>GM_Point</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='07AA3CFC'>Vlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='28F2328A'>GM_Surface</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='327D9AA4'>Multivlak</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='17A24E30'>GM_MultiSurface</p></td>
</tr>
</tbody>
</table>


### Gebruiksoppervlakte {#3DB002BE}
<p id='2DF2154D'>De bepaling van de gebruiksoppervlakte van een verblijfsobject geschiedt conform hetgeen in NEN 2580:2007 is vastgelegd omtrent gebruiksoppervlakte. Tot de oppervlakte van een verblijfsobject wordt uitsluitend gerekend de binnenruimte, zoals gedefinieerd in NEN 2580:2007, van een dergelijk object. In afwijking van NEN 2580:2007 maken gemeenschappelijke ruimten geen onderdeel uit van de oppervlakte van een verblijfsobject. Er dienen dus geen percentages van de oppervlakte van gemeenschappelijke ruimten te worden toegerekend aan de oppervlakte van een verblijfsobject. Als basisvoorzieningen zich bevinden in een of meer nabijgelegen ondersteunende binnenruimten die geen deel uitmaken van een verblijfsobject maar wel exclusief ondersteunend zijn aan dat verblijfsobject (zie stap 2 van § <a href='#129B35EA'>10.8</a>), dan tellen de gebruiksoppervlakten van deze nabijgelegen binnenruimten met basisvoorzieningen mee voor de gebruiksoppervlakte van het verblijfsobject.</p>

## Relaties tussen BAG-objecten {#02B253FB}
<p id='077E7211'>De objecten in de BAG zijn onderling sterk aan elkaar gerelateerd. De relatie naar een ander object wordt gevormd door een verwijzing naar het identificerende attribuut. Bijvoorbeeld het identificerende attribuut van een woonplaats is de identificatie.</p>

<p id='1C5F739E'>De BAG kent de volgende relaties tussen objecten:</p>
<ul><li>Openbare ruimte: <ul><li>Een openbare ruimte ligt in een woonplaats en heeft daartoe een verwijzing naar de gerelateerde woonplaats.</li>
</ul>
</li>
</ul>

<ul><li>Nummeraanduiding: <ul><li>Een nummeraanduiding is gelegen aan een openbare ruimte en heeft daartoe een verwijzing naar deze gerelateerde openbare ruimte. Op het moment dat een object is gelegen in een andere woonplaats dan de openbare ruimte waaraan de nummeraanduiding is gerelateerd, heeft de nummeraanduiding een verwijzing naar de gerelateerde Woonplaats. Een nummeraanduiding mag niet bestaan zonder het bijbehorende verblijfsobject of de bijbehorende standplaats of ligplaats. </li>
</ul>
</li>
</ul>

<ul><li>Standplaats of ligplaats: <ul><li>Een standplaats of ligplaats heeft één adres als hoofdadres en daartoe een verwijzing naar een gerelateerde nummeraanduiding, zijnde het hoofdadres. Een standplaats of ligplaats heeft eventueel een of meer adressen als nevenadres en in dat geval een verwijzing naar een of meer nummeraanduidingen, zijnde het nevenadres of de nevenadressen (zie §<a href='#66034D93'>10.2</a>).</li>
</ul>
</li>
</ul>

<ul><li>Verblijfsobject: <ul><li>Een verblijfsobject heeft één adres als hoofdadres en daartoe een verwijzing naar een gerelateerde nummeraanduiding, zijnde het hoofdadres. Een verblijfsobject heeft eventueel een of meer adressen als nevenadres en in dat geval een verwijzing naar een of meer nummeraanduidingen, zijnde het nevenadres of de nevenadressen (zie §<a href='#66034D93'>10.2</a>). Een verblijfsobject is gelegen in een of meer panden en heeft daartoe een verwijzing naar een of meer gerelateerde panden.</li>
</ul>
</li>
</ul>

<p id='30C544CC'>Bij een woonplaats of pand wordt geen identificatie naar een gerelateerd BAG-object opgenomen.</p>

<p id='290EE719'>Panden hoeven geen verblijfsobjecten te bevatten. Op het moment dat er binnen een pand geen verblijfsobjecten aanwezig zijn (bijvoorbeeld een schuur in de tuin van een woning), zal dit dus betekenen dat er sprake is van een pand zonder daarbinnen gelegen verblijfsobjecten.</p>

<p id='2C63A6CC'>Hiermee ontstaat een situatie dat er verschillende soorten relaties tussen panden en verblijfsobjecten kunnen bestaan. <a href='#d6aCfBaa'>Tabel 3</a> laat zien welke situaties mogelijk zijn. In deze tabel staat <i>n</i> voor twee of meer panden en <i>m</i> voor twee of meer verblijfsobjecten.</p>

<table id='d6aCfBaa' style='width: 100%;'><caption><span class='tblno'>Tabel 3</span>   De mogelijke relaties tussen panden en verblijfsobjecten</caption>
<colgroup><col id='col1-d6aCfBaa' style='width: 20%;'>
<col id='col2-d6aCfBaa' style='width: 20%;'>
<col id='col3-d6aCfBaa' style='width: 60%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='61B75276'>Pand</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='50E361B1'>Verblijfsobject</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3E27A190'>Omschrijving</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3E08E9B0'>1</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='76F9E943'>0</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='6C76B7DB'>Een pand zonder verblijfsobjecten. De situatie waarin een gebouw ondersteunend is aan een hoofdgebouw en alleen als zodanig van belang is, zonder dat het een zelfstandige eenheid van gebruik is. Een pand zonder verblijfsobject heeft geen adres.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1EE0A9B1'>1</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2BDABB7A'>1</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0156F870'>Een pand met één verblijfsobject. Dit is een veel voorkomende situatie bij bijvoorbeeld vrijstaande woningen en eengezinswoningen.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1EAECB26'>1</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='32B441FD'>m</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='4854558C'>Een pand met meerdere verblijfsobjecten. Dit is een veel voorkomende situatie bij bijvoorbeeld ﬂatgebouwen met portiekwoningen of galerijwoningen.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='74A36D01'>n</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='3C99B8F9'>1</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7059FACD'>Een verblijfsobject dat zich uitstrekt over meerdere panden. Dit is een situatie die soms voorkomt bij bijvoorbeeld doorbraken van winkels tussen enkele panden.</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1F6519A2'>n</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0495128E'>m</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='65F575A0'>Meerdere verblijfsobjecten die zich uitstrekken over meerdere panden.</p></td>
</tr>
</tbody>
</table>

<p id='0002C18E'>Uit deze relaties volgt ook de logische volgordelijkheid van het opvoeren van BAG-objecten in de registratie van een bronhouder:</p>
<ul><li>eerst Woonplaats en/of Openbare ruimte, daarna tegelijk Nummeraanduiding van het hoofdadres met Verblijfsobject of Standplaats of Ligplaats;</li>
<li>eerst Pand, daarna Verblijfsobject;</li>
<li>eerst Nummeraanduiding van het hoofdadres, daarna Nummeraanduidingen van eventuele nevenadressen.</li>
</ul>

<p id='7231C9D4'>De logische volgordelijkheid voor het afvoeren van BAG-objecten is andersom.</p>
<p id='71B78776'>De nummeraanduidingen van eventuele nevenadressen ontstaan tegelijk met het hoofdadres of later en mogen worden afgevoerd terwijl het Verblijfsobject, de Standplaats of de Ligplaats blijft bestaan.</p>

<p id='42F88DFB'>Voor de relatie tussen Pand en Verblijfsobject geldt dat de administratieve relatie leidend is boven de ruimtelijke relatie (zie §<a href='#48C73D30'>3.5</a>).</p>
<p id='7C9685FC'>Voor de verwijzing naar een Woonplaats geldt dat de ruimtelijke relatie leidend is boven de administratieve relatie.</p>

## Topologie {#48C73D30}
<p id='68D9C989'>Topologie beschrijft de onderlinge ruimtelijke relaties tussen de objecten, onafhankelijk van hun werkelijke positie (coördinaten). Een voorbeeld is dat een object gepositioneerd is in een ander object: 'ligt in' is dan de topologische relatie.</p>

<p id='14D97D80'>De BAG kent de volgende topologische relaties:</p>
<ul><li>Pand en verblijfsobject: <ul><li>Verblijfsobjecten maken altijd deel uit van een pand (of van meerdere panden). Een verblijfsobject moet daarom volledig binnen een of meer panden worden gepositioneerd waarbinnen het zich bevindt. Als een verblijfsobject een puntgeometrie heeft, mag deze punt binnen het pand op een willekeurige plek staan.</li>
</ul>
</li>
</ul>

<ul><li>Woonplaats en openbare ruimte: <ul><li>Openbare ruimten moeten altijd volledig zijn gelegen binnen één woonplaats. Als een openbare ruimte door het splitsen van een woonplaats in meerdere woonplaatsen komt te liggen, wordt de openbare ruimte in elk van deze woonplaatsen afgebakend. </li>
</ul>
</li>
</ul>

<ul><li>Woonplaats: <ul><li>Het gehele grondgebied van de gemeente dient te zijn ingedeeld in woonplaatsen. De geometrieën van de woonplaatsen dienen naadloos op elkaar aan te sluiten en mogen elkaar niet overlappen, oftewel de geometrische vereniging van iedere woonplaats binnen een gemeente komt overeen met de geometrische contour van het grondgebied van deze gemeente.</li>
</ul>
</li>
</ul>

## Levenscyclus {#3688B20B}
<p id='3228F084'>De levenscyclus van een BAG-object beschrijft de opeenvolgende fasen in de ontwikkeling van een object. Hierbij dient de werkelijkheid zoveel mogelijk in de registratie zichtbaar te zijn. In de verschillende fasen zijn er situaties die aanleiding geven tot het wijzigen van de gegevens van het object. De fase van ontwikkeling waarin een BAG-object zich bevindt, wordt met een eigenschap status bij het object geregistreerd.</p>

<p id='58D1AB26'>In de levenscyclus van een pand en verblijfsobject wordt in hoofdlijnen een onderscheid gemaakt tussen de vier fasen planvorming, bouw, gebruik en sloop. Binnen deze fasen kunnen verschillende statussen aan het object worden toegekend. De levenscyclus van een pand of een verblijfsobject volgt meestal een logische volgorde van statussen (zie <a href='#d6aChBdBb'>Figuur 2</a>), maar fasen in de levenscyclus mogen ook worden overgeslagen.</p>
<figure id='d6aChBdBb'><img src='media/image3.jpg' alt='Afbeelding 2' style='width: 100%;'></img>
<figcaption>De logische volgordelijkheid van de ontwikkeling en status van panden en verblijfsobjecten. Het plaatje geeft de meest logische route aan. </figcaption></figure>

<p id='3EF715DD'>In de levenscycli van standplaatsen, ligplaatsen, openbare ruimten, nummeraanduidingen en woonplaatsen wordt onderscheid gemaakt tussen het benoemen en het intrekken van deze objecten.</p>
<p id='03591C2B'>Binnen een fase van de levenscyclus kunnen attributen worden gewijzigd, zoals het gebruiksdoel bij een verblijfsobject of de geometrie van een pand.</p>

<p id='208F015F'>Verder gelden de volgende regels voor het toewijzen van een status aan een object:</p>
<ol type='1'><li>Indien voor een pand met de status Bouwvergunning verleend of Bouw gestart een nieuwe vergunning of andere publiekrechtelijke toestemming wordt verleend, worden wel de gegevens van het pand gewijzigd conform de vergunning of andere publiekrechtelijke toestemming, maar de status van het pand blijft ongewijzigd.</li>
<li>Indien:<ul><li>een pand de status Pand in gebruik (niet ingemeten) of Pand in gebruik heeft bereikt, kan de status van het pand niet meer terug naar Bouwvergunning verleend of Bouw gestart, tenzij sprake is van een ten onrechte toegekende status.</li>
<li>een verblijfsobject de status Verblijfobject in gebruik (niet ingemeten) of Verblijfsobject in gebruik heeft bereikt, kan de status van het verblijfsobject niet meer terug naar Verblijfsobject gevormd, tenzij sprake is van een ten onrechte toegekende status.</li>
</ul>
</li>
<li>Elke statusovergang is toegestaan, mits deze een correctie betreft van een ten onrechte toegekende status.</li>
<li>Als een vergunning of andere publiekrechtelijke toestemming wordt verleend voor de verbouwing van een pand en/of verblijfsobjecten, krijgen het pand en/of verblijfsobjecten die als gevolg van deze verbouwing als zodanig zullen blijven bestaan, maar waarvan een of meer gegevens in de BAG zullen wijzigen, de status Verbouwing pand of Verbouwing verblijfsobject. Als de verbouwing is afgerond, krijgt het pand de status Pand in gebruik (niet ingemeten) of Pand in gebruik, en de verblijfsobjecten de status Verblijfsobject in gebruik (niet ingemeten) of Verblijfsobject in gebruik.</li>
<li>Als een vergunning of andere publiekrechtelijke toestemming wordt verleend voor het splitsen van een verblijfsobject of het samenvoegen van meerdere verblijfsobjecten, worden de nieuw te realiseren verblijfsobjecten opgenomen met de status Verblijfsobject gevormd. De 'oude' verblijfsobjecten behouden hun status tijdens de verbouwing (meestal Verblijfsobject in gebruik). Als de verbouwing is afgerond, worden de ‘oude’ verblijfsobjecten ingetrokken, terwijl de nieuwe verblijfsobjecten de status Verblijfsobject in gebruik (niet ingemeten) of Verblijfsobject in gebruik krijgen, zodra zij gebruiksgereed zijn.</li>
<li>Als een vergunning of andere publiekrechtelijke toestemming wordt verleend voor het toevoegen van verblijfsobjecten aan bestaande panden of een verbouwing waarbij het aantal verblijfsobjecten verandert, worden nieuwe Verblijfsobjecten opgenomen met de status Verblijfsobject gevormd. </li>
<li>Bij een verbouwing op een pand krijgen de eventueel aanwezige Verblijfsobjecten de status Verbouwing verblijfsobject, ongeacht of de pandcontouren wijzigen. Als de pandcontouren wijzigen, krijgt het Pand de status Verbouwing pand .</li>
<li>Indien er meerdere verbouwingen aan een pand worden verricht, krijgt het pand na voltooiing van de laatste verbouwing de status Pand in gebruik (niet ingemeten) of Pand in gebruik.</li>
<li>Indien de geometrie van een pand of verblijfsobject is ingemeten voordat de bouw is afgerond en er geen nieuwe geometrie hoeft te worden ingemeten, krijgt het pand of verblijfsobject meteen de status Pand in gebruik of Verblijfsobject in gebruik zodra het gereed is voor gebruik na afronding van de bouw.</li>
<li>Indien een verblijfsobject de status Verblijfsobject in gebruik (niet ingemeten) heeft gekregen, krijgen ook de een of meer panden waarin het verblijfsobject is gelegen, de status Pand in gebruik (niet ingemeten).</li>
<li>Indien in een vergund pand met meerdere verblijfsobjecten een of meerdere verblijfsobjecten de status Verblijfsobject in gebruik (niet ingemeten) of Verblijfsobject in gebruik krijgen, dan krijgt het pand meteen de status Pand in gebruik (niet ingemeten), respectievelijk Pand in gebruik.</li>
<li>De status Sloopvergunning verleend is zowel van toepassing op situaties waarin specifiek voor het betreﬀende pand een vergunning of andere publiekrechtelijke toestemming tot sloop is verleend, als op situaties waarin op grond van andere regelgeving geen vergunning of andere publiekrechtelijke toestemming tot sloop nodig is (omdat deze andere regelgeving daarmee in wezen al vergunning of andere publiekrechtelijke toestemming heeft verleend).</li>
<li>Indien een object de status niet gerealiseerd, ten onrechte opgevoerd, gesloopt of ingetrokken heeft, is het feitelijk beëindigd en kan de status niet meer worden gewijzigd. Alleen objecten die ten onrechte een van deze statussen hebben gekregen, kunnen middels een schriftelijke verklaring herleven.</li>
<li>Bij elke mutatie wordt de actuele status toegekend. Muteren in het verleden is niet toegestaan.</li>
</ol>

## Identificatie en historie {#4FF275BF}
<p id='591A976B'>Deze paragraaf beschrijft algemene principes die gelden voor de inhoud van de BAG en die betrekking hebben op identificatie (zie §<a href='#0CD0FCE7'>3.7.1</a>) en op historie (zie §<a href='#3C38C72E'>3.7.2</a>).</p>

### Identificatie {#0CD0FCE7}
<p id='7F0F51DE'>Aan elk object wordt een uniek objectnummer (identificatie) toegekend. Zolang het object bestaat, mag deze identificatie niet veranderen.</p>

<p id='66E87D5C'>Bij splitsing van een woonplaats of openbare ruimte wordt alleen een daardoor nieuw ontstane (oftewel niet reeds aanwezige) woonplaats of openbare ruimte van een nieuwe identificatiecode voorzien. Dat aan een nieuw ontstaan object een identificatiecode<span class='noot'>[10]<span class='noottekst'>Wet basisregistratie adressen en gebouwen, artikel 19, eerste lid: "In de basisregistratie worden een identificerend objectnummer, beschrijvende gegevens, temporele gegevens en meta-gegevens opgenomen over de in de gemeente bestaande: a. panden; b. verblijfsobjecten; c. standplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 1°; d. ligplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 2°; e. woonplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 3°; f. openbare ruimten, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 4°, en g. nummeraanduidingen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 5°." https://zoek.officielebekendmakingen.nl/stb-2017-60.html<br/>
</span></span> <span class='noot'>[11]<span class='noottekst'>Wet van 10 februari 2017 tot wijziging van de Wet basisregistratie adressen en gebouwen en enige andere wetten in verband met modernisering en vereenvoudiging van de registratie en het toezicht, artikel I, onderdeel Q, onder 19, eerste lid: "In de basisregistratie worden een identificerend objectnummer, beschrijvende gegevens, temporele gegevens en meta-gegevens opgenomen over de in de gemeente bestaande: a. panden; b. verblijfsobjecten; c. standplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 1°; d. ligplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 2°; e. woonplaatsen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 3°; f. openbare ruimten, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 4°, en g. nummeraanduidingen, alsmede situaties als bedoeld in artikel 2, tweede lid, onderdeel b, aanhef en onder 5°." https://zoek.officielebekendmaking en.nl/stb-2017-60.html<br/>
</span></span> wordt toegekend, volgt uit artikel 19, eerste lid, van de wet en het gewijzigde artikel 10<span class='noot'>[12]<span class='noottekst'>Besluit van 6 juli 2017 tot wijziging van het Besluit basisregistratie adressen en gebouwen in verband met modernisering en vereenvoudiging van de registratie, artikel I, onderdeel G: "Artikel 10 wordt als volgt gewijzigd: 1. In het eerste lid wordt “in de artikelen 19, eerste lid, onderdeel a, 20, eerste lid, onderdeel a, 21, eerste lid, onderdeel a, 22, eerste lid, onderdeel a, 23, eerste lid, onderdeel a, 24, eerste lid, onderdeel a, en 25, eerste lid, onderdeel a, van de wet” vervangen door: bij de nummers 1.1, 2.1, 3.1, 4.1, 5.1, 6.1 en 7.1 in de bijlage bij dit besluit. 2. Het tweede en derde lid komen te luiden: 2. Indien een in de basisregistratie opgenomen verblijfsobject, standplaats of ligplaats wordt gesplitst, wordt elk van de aldus ontstane verblijfsobjecten, standplaatsen of ligplaatsen van een nieuwe identificatiecode voorzien. 3. Indien in de basisregistratie opgenomen verblijfsobjecten, standplaatsen of ligplaatsen worden samengevoegd, wordt het aldus ontstane verblijfsobject, dan wel de aldus ontstane standplaats of ligplaats van een nieuwe identificatiecode voorzien." https://zoek.officielebekendmakingen.nl/stb-2017-311.html<br/>
</span></span> <span class='noot'>[13]<span class='noottekst'>Nota van toelichting bij het Besluit van 6 juli 2017 tot wijziging van het Besluit basisregistratie adressen en gebouwen in verband met modernisering en vereenvoudiging van de registratie, algemeen deel, artikel 2.3: "Identificatiecodes bij splitsing en samenvoeging van woonplaatsen en openbare ruimten. Bij de evaluatie van de wet is de wens geuit om bij wijzigingen van woonplaatsen alleen de geometrie te wijzigen. De regels voor wijzigingen van woonplaatsen die in het tweede en derde lid van artikel 10 van het besluit waren opgenomen, brachten onder meer mee dat in veel gevallen mutaties in de registratie moesten worden doorgevoerd die voor gebruikers de indruk wekten dat verhuizingen naar andere woonplaatsen hadden plaatsgevonden, terwijl het uitsluitend ‘administratieve verhuizingen’ betrof. Bij wijziging van openbare ruimten deed zich hetzelfde voor. Het BAG Bronhouders- en Afnemers Overleg (BAG BAO) heeft nader onderzoek laten doen naar het behoud van de identificatiecode bij geometriewijzigingen. Op basis van de resultaten is door het BAG BAO geadviseerd artikel 10 van het besluit aan te passen. Het advies houdt in dat de identificatiecode van de woonplaats alleen wordt gewijzigd in het geval van splitsing van een woonplaats, voor zover de opgesplitste delen geen deel gaan uitmaken van een andere bestaande woonplaats. Bij samenvoeging van (een deel van) een woonplaats met een andere woonplaats wordt ofwel een van de woonplaatsen opgeheven (als deze geheel met een andere woonplaats wordt samengevoegd), ofwel wijzigt alleen de geometrie van beide woonplaatsen. Op die manier leidt de wijziging van de geometrie van een bestaande woonplaats niet tot wijziging van de identificatiecode van die woonplaats. Het BAG BAO heeft hierbij tevens geadviseerd om, gezien de overeenkomsten in de aard van de problematiek, dezelfde aanpak te volgen bij wijzigingen van openbare ruimten. Gelet op het uitgebrachte advies zijn het tweede en derde lid van artikel 10 heroverwogen. Geconcludeerd is dat opvolging van het advies aanbeveling verdient. Een en ander heeft geleid tot een formulering van artikel 10 die inhoudt dat bij splitsing van een woonplaats of openbare ruimte alleen een daardoor nieuw ontstane (oftewel niet reeds aanwezige) woonplaats of openbare ruimte van een nieuwe identificatiecode wordt voorzien. Dat aan een nieuw ontstaan object een identificatiecode wordt toegekend, volgt uit artikel 19, eerste lid, van de wet en het nieuwe artikel 8 van het besluit in samenhang met de bij het besluit behorende bijlage. Een bij splitsing betrokken reeds bestaande woonplaats of openbare ruimte wordt niet geacht op te houden te bestaan, maar ondergaat alleen een wijziging van de geometrie. Bij samenvoeging van twee woonplaatsen of openbare ruimten houdt de ene daarbij betrokken woonplaats of openbare ruimte op te bestaan, en wijzigt de geometrie van de andere woonplaats of openbare ruimte. Bij dat laatste bekijkt de gemeente per geval welk betrokken object logischerwijs geacht wordt voort te bestaan en welk object verdwijnt." https://zoek.officielebekendmakin gen.nl/stb-2017-311.html<br/>
</span></span> van het besluit. Een bij splitsing betrokken reeds bestaande woonplaats of openbare ruimte wordt niet geacht op te houden te bestaan, maar ondergaat alleen een wijziging van de geometrie. Bij samenvoeging van twee woonplaatsen of openbare ruimten houdt de ene daarbij betrokken woonplaats of openbare ruimte op te bestaan en wijzigt de geometrie van de andere woonplaats of openbare ruimte. Bij dat laatste bekijkt de gemeente per geval welk betrokken object logischerwijs geacht wordt voort te bestaan en welk object verdwijnt.</p>

<p id='3DACCAB7'>De identificatie moet het object per bronhouder uniek identificeren. Hiervoor dient gebruik te worden gemaakt van een viercijferige objectnummering voor het objecttype Woonplaats en een zestiencijferige objectnummering voor de overige BAG-objecten.</p>

<p id='6C62C629'>Het viercijferige objectnummer van een woonplaats is de code die de beheerder van de landelijke voorziening toekent aan een nieuwe woonplaats. Dit gebeurt binnen twee<span class='noot'>[14]<span class='noottekst'>De beheerder van de landelijke voorziening geeft de woonplaatscodes uit op grond van artikel 19 lid 3 van de Wet basisregistratie adressen en gebouwen en artikel 11 van het Besluit basisregistratie adressen en gebouwen. http://wetten.overheid.nl/jci1.3:c:BWBR0023466  en http://wetten.overheid.nl/jci1.3:c:BWBR0 025520#Hoofdstuk3_Artikel11 en http://www.kadaster.nl/web/Themas/Registraties/BAG/BAGartikelen/BAG-Woonplaatscodes.htm<br/>
</span></span> werkdagen nadat de gemeente erom heeft verzocht.</p>

<p id='11A12EE6'>Het eerste deel van het zestiencijferige objectnummer bestaat uit vier numerieke posities met de gemeentecode, zoals gepubliceerd in Tabel 33 Gemeententabel van de Rijksdienst voor Identiteitsgegevens<span class='noot'>[15]<span class='noottekst'>Tabel 33 Gemeententabel maakt deel uit van de Landelijke Tabellen BRP. "Landelijke Tabellen zijn coderingslijsten waarin gegevens zijn opgenomen die gebruikt worden voor de bijhouding van persoonsgegevens in het geautomatiseerde systeem van de Basisregistratie Personen (BRP). Hoewel deze tabellen een onderdeel zijn van het Logisch Ontwerp BRP en op grond daarvan dezelfde juridische waarde bezitten, nemen ze een bijzondere plaats in. Dat komt voornamelijk omdat tabellen aan voortdurende wijziging onderhevig kunnen zijn. [...] De bijhouding en verspreiding van de Landelijke Tabellen wordt uitgevoerd door de Rijksdienst voor Identiteitsgegevens (RvIG)." http://publicaties.rvig.nl/Landelijke_tabellen/Inleiding_op_de_Landelijke_Tabellen_BRP<br/>
</span></span>. De gemeentecode wordt toegekend aan de identificatie op basis van de gemeente waar het object ontstaat. Het tweede deel van het zestiencijferige objectnummer bestaat uit twee numerieke posities met de code voor het betreﬀende objecttype (zie <a href='#d6aCiCbK'>Tabel 4</a>).</p>
<table id='d6aCiCbK' style='width: 100%;'><caption><span class='tblno'>Tabel 4</span>   De objecttypecodes van de BAG</caption>
<colgroup><col id='col1-d6aCiCbK' style='width: 50%;'>
<col id='col2-d6aCiCbK' style='width: 50%;'>
</colgroup>
<thead><tr><th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='13CF8720'>Objecttypecode</p></th>
<th class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1B7F8888'>BAG-object</p></th>
</tr>
</thead>
<tbody><tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='158C7D96'>01</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='49BAA9D9'>Verblijfsobject</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='03226A0B'>10</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='5A4AE18A'>Pand</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='7F31CC05'>02</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='346CE5AF'>Ligplaats</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='2FF359B2'>20</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='25C4D9DB'>Nummeraanduiding</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='23A50891'>03</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='0D4668AA'>Standplaats</p></td>
</tr>
<tr><td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='1FB2277E'>30</p></td>
<td class='left' style='border-top: 0.5pt solid #000000; border-left: 0.5pt solid #000000; border-bottom: 0.5pt solid #000000; border-right: 0.5pt solid #000000;'><p id='10A1C473'>Openbare ruimte</p></td>
</tr>
</tbody>
</table>

<p id='73CE7299'>Het derde deel van het zestiencijferige objectnummer bestaat uit tien numerieke posities met een binnen een gemeente uniek objectvolgnummer. Indien een objectvolgnummer uit minder dan tien posities bestaat dan dient deze ten behoeve van de uitwisseling te worden aangevuld met voorloopnullen.</p>

<p id='2C8E68D5'>Op deze wijze ziet de identificatie van een Pand (objecttypecode 10) dat is ontstaan in de gemeente Amersfoort (gemeentecode 0307) en toen objectvolgnummer 367968 heeft gekregen, eruit als: 0307100000367968.</p>

<p id='5404A517'>De identificatie van een BAG-object wordt bepaald bij het ontstaan van het object en blijft behouden als het object wordt overgedragen aan een andere bronhouder, zoals bij een gemeentelijke herindeling. De gemeentecode in de identificatie kan daarom niet worden gebruikt om te bepalen binnen welke gemeente een object is gelegen.</p>

### Historie {#3C38C72E}
<p id='5EEAB57C'>Deze paragraaf beschrijft hoe de BAG invulling geeft aan historie.</p>

<p id='1A8040C7'>In de BAG worden gegevens bijgehouden van alle objecten in de BAG. Al deze gegevens worden bestendig bewaard in de registratie van bronhouders en de landelijke voorziening. Als er nieuwe gegevens worden geregistreerd, dan blijven de oude gegevens bewaard. Dit heet het bijhouden van gegevens onder historie. Het uiteindelijke doel van het bijhouden van historie is om vragen te kunnen beantwoorden zoals "welke gegevens zijn er nu geldig?", "sinds wanneer had men dit kunnen weten?" en andere vragen.</p>

<p id='66917F84'>Elk object heeft kenmerken, zoals een naam, een geometrie, een status of een relatie met een ander object. Hiervan worden de gegevens bijgehouden. In de BAG is het nodig om van alle gegevens te weten wanneer ze geldig zijn of geldig zijn geworden. In de tijd kunnen deze gegevens een andere waarde krijgen. De nieuwe gegevens worden dan geregistreerd en geldig, de oude zijn dan niet meer geldig. De BAG hanteert hiervoor materiële historie.</p>
<p id='1E2EE0EE'>Ook is het nodig om te weten wanneer de gegevens formeel in werking zijn getreden, omdat een besluit rondom de materiële geldigheid eerder of later verwerkt kan zijn. Er zit dan een grotere periode tussen wanneer een gegeven geldig is en wanneer dit is geregistreerd. De BAG hanteert hiervoor het concept formele historie. De BAG streeft ernaar om de materiële en formele historie dichtbij elkaar te houden, maar dit is niet altijd mogelijk.</p>
<p id='5E97F1DC'>Deze twee soorten historie dekken de juridische geldigheid van de BAG-gegevens af.</p>

<p id='702CD0DD'>In het conceptuele informatiemodel (zie hoofdstuk 5 Conceptueel model) zijn alle kenmerken van het object opgenomen. Op deze gegevens is het bijhouden van historie (meestal) van toepassing. Per gegeven wordt daarom via een metagegeven aangegeven of het bijhouden van historie aan de orde is. Deze metagegevens specificeren we als volgt:</p>
<ul><li>Indicatie materiële historie: indicatie of de materiële historie van de attribuutsoort te bevragen is. Materiële historie geeft aan wanneer een verandering is opgetreden in de werkelijkheid die heeft geleid tot verandering van de attribuutwaarde. Materiële historie impliceert dat actuele, historische en eventuele toekomstige attribuutwaarden te bevragen zijn.</li>
<li>Indicatie formele historie: indicatie of de formele historie van de attribuutsoort te bevragen is. Formele historie geeft aan wanneer in de administratie een verandering is verwerkt van de attribuutwaarde (wanneer was de verandering bekend en is deze verwerkt).</li>
</ul>

<p id='773FCA05'>Aanvullend is het van belang wanneer gegevens vanuit de bronhouders succesvol zijn verwerkt in de landelijke voorziening, waarmee deze gegevens (binnen bepaalde termijn) beschikbaar zijn geworden voor afnemers van de landelijke voorziening. Hiervoor houdt de landelijke voorziening aanvullende datums bij.</p>
<p id='490CDC9D'>De implementatie van historie is beschreven in hoofdstuk 9.</p>

## Gebruiksdoel {#1E54126F}
<p id='60FAB46A'>Bij een verblijfsobject worden een of meer gebruiksdoelen opgenomen. Onder het gebruiksdoel van een verblijfsobject wordt verstaan een overzicht van de (gecategoriseerde) gebruiksdoelen die bij het verlenen van een vergunning of andere publiekrechtelijke toestemming aan het betreﬀende verblijfsobject zijn toegekend. Deze gebruiksdoelen worden ook wel aangeduid als de bouwkundige bestemming conform de categorisering van het Bouwbesluit 2012<span class='noot'>[16]<span class='noottekst'>Bouwbesluit 2012, artikel 1.1, tweede lid: "Voor de toepassing van de bij of krachtens dit besluit gegeven voorschriften wordt voorts verstaan onder: bijeenkomstfunctie: gebruiksfunctie voor het samenkomen van personen voor kunst, cultuur, godsdienst, communicatie, kinderopvang, het verstrekken van consumpties voor het gebruik ter plaatse of het aanschouwen van sport; bouwwerk geen gebouw zijnde: bouwwerk of gedeelte daarvan, voor zover dat geen gebouw of onderdeel daarvan is; celfunctie: gebruiksfunctie voor dwangverblijf van personen; gezondheidszorgfunctie: gebruiksfunctie voor medisch onderzoek, verpleging, verzorging of behandeling; industriefunctie: gebruiksfunctie voor het bedrijfsmatig bewerken of opslaan van materialen en goederen, of voor agrarische doeleinden; kantoorfunctie: gebruiksfunctie voor administratie; logiesfunctie: gebruiksfunctie voor het bieden van recreatief verblijf of tijdelijk onderdak aan personen; onderwijsfunctie: gebruiksfunctie voor het geven van onderwijs; overige gebruiksfunctie: niet in dit lid benoemde gebruiksfunctie voor activiteiten waarbij het verblijven van personen een ondergeschikte rol speelt; sportfunctie: gebruiksfunctie voor het beoefenen van sport; winkelfunctie: gebruiksfunctie voor het verhandelen van materialen, goederen of diensten; woonfunctie: gebruiksfunctie voor het wonen." http://wetten.overheid.nl/jci1.3:c:BWBR0030461<br/>
</span></span>.</p>

<p id='54CF6B12'>Bij een geconstateerd verblijfsobject wordt het feitelijke gebruik als gebruiksdoel (of de gebruiksdoelen) opgenomen op grond van een document van constatering.</p>

<p id='3483FF71'>Voor het wijzigen van het gebruiksdoel van verblijfsobjecten gelden de volgende uitgangspunten:</p>

<ul><li>Een vergunde gebruikswijziging wordt geregistreerd in de BAG op basis van een vergunning of andere publiekrechtelijke toestemming;</li>
<li>Een bestemmingsplan- / omgevingsplanwijziging wordt niet geregistreerd in de BAG;</li>
<li>Een vergunningvrije gerealiseerde gebruikswijziging, voor zover die past binnen de regels van het bestemmingsplan / omgevingsplan, kan (lees: niet verplicht) worden geregistreerd in de BAG op basis van een ambtelijke verklaring (bijv. een bevindingenbrief van de afdeling Vergunningverlening);</li>
<li>Een niet-vergunde gebruikswijziging, die niet past binnen de regels van het bestemmingsplan / omgevingsplan, wordt niet geregistreerd in de BAG.</li>
</ul>
