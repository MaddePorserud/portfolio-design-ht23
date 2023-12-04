---
Title: Load
Description: Analysis of load
Date: December 3, 2023
Template: analys
---

Min analys kring load.
=======================

I denna rapport finns en analys kring hur snabbt olika nyhetssidor laddar.

Urval
-----------------------

För analysen av hur snabbt olika sidor laddar har jag valt ut tre stora svenska nyhetssidor. Anledningen till att jag valde dessa sidor är att jag själv ofta upplever att jag behöver vänta en stund innan sidan visas. Därför tyckte jag att det var intressant att analysera just dessa sidor. Sidorna som valts är webbsidan för Sveriges Radio, Dagens Nyheter samt Aftonbladet. 

Metod
-----------------------

Analysen genomfördes genom att först med verktyget Pagespeed Insight då ett betyg för webbsidan anpassad för dator samt mobil-enhet. Därefter öppnades respektive sida i Google Chrome och varje sida uppdaterades tre gånger med shift+control+r och under fliken "Nätverk" i utvecklarverktyget noterades laddnindstiderna samt hur många bilder som laddades in. I rapporten presenteras ett medelvärde för laddningstiderna. För varje sida testades två undersidor utöver startsidan. Detaljerade resultat finns i flikarna i tabellen nedan.

Resultat
-----------------------

<div class="screendump">
<img src="%assets_url%/img/dn.png" alt="dn.se">
<img src="%assets_url%/img/sr.png" alt="sr.se">
<img src="%assets_url%/img/aftonbladet.png" alt="aftonbladet.se">

</div>


###Test av de tre utvalda sidorna

<div class="embed-container">
<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQS1fUH_HyAUfCdHNuGhK126KRASFJrgpGkVx2Nrbqzn5J3ljaJZZJN0YExbxDewpi4afnIgiE9pmgy/pubhtml?widget=true&amp;headers=false"></iframe>



Analys
-----------------------

Min upplevelse är att alla dessa sidor laddar långsamt. Jag tycker att en snabb webbplats bör ha en laddningstid på under 1 sekund. Alla sidor verkar ha väldigt stora DOM-träd. Troligen kan laddningen göras snabbare om DOM-trädet skulle göras mindre. DN och Sveriges radio verkar dessutom ha flera bilder som laddas i störra storlek än vad som behövs - så deras utvecklare kanske skulle vara hjäpta av at delta på det gär kursmomentet.

Kanske att man skulle kunna få en känsla av att sidan är snabbare om man väntade med att ladda in det som är "below-the-fold" på sidan.

DN och Aftonbladet som båda finaniseras av reklamintäkter verkar ha någon form av annonseringsverktyg på sidan som hindrar innehåll från att laddas direkt. Blir delvis orättvist att jämföra det med Sveriges radio som inte är beroende av reklam men för mig som slutkonsument så blir uppfattningen att sidorna med reklam är långsammare. 

Bäst i detta test är Sveriges radio då sidan är snabbast att ladda. På andra plats kommer DN som är den minsta sidan, det långsamma på sidan verkar främst bero på att någon form av reklamverktyg blockerar direkt laddning av allt innehåll. På sista plats hamnar Aftonbladet vars sida är långsammast och dessutom störst. 


Referenser
-----------------------


Övrigt
-----------------------
Analysen är utförd av mapu23 hösten 2023.