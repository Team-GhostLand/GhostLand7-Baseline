# **Patch 4** *Autor: Guzio*
* Updated: AmbientSounds, CraftPresence i UniLib. Dodania/usunięcia/updatey modów z Modrintha nie są śledzone w plikach patchy, więc nie wystarczy zaaplikować `patch4.zip` - musisz sam je updateować, lub reinstalować paczkę do najnowszej wersji, która te zmiany posiada.
* Usunięto OmniCore i Moonlight Lib (bez żadnych configów, bo te mody ich nie mają), bo któryś z nich psuł komendy na kliencie, a drugi okazał się nie mieć żadnych dependencji (mimo bycia zapisanym jako biblioteka). Nie wiem który to który, ale to nie ważne, bo po wyłączeniu ich obydwu razem, okazało się, że żaden z nich nie jest nam potrzebny (again - nie miały dependencji, a są bibliotekami). Przypadkowe naprawienie ostatniego road-blocking bug Baselinea to po prostu (**bardzo** mile widziany) side-effect. Dodania/usunięcia/updatey modów z Modrintha nie są śledzone w plikach patchy, więc nie wystarczy zaaplikować `patch4.zip` - musisz sam je usunąć, lub reinstalować paczkę do najnowszej wersji, która te zmiany posiada. Anyway, skoro ten ostatni road-blocking bug jest naprawiony, to można powiedzieć, że baseline osiągnął status stabilny - można oficjalnie przejść do fazy „slimming this bitch down”. Prace nad GhostLand 7 już niedługo, czuję to w kościach! Hell, część z nich można rozpocząć już teraz, np. pewne akcje demokratyczne (*wink-wink, nugde-nudge, Tymuś, rusz dupę z ankietą do cholery jasnej*) lub ustawienie *niektórych* configów tutaj.
* Usunięto Frozen Lib, Textile i Lithostitched, bo okazały się być niepotrzebne (są bibliotekami, a nie mają dependencji). Usunięto też config `frozenlib.json5`, a Lithostitched i Textile nie miały configów. Dodania/usunięcia/updatey modów z Modrintha oraz usunięcia configów nie są śledzone w plikach patchy, więc nie wystarczy zaaplikować `patch4.zip` - musisz sam je usunąć, lub reinstalować paczkę do najnowszej wersji, która te zmiany posiada.
* Dodano Bind Pizzeria. Configi na razie nie były zmieniane, więc są defaultowe. Dodania/usunięcia/updatey modów z Modrintha oraz powstanie defaultowych configów nie jest śledzone w plikach patchy, więc nie wystarczy zaaplikować `patch4.zip` - musisz sam dodać moda (i w konsekwencji wygenerować jego defaultowe configi), lub reinstalować paczkę do najnowszej wersji, która te zmiany już posiada.

## Zmiany poza patchem:
* Skorygowano fucked-up kopiowanie w `patch3.md`.
* Znaleziono mody, które wymagają YACL.
* Fixed an accidential „œ” in `README.md`.
* Re-ordered some sections of `README.md`.
* Nareszcie, ilość modów podawana przez MR i z sumy w `README.md` się zgadza! YIPPPEEEEEEEEEEEEE! (Okazało się, że problem powodował podwójnie-liczony OmniCore.)
* Oficjlanie osiągnięto próg „wywalenie wszystkich QOLek = dobicie do setki modów”, co spowodowało zmiany w tamtej sekcji `README.md`.
* Skorygowano nazwę jednego z configów w `CONTRIBUTING.md`.
* Incremented N and version in `CONTRIBUTING.md` for future contibutors.

## Btw...
* Nie dodano pliku `patch4.zip` (mimo wielokrotnego wspominiania go w patchnotesach), gdyż byłby on kompletnie pusty (przecież po to był wspominany, żeby powiedzieć, że zmiany wprowadzone w tym patchu nie są reprezentowane w plikach ZIP).
* To, że udało mi się znaleźć kilka useless dependencies nie znaczy, że opracja „Wywalamy niepotrzebne biblioteki” została ukończona. Te 5 tutaj (+dzieci YACL) udało mi się znaleźć przez przypadek.