# GL baseline
A list of „modded MC essentials” that for whatever reason must be inside GhostLand 7 (and preferably future GL editions). Note: the rest of this doc (apart from the very last section) is in Polish.

O ile nie podano inaczej, `[tagi]` oznaczają, że mod należy do kategorii z której się wziął, ale posiada też aspekty pasujące do tej z taga (np. Mod w QoL z `[Ambience]` jest QoL, ale ma w sobie elementy Ambience-moda).

## Dependencje (13 udało mi się „złapać”; 15 musiało dojść „gdzieś po drodze”; pewnie można część usunąć (była Wielka Czystka, after all - część dependencji na pewno straciła swoje „dzieci”), ale to lepiej robić jak przeczyścimy wszystko inne):
* Fabric API (prawie wszystko)
* Cloth Config API (prawie wszystko)
* YACL (Zoomify, Adaptive Tooltips)
* Fabric Language Kotlin (dość sporo)
* Indium (Pozwala używać z Sodium wieloma modami)
* Sodium Options API (niektóre mody dodające rzeczy do ustawień Sodium, które z jakiegokolwiek powodu nie robią tego przez wbudowane API Sodium) - *W połączeniu z Reese's Options: Dodaje ikonki pokazujące, który mod dodał co do ustawień Sodium. Dział dla wszystkich modów; nie tylko do tych rejestrujących przez to.*
* CreativeCore (AmbientSounds)
* Konkrete (FancyMenu, Drippy Loading Screen)
* Melody (FancyMenu)
* Architectury API (dość sporo)
* Balm (wszelkie mody Blaya, np. zainstalowany Nether Portal Fix; w przyszłości mogą się jeszcze pojawić Waystoney, a może nawet i KleeSlaby i/lub Cooking for Blockheads)
* libIPN (IPN *(duh)*)
* Searchables (Controlling)
* *Niezidentyfikowane (auto-dodały się gdzieś w miedzyczasie i nie zauważyłem kiedy): Almanac, Athena, Bookshelf, Cardinal Components API, CICADA, Cobweb, Forge Config API Port, Iceberg, Puzzles Lib, Resourceful Lib, Silk, SuperMartijn642's Config Lib, SuperMartijn642's Core Lib, TCDCommons API, UniLib*

## Z Simply Optimised (15  *+3 libs*):
Baza naszego modpacka. Dość niekonwenjconalnie - zazwycaj Fabricowe GhostLandy bazowały na Fabulously Optimised, nie Simply Optimised. Wydaje mi się jednak, że mam bardzo dobre uzasadnienie takiej decyzji, ale przedstawię je dopiero przy FO. Na razie jesteśmy przy SO - aprops którego: SO to modpack CZYSTO pod optymalizację. Nie ma nic, poza modami na performance (nie licząc NCR). Co za tym idzie, nie daję tagów. Po prostu pamiętaj, że każdy z tych modów należy również do kategorii Optymalizacja (poza NCR - ale on został correctly oznaczony). Also - ponieważ te mody są czysto pod optymalizację, to pozwolę sobie nie dawać uzasadnień, czemu są dodane, bo przyznam, że sam nie mam do końca pewności co niektóre z nich robią. Trust the process, że tak powiem.
* BadOptimizations
* C2ME
* Enhanced Block Entities
* Entity Culling
* FerriteCore
* ImmediatelyFast
* Lithium
* ModernFix `[Poprawki błędów]`
* MoreCulling
* No Chat Reports `[Social; BEZ Optymalizacja]`
* Noisium
* Nvidium - *Nie trzeba mieć GPU Nvidii - bez Nvidia, po prostu nic nie będzie robił.* **[UWAGA: MOŻE CRASHOWAĆ PRZY GPU NVIDII]**
* Sodium
* ThreadTweak **[WYMAGA CONFIGU! - śmiem założyć, że taki już dodali, ale trzeba się upewnić i possibly dostosować go do naszych modów]**
* Very Many Players
* *biblioteki: FAPI, CCAPI, Indium*

## Z Fabulously Optimised (23 (licząc 2 replacements)  *+5 libs, +9 z SO, +11 usuniętych*):
Ahhhh, Fabulously Optimised... Legenda GhostLanda. The One the Makes GhostLands. Bez FO nie byłoby GL na Fabricu. Problem jest tylko taki, że FO to kinda średni modpack pod optymalizację! Dodaje niecałą połowę rzeczy z SO, który jest złotym standardem optymalizacji (UPDATE: Apparently nie, Performium is (too bad I found out so late). Ale jest wciąż bardzo dobry.); nawpychali dużo modów typu QOL (to be fair - my też, ale my nie udajemy, że głównym celem GhostLand Baseline jest optymalizacja, nawet jeśli nam na niej bardzo zależy), z których większość jest mid i musiałem usunąć; mówią, że jest well-researched, ale to clearly bullshit (inaczej dodaliby C2ME, a nie dodali by Debugify oraz Borderless Mining - patrz: mój rant poniżej, oraz warning autora Cubes Without Borders na temat podobnych modów). Overall - no, takie mocne 2/10. Mimo wszystko, mieli tu parę ciekawych pomysłów. Więc zaimportowałem niektóre co to lepsze mody stąd z powrtoem na naszą paczkę. Poniżej jest ich lista. Gwiazdką oznaczyłem rzeczy, które już były w SO. Also, dołączyłem tagi (bo FO dotyka sporo gałęzi poza optymalizacją, so it's not as simple as it was on SO) i opisy (bo niektóre mody są mało oczywiste - ofc, jeśli po samej nazwie widać, to nie pisałem). Btw! FO dodaje sporo modów, które mogą być wykorzystywane przez texturepacki. Ale tego typu mody często są dependencjami dla innych modów, po prostu. Więc raczej dobrze, że tu są (nawet, jeśli nie mamy żadnego texturepacka, który akurat *jakiegoś konkretnego* używa). Not to mention, że ktoś może chcieć zsideloadować jakąś paczkę (a konieczność pobierania dodatkowych modów dla jej obsługi zawsze jest irytująca - trust me, I've been there).
* ~~LambDynamicLights~~ `[QOL, Ambience]` **ZASTĄPIONE: Sodium Dynamic Lights**
* ~~FabricSkyBoxes Interop~~ `[Tekstury]` - *Dodaje support dla większej ilości formatów skyboxa w Fabric Skyboxes.* **USUNIĘTY: WYWALONO FSB**
* Dynamic FPS `[Optymalizacja, QOL]` - *Spowalnia grę w tle, żeby nie zabierała zasobów, gdy np. szukasz czegoś w necie.*
* Better Mount HUD `[QOL]` - *Pozwala widzieć jedzenie oraz XP-bar, gdy jedziesz konno.*
* ~~Borderless Mining~~ `[QOL]` **ZASTĄPIONE: CUBES WITHOUT BORDERS**
* \*MoreCulling `[Optymalizacja]`
* \*ImmediatelyFast `[Optymalizacja]`
* Memory Leak Fix `[Poprawki błędów]`
* \*FerriteCore `[Optymalizacja]`
* \*Enhanced Block Entities `[Optymalizacja]`
* ~~FADELESS~~ `[QOL]` **USUNIĘTY: ŹLE WYGLĄDA**
* ~~FabricSkyboxes~~ `[Tekstury]` - *Wymagany przez Dramatic Skies. Tak, wiem, Iwo nie lubi DS. Ale trzeba przyznać, że dla ludzi, którzy nie mogą odpalić shaderów - DS pozwala osiągnąć trochę tego shader-like feel.* **USUNIĘTY: JEDNAK NIE (to jednak Celestial był)**
* Mod Menu `[QOL]` - *Fabric nie ma wbudowanej modlisty, więc ten mod ją dodaje*
* Model Gap Fix `[Poprawki błędów]`
* AdvancementInfo `[QOL]` - *Pokazuje co potrzebujesz do danego achievementa.* **[DEPRECATED - jak będzie powodował niekompatybilność, to usuniemy]**
* \*Lithium `[Optymalizacja]`
* ~~YOSBR~~ `[QOL]` **USUNIĘTY: NIEPOTRZEBNY W PACZCE, KTÓRA NIE JEST PUBLIKOWANA NA CF/MR**
* Remove Reloading Screen `[QOL]` - *Reloaduje tekstury w tle, pozwalając tobie nawigować po ustawieniach, gdy reload dalej trwa*
* Continuity `[Tekstury]` - *Connected Textures*
* FastQuit `[Optymalizacja, QOL]` - *Zapisuje świat w tle, pozwalając tobie nawigować po main menu, gdy zapis dalej trwa*
* Zoomify `[QOL]` **[WYMAGA CONFIGU! - keybind; ma duuuużo opcji i niektóre defaulty warto by zmienić (np. zrobić tak, że działa tylko ze spyglassem w inventory - dla realizmu)]**
* \*No Chat Reports `[Social]`
* ~~Puzzle~~ `[QOL]` **USUNIĘTY: ŚREDNIO PRZYDATNY; HISTORIA POWODOWANIA CRASHY**
* ~~e4mc~~ `[Social]` - *Replikuje kluczowy feature Essential Moda (granie po sieci bez serwera), bez spy-wareu i monetyzacji Essential Moda* **USUNIĘTY: MAMY SERWER**
* More Chat History `[Social]`
* MixinTrace `[Debugging]`
* \*Sodium `[Optymalizacja]`
* \*ModernFix `[Optymalizacja, Poprawki błędów]`
* CIT Resewn `[Tekstury]` - *Modele/tekstury zależne od stanu - nazwy, damage value, enchanty, etc.*
* ETF `[Tekstury]` - *Entity Texture Features*
* EMF `[Tekstury]` - *Entity Texture Features*
* Iris `[Ambience]`
* Sodium Extra `[Optymalizacja, QOL]` - *Dodatkowe (przydane) featuresy w Sodium. M. in. nakładka FPS.*
* \*Entity Culling `[Optymalizacja]`
* Animatica `[Tekstury]` - *Pozwala teksturpackom dawać animowane tesktury dla rzeczy które ich nie mają by default*
* Reese's Sodium Options `[QOL]` - *Lepsze UI ustawień dla Sodium. Jeśli UI Sodium wygląda jakoś „dziwnie” (np. GL6), to pewnie dlatego, że nie było tego moda.*
* ~~Controlify~~ `[QOL]` **USUNIĘTY: POWODOWAŁ START-CRASHE PO UPDATE FABRICA**
* ~~Capes~~ `[Social]` **USUNIĘTY: NIKT Z NAS NIE MA O.F. CAPE** *(jak masz, to powiedz - przywrócimy)*
* ~~Debugify~~ `[Poprawki błędów]` **USUNIĘTY: AUTOR KOMPLETNIE NIE WIE CO ROBI; KRADNIE BUGFIXY INNYM MODOM I PAKUJE JE DO SWOJEGO; JAK BĘDZIE Z TYM PROBLEM, TO NIE DOSTANIEMY SUPPORTU, BO SAM NIE BĘDZIE WIEDZIAŁ; LEPIEJ BEZPOŚREDNIO DODAĆ MODY NA BUGFIXY**
* Lanuguage Reload `[QOL]` - *Pozwala ustalić priorytet języków oraz zmieniać ustawienia języka bez reloadu tekstur*
* ~~OptiGUI~~ `[Tekstury]` - *Pozwala teksturpackom zmieniać układy GUI* **USUNIĘTY: JEŚLI CHCEMY CUSTOMOWE UKŁADY GUI, OD TEGO JEST FANCYMENU, NIE TEXTURPACKI**
* Fabrishot `[QOL]` - *Zrzuty ekranu w 4K* **[WYMAGA CONFIGU! - keybind i rozdzielczość]**
* ~~Main Menu Credits~~ **USUNIĘTY: JEŚLI CHCEMY CUSTOMOWE CREDITSY W MAIN MENU, OD TEGO JEST FANCYMENU**
* *biblioteki: YACL, CCAPI, FAPI, Kotlin, Indium*

## Debugging (6 *(1 off);  +1 z FO*)
* spark - *Pokazuje graf TPSów over time, among many other things.*
* BadStdOut - *Ogranicza sytuacje, w których nie da się poznać, jaki mod wysłał coś na logu. Nie eliminuje ich zupełnie, ale at least pomaga. A biorąc pod uwagę, że było to jedno z większych źródeł naszej frustracji przy debugowaniu paczki - mod bardzo przydatny, imo.*
* CME is bad - *Pozwala lepiej śledzić błędy concurrency, poprzez wypisywanie stacktrace każdego wątku, gdy dojdzie do Concurrent Memory Exception (w preciwieństwie do vanilla, która daje trace tylko jednego). Wyłączony by default, bo aby cokolwiek robił, trzeba zarejestrować go jako customowego agenta debugowania Javy - coś, co raczej mało kto będzie robił (chyba, że go wyraźnie o to poprosimy, w ramach naprawiania jakiegoś błędu - a wtedy można też go poprosić o włączenie tego moda z listy, po prostu) z własnej woli (więc po co ten mod ma mu w ogóle startować i tylko RAM jeść)?*
* Unsafe World Random Access Detector - *Pozwala lepiej śledzić błędy concurrency (związane konkretnie z asynchornicznym dostępem do RNG świata) i nawet stara się je samemu jakoś naprawić (funkcja o której nie miałem pojęcia, dopóki na logu nie napisał wprost „attempting to fix”, bo nigdzie o niej nie mówią).*
* Mixin Conflict Helper - *too lazy to explain what it does, but it saved my ass numerous times as I was working on this baseline thing, so I have no doubts it'll come handy when building the actuial modpack*
* Observable - *Pokazuje, jakie bloki i moby generują lagi. Przydatne do wykrywania powodu spadku TPSów w niektórych chunkach oraz do obalania Palmerowego mitu, że Create zabija TPSy.*
* *z FO: MixinTrace*

## Optymalizacja (10 *+3 z FO, +14 z SO*)
* LazyDFU - *Przyspiesza wczytywanie świata, poprzez opóźnianie startu DFU do czasu wczytania chunku wymagającego DFU (zamiast robienia tego na starcie świata - ZAWSZE, nawet gdy DFU nie jest potrzebny). Może spowolnić pierwszy chunk-loading po updacie jakiegoś z modów, ale to raczej nie będzie częsty problem.*
* Chunky - *Sam w sobie nie optymalizuje, ale jest wymagany do pregenu - a to DUŻO daje performace-wise.*
* Memory manager - *Pozwala manualnie prosić GC Javy o wykonanie pełnego cyklu cleanupu. Może spowodować chwilowy lag na dłuższy czas (>1s) - ale za to powinno utrzymać użycie RAMu na niskim poziomie przez dłuższy czas.*
* Krypton - *networking*
* Clumps - *Skleja XP orby*
* Starlight - *Światło* **[INWAZYJNY! - jak coś nie będzie działać z renderowaniem, to pewnie jego wina]**
* Distant Horizons
* Let Me Despawn `[Poprawki błędów]` - *Ogranicza sytuacje pokroju „nieśmiertelny mob, lagujący serwer gdzieś głęboko w jaskini.”*
* Ksyxis - *Przyspiesza start serwera poprzez zupełne usunięcie mechaniki spawn chunków. Imo nieco za bardzo inwazyjny (for not a lot of improvement), ale był od zawsze na GL, więc dodałem go i tu.*
* Async - *Patrz: #dev* **[ALPHA! - jak coś nie będzie działać z entities, to pewnie jego wina]**
* *z SO: wszystko, poza NCR (14)*
* *z FO: Dynamic FPS, FastQuit, Sodium Extra, rzeczy z SO (nie liczę)*

## Poprawki błędów (6  *+3 z FO*)
* Video Tape - *Jak „Memory Leak Fix”, ale dla GPU.*
* Nether Portal Fix - *Ułatwia łączenie portali.*
* AntiGhost - *Usuwa ghost blocki* **[DEPRECATED - jak będzie powodował niekompatybilność, to usuniemy]**
* ServerCore `[Optymalizacja]` - *Port bugfixów i optymalizacji z PaperMC. Wszystkie te, co zmieniają vanilla behaviour, są disabled by default (w przeciwieństwie do PaperMC, który rutynowo psuje vanilla features).*
* Adaptive Tooltips - *Naprawia tooltipy, które na Vanilla lubią uciekać poza ekran.* **[WYMAGA CONFIGU! - USTALIĆ JAKIŚ STYL TOOLTIPÓW Z DOSTĘPNYCH]**
* Gravestones Fix `[Compat]` - *Czyni Gravestoney eksplozjo- i wodo-odpornymi i daje im compat z Trinkets (którego jeszcze nie mamy, ale może się pojawić)*
* *z FO: Memory Leak Fix, Model Gap Fix, ModernFix*

## Ambience (14  *+2 z FO*)
* Dynamic Surroundings - *ambient audio*
* Sodium Shadowy Path Blocks - *przywraca naprawiany przez Sodium bug renderowania, który sprawia, że zagłębione bloki (farmland, ścieżki) wyglądają ciemniej - imo tak jest lepiej, ale that's up for debate*
* Chunks Fade In - *prettier chunk loading*
* Presence Footsteps - *ambient audio*
* Sound Physics Remastered - *ambient audio*
* Falling Leaves - *As seen in: 1.21.5*
* Visuality - *dodatkowe particle*
* AmbientSounds - *ambient audio*
* Visual Workbench - *Stawia itemy na craftingu. Nie do końca ambience, ale ciężko mi to inaczej określić.*
* Wilder Wild - *Poprawy do Wild Update: pyłki, świetliki, tumbleweedy, shelf fungusy-amogusy, etc. Jeden z lepszych ambience modów, imo. Haczyk jest taki, że dodaje trochę własnych biomów, ale ciiiii...*
* Effective - *dodatkowe particle-like-thingys*
* BetterGrassify - *Trawa, która schodzi niżej. More like „visuals”, nie stricte ambience.*
* Immersive Melodies - *Pozwala graczom grać własne utwory z MIDI. Może nie jest to naturalny ambience, ale pozwala nam samym tworzyć ambience (np. grając muzykę na lutni w tawernie).*
* Dynamic Crosshair `[QOL]` - *Zmienia wygląd celownika, w zależności na co patrzysz. Można powiedzieć, że to nie ambience, but I beg to differ. Imo, może mieć bardzo duży wpływ na ambience. Why? Bo ukrywa celownik, gdy nie patrzysz na nic. Wyobraź sobie, że patrzysz ze szczytu góry na epicką dolinę. A very emotional, breathtaking moment. Celownik na środku zaburza wtedy immersję. A z tym modem - nie. Dobra, nie wiem. Może nie do końca tu pasuje. I keep yeeting it between QOL and Ambience; can't decide. Whatever we do - DC zostaje. Michau i ja oboje jesteśmy zdania, że (mimo tego, że robi bardzo mało) ma szokująco ogromny pozytywny impact. UWAGA! Powoduje kolizję z **Better Third Person**. Wyłącz go, jeśli zamierzasz side-loadować tamtego moda (btw, B3P (poza tym jednym incompatibility) działa w paczce w 100%).*
* *z FO: LambDynamicLights, Iris*

## QOL (30 *(1 off);  +12 z FO*)
Nie wpisywałem tu storage modów (poza Traveller's Backpack - tylko po to, żeby przekupić Tymusia), mimo że bardzo chciałem. Ale storage mody raczej powinny być zostawione pod głosowanie (np. jaki tech-styled storage mod, spośród AE2 i RS2; które drawery lubisz; etc.). Oh, btw! Apropos przekupienia Tymusia: IIRC, ty mówiłeś, że masz jakiegoś konkretnego moda na mapę, którego lubisz. Feel free to replace Xaero with it. Nie wydaje mi się, że ktoś poza tobą ma tu silną preferencję w stronę map modów, więc się dostosujemy. (Szczególnie, że Xaero zajmuje obecnie 3 sloty, a bardziej zintegrowane rozwiązanie by to zmniejszyło do jednego.)
* Better Statistics Screen - *Poprawia ekran statystyk*
* Better Advancements - *Poprawia ekran acheivementów*
* Better Ping Display - *Pokazuje prawdziwe milisekundy na TABie, nie jakieś kreski.*
* Controlling - *Search bar w menu keybindów.*
* Apple Skin - *Pokazuje więcej statystyk głodu.*
* Xaero's Minimap
* Xaero's World Map
* World Preview - *pokazuje świat przy jego tworzeniu*
* Jade - *Pokazuje na co patrzysz.*
* MouseTweaks - *Poprawia obsługę inventory myszką.*
* BetterF3 - *kolorki ^-^*
* Enchantment Descriptions - *Szary tekst pod każdym echantem, mówiący co on daje.*
* IPN - *Zamienia narzędzia, które się psują (among other things)*
* REI
* Item Highlighter - *Podświetla nowo-zebrane itemy, jak w większości innych gier.*
* Traveller's Backpack
* BetterCompatChecker - *Pokazuje wersje paczki serwera i klienta, i ostrzega, jeśli nie pasują,* **[WYMAGA CONFIGU! - Ustawić mu naszą paczkę I PAMIĘTAĆ O ZMIENIENIU WERSJI, GDY ROBIMY UPDATE! (bo zawsze był z tym problem)]**
* HT's Tree Chop `[Ambience]` - *Balanced i ładniejszy veinminer (tylko dla drzew).*
* Xaero Zoomout - *Pozwala zobaczyć więcej terenu na ekranie na raz w Xaero.*
* Rebind Narrator - *Pozwala rebindować klawisz narratora.* **[WYMAGA CONFIGU! - WYŁĄCZYĆ NARRATORA]**
* Nature's Compass - Immersive - *Pozwala znaleźć biomy. Edycja „Immmersive” wymaga użycia stołu Kartografa, aby wybrać biom.*
* JLine - *Dodaje autocomplete komend na serwerze.*
* Veinminer - *Pozwala zbierać całe rudy* **[WYMAGA CONFIGU! - WYŁĄCZYĆ NA DRZEWA, ŻEBY SIĘ NE GRYZŁ Z HT'S]**
* Harvest with ease - *right-click harvest* **[WYMAGA CONFIGU! - WŁĄCZYĆ WYMAGANIE MOTYKI, for balancing sake, and to prevent bugs *(patrz: ich opis)*]**
* Panoramics - *Robienie panoram. Mostly useful for dev; potem będzie można usunąć.*
* Toggle Item Frames - *Pozwala ukrywać itemframey (bez komend), robiąc niejako survival-friendly item display.*
* Remove Terralith Into Message - *Usuwa spam na chacie z Terralitha. Wyłączony, bo na razie nie mamy Terralith, ale chciałem to przygotować na później, gdy już będziemy implementować wyniki głosowania.*
* Gravestones
* Just Hammers - *Dodaje młoty znacznie ułatwiające duże wykopaliska.*
* BindPizzeria - *Pozwala wrzucać skróty klawiszowe na pizza-style menu, zamiast zapychać nimi całą klawiaturę. (Pls, let's not make it so that the whole damn keyboard is needed to play this time, I'm SO SICK OF IT! Kanciarz also had the same opinion. We must get the keybind mess under control this edition.).* **[WYMAGA CONFIGU! - GDY JUŻ BĘDZIEMY MIELI FINALNĄ LISTĘ MODÓW, *MUSIMY* OGARNĄĆ MORZE KEYBINDÓW, A DO TEGO TEN MOD SIĘ NAM BARDZO PRZYDA]**
* *z FO: za dużo (12), żeby je tu wymieniać; liczę tylko włączone*

## Tekstury (2  *+5 z FO*)
* ESF - *Entity Sound Features*
* Celestial - *Wymagany przez Dramatic Skies. Tak, wiem, Iwo nie lubi DS. Ale trzeba przyznać, że dla ludzi, którzy nie mogą odpalić shaderów - DS pozwala osiągnąć trochę tego shader-like feel.*
* *z FO: za dużo (6), żeby je tu wymieniać*

## Compat (4 *(3 off)*)
* Iris-GeckoLib Compat - *Dodaje compat GeckoLiba i Iris (bez tego, cienie modeli z GcL są zbugowane). Wyłączony, bo na razie nie mamy GeckoLib, ale to się bardzo szybko zmieni, gdy dodamy jakieś mody na entities, więc chciałem to przygotować na później.*
* Iris-Flywheel Compat - *Dodaje compat Flywheel i Iris (Bez tego, blok-entities z Flywheel (np. pociągi i wiatraki z Create) BARDZO lagują na shaderach. Stąd musiał się wziąć Iwoski mit, że Create zabija FPS.). Wyłączony, bo nie mamy Create/Flywheel, ale to się (mam nadzieję) zmieni, więc chciałem to przygotować na później.*
* Dynamic Crosshair Compat - *Lepszy compat DCh z modded blokami.*
* Pufferfish's Skills x Origins - *Compat modów wymienionych w nazwie. Nie mamy żadnego, więc jest disabled - ale jest spora szansa, że się pojawi choćby jeden z nich (na Originsy będzie głosowanie, jeśli mam zgadywać), a PufferSkils dodaje levelling&skills system - **bardzo podobny do tego, z CraftMine**, z tą różnicą, że mają wewnętrzny system XP, domyślnie nie ma żadnego drzewka (trzeba użyć datapacka - można wziąć od nich przykładowy lub zrobić własny (np. inspirowany drzewkiem CraftMinea lub dopasowany do progression samego GhostLanda)) i (oczywiście) nie ma tego całego aspektu budowania światów (XP zdobywasz „naturalnie”). Michau dodał PufferSkills do swojej paczki (GL7CEu Modern) i - tbh - I'm VERY IMPRESSED. Świetny pomysł. Nie zdziwiłbym się, jeśli Mojang właśnie tym modem się inspirowało robiąc CM. Anyway, dodaję go tu w mniejszym stopniu, żeby się przygotować na obecność PufferSkills/Origins w przyszłości, a w większym, żeby po prostu rozpocząć dialog na ich temat.*

## Social (7  *+2 z FO*)
* FancyMenu - *Pozwala ustawić customowe menu.*
* Smooth Chat - *smooth-scrolluje nowe wiadomości, zamiast pokazywać je znikąd*
* 3D Skin Layers - *Dodaje trochę objętości do skinów.*
* Chat Heads - *Pokazuje na chacie skina osoby, która pisze.*
* Bobby `[QOL, Compat]` - *Zapisuje chunki na kliencie, umożliwiając szybsze wczytywanie świata oraz granie na ogromnych Render Distance z Distant Horizons.*
* CraftPresence - *RichPresnece na Discordzie.* **[WYMAGA CONFIGU! - Ustawić mu naszą paczkę]**
* Skin Restorer - *SkinsRestorer działający po stronie serwera. OD ZAWSZE GhostLand używa client-side skin restoring (co jest mało optymalne, bo bez sensu obciąża sieć klienta, który musi pobrać każdego nowo-napotkanego skina; blokuje też pewne funkcje, np. customizacja wyświetlania warstw). I - tbh - byłem pewien, że systemów serwerowych po prostu nie ma na Fabricu. A jednak był! Po prostu nigdy go nie znaleźliśmy.*
* *custom: Coś na integrację z Discordem (są pre-made, ale w porównaniu ze standardem ustawionym przez DiscordSRV na szkolnym - they all SSSUUUUUUCK).*
* *z FO: NCR (also in SO) i More Chat History*

## **>>*MODÓW ŁĄCZNIE: `145`*<<**
* Debugging - aktywne: 5 dodanych-aktywnch + 1 FO = **6**
* Debugging - wszystkie: 6 dodanych + 1 FO = **7**
* Optymalizacja: 10 dodanych + 3 FO + 14 SO + 1 PoBł = **28**
* Poprawki błędów: 6 dodanych + 3 FO + 1 Opt = **10**
* Ambience: 14 dodanych + 2 FO + 1 QoL = **17**
* QOL - aktywne: 29 dodanych-aktywnych + 12 FO + 1 Amb + 1 Soc = **43**
* QOL - wszystkie: 30 dodanych + 12 FO + 1 Amb + 1 Soc = **44**
* Tekstury: 2 dodane + 5 FO = **7**
* Compat - aktywne: 1 dodane-aktywne + 1 Soc + 1 PoBł = **3**
* Compat - wszystkie: 4 dodanych + 1 Soc + 1 PoBł = **6**
* Social: 7 dodanych + 2 FO = **9**
* Biblioteki: 13+15 = **28**

Powyższe sumy zawierają w sobie dużo powtarzających się modów - by design. Wypisałem je tak „poglądowo”: żeby było wiadomo, ile modów pełni w paczce jakąś rolę - więc jak pełni kilka ról, to będzie w kilku miejscach. Anyway... To nie jest tak, że twój MC ładuje 151 modów, a w przyszłości nawet 156 (bo tyle wychodzi z sumy powyższych). Tyle przecież nawet nie ma w paczce! Spokojnie: nie jest *aż tak* źle.

Btw, jak już jesteśmy w tym temacie: MC ładuje **145-1-1-3=140** - czyli  mniej, ale nadal „trochę” za dużo. Ja bym to ograniczył tak do 100 (which still sounds like a lot, considering Tymon's ridiculus 120 cap - but more on that later) - czyli musimy „nieco” to jeszcze obciąć (nieco/trochę = prawie jedna trzecia xD). Czysto teoretycznie, jeśli nie będziemy liczyć CME is Bad (bo - powiedzmy sobie szczerze - większość graczy nigdy go nie włączy, więc trochę nie fair byłoby go traktować jako moda w paczce - at this rate, jako do mod-capa możnaby równie dobrze liczyć resourcepacki, bo też niby są w paczce, nawet jeśli MC ich rzeczywiście nie ładuje), to mamy tylko 144 mody. Czyli usunięcie *WSZYSTKICH* QOL modów by doprowadziło nas do celu. Pytanie tylko - is it worth it? Bo spora część tych modów jest na prawdę ultra-essential, np. REI. Sure, można powiedzieć „You don't need all that QOL suff, grow up! It makes the game too easy!”, ale wydaje mi się, że taki „minimalism just for the sake of mimimalism” jest nieco bezproduktywny. Według mnie, można to rozwiązać jakoś bardziej pokojowo, bez zrzucania atomówki na prawie jedną trzecią paczki.

### SHADERY: 8
* Complementary Reimagined i Unbound oraz Photon (klasyki GhostLandowe)
* Miniature Shader (kinda mid, ale działa nawet na kartoflu; w połączeniu z Dramatic Skies, wygląda nawet passable)
* Noble, Nostlgia, Pixel-perfect i Rethinking Voxels (IIRC prawie nikt z tego nie korzystał, ale często były na poprzednich GLach, więc niech będą i tu)

### TEXTUREPACKI: 8
* 3D crops
* Chat Reporting Helper
* Dramatic Skies
* Fancy Crops
* Low-on-Fire
* Motszen's Better Leaves (sry; I butchered that)
* Simple Grass Flowers
* Translations for Sodium

### **>>*Łącznie projektów:*<<**
145 modów + 8 shaderów + 8 texturepacków + 1 plik TXT ustawień shaderów (który Modrinth wykrywa jako shader for some reason) = **162**

*Pamiętaj: to nie wszystko mody - a z pośród samych modów: niektóre są wyłączone, a inne będą usunięte. Więc ta liczba wygląda strasznie, ale na prawdę nie jest tak źle. Co nie znaczy, że jest dobrze - tak ze 40 modów wciąż musi polecieć. A nawet wtedy byłoby mało miejsca na rzeczywiste mody - at least, jeśli liczyć cap Tymusia. Speaking of which...*

120? Rly, Tymon? If his limits are to be followed - trzymanie się celu setki modów w baseline, would keep us at **just 20 gameplay mods**. To ofc niedorzecznie za mało (nawet przy jego (imo mocno drakońskim) capie 3 odpowiedzi na osobę - wystarczy tylko 10 odpowiedzi w ankiecie i już przelatujemy). Here's the thing: twój szacunek 120 modów był imo O WIEEELEE zbyt optymistyczny. Od samego początku. Wszystkie Fabricowe GhostLandy do których mam dostęp miały dużo więcej. GL3 (ten z Depustynnieniem i powstaniem GRA) w wersji pierwszej miał ich 216, a GL5 (((przedostatni, which (imo) is an absolute *master-class* in vanilla-feeling packs (a przecież obecny GhostLand ma być podobny, jeśli rozumiem intencję); jeśliby wywalić z tego AE2 i MI oraz nigdy bym nie wiedział o Create (ie. nie potrafiłbym go poznać jako moda), to gdyby ktoś mi powiedział, że tak będzie wyglądać MC za 20 lat - I'd probably believe them))) dużo mniej, ale wciąż powyżej sporo 120: 173 (chociaż wzrosło do 177 w ostatniej wersji). Takie precyzyjne wartości są trochę arbitrary, ale stanowią dobry punkt odniesienia. Imo, cel zbliżony do tego z GL5 jest o wiele bardziej osiągalny. Ja bym dał cap na <190, a oficjalnie ogłosił 180 - te 9 zapasu na potencjalne integracje między zainstalowanymi modami, lub scenariusze typu „Oj pliiiisss... 180-ileś, a 180? To prawie brak różnicy. Come on, dodajcie *moda X*!”. 80 modów na gameplay features i worldgen to prefekcyjnie fine liczba, jeśli paczka ma być vanilla-like. 20, natomiast - to szaleństwo.

## **>>*FINAL NOTES AND CREDITS*<<**
* W niektórych miejscach napisałem, że trzeba ustawić keybindy. Ale prawie na pewno będzie ich dużo więcej, niż te kilka wymienionych. Obecnie, tylko powyłączałem większość keybindów, tak żeby dało się grę obsługiwać, bez 300 konfliktów na guzikach. Ale trzeba będzie je jakoś thoughtfully powłączać z powrotem. Może nam w tym pomóc Bind Pizzeria.
* **CONFIGI! I CAN'T STRESS THIS ENOUGH!** *z naciskiem na często pomijane rzeczy, np. CraftPresence, BetterCompatChecker lub zamknięcie paska FancyMenu (also, jeśli chodzi o FM, to fajnie by było trochę sprzątnąć menu pauzy, bo po instalacji World Preview oraz wywaleniu Remove GFARB jest mocno cluttered)*
* Sprawdź [CONTRIBUTING](CONTRIBUTING.md), jeśli chcesz coś zmieniać w tym repo (a mam nadzieję, że chcesz - bo trochę średnio mam ochotę być jedynym robiącym thinning out tej abominacji).

### Performace analysis:
Overall, paczka działa niesamowicie płynnie. Na obecnych ustawieniach radzi sobie nawet lepiej, niż GL6 (na... Yyy... Chyba pi-razy-drzwi podobnych ustawieniach). For all it's gameplay flaws, GL6 was *insanley* well optimised. Pamiętam mój szok z tego powodu i jak gratulowałem Iwowi (szczególnie, że paczka była na NeoForge, który historycznie radził sobie z tym średnio). Więc jak ta paczka trzyma podobny poziom, to na pewno będzie git.

Jeśli chodzi o jakieś bardziej concrete wartości, a nie „vibes”, to zapraszam do [starszych wersji tego dokumentu](https://github.com/Team-GhostLand/GhostLand7-Baseline/blob/4d0e6945f799cc8912438611b79bc25e86958884/README.md#performace-analysis), bo tam dałem bardziej dokładne wyniki benchamrku. Zostały usunięte z obecnej wersji, bo wydają się być outdated. Like... Przed chwilą sobie latałem po świecie i ofc miałem jakieś 22FPSy at lowest (bo wczytywanie chunków) - ale po wylądowaniu, często przekraczały 90 (przy chodzeniu (ie. wczytywaniu chunków, ale w normalniejszym tempie) spadały do 70 co chwilę (ie. co nowy slice chunków), but that's still good). Like... This almost never happens! Wasn't even the case on GL6! I - oczywiście -  nie było też zarejestrowane we wcześniejszych benchamrkach. I to jest powód dla którego musiałem usunąć jego wyniki. Nie wiem co poprawiło liczby tak bardzo (większość ustawień jest more or less zbliżona do Potato, z Render Distance na 12, a modów usunęliśmy tylko kilka), but whatever it was - it'd likely affect all other categories. A re-testować kilkunastu konfiguracji mi się po prostu nie chce. Jak chcesz sprawdzić stare liczby - proszę bardzo, nikt ci nie broni. Ale wiedz, że paczka radzi sobie jeszcze lepiej, niż tam napisano (a już tamte wyniki były w miarę git).

Poza FPS, warto też zwrócić uwagę na bardzo dobry czas startu (zazwyczaj poniżej minuty (np. just now zrobił to w 50.747s), okazjonalnie poniżej półtorej - szczególnie przy pierwszym uruchomieniu od włączenia kompa, co ma sens, bo OS jeszcze nie zdążył zapisać plików w cache). Ma też bardzo niskie zużycie RAMu - nie przekroczyło u mnie ani razu 20% (dałem mu ok. 12,5GB - co znaczy, że paczka nie przekracza nawet 3GB i to z dużym zapasem). Tak więc jest jeszcze DUUUŻO miejsca na zapchanie jej pierdylionem modów dodających custom modele/tekstury (ie. like... 99% of all gameplay-features-focused mods), które zawsze zajmują najwięcej RAMu i czasu na starcie. :-P

### Zmienione default ustawienia:
* Wyłączenie keybinda na fullscreen, pasek szybkiego dostępu creative (nie mówię o F3+F4, tylko swapowaniu hotbara), Narratora (Ave!), Advancementy i znaczą większości modded klawiszy.
* Włączenie/przepisanie kilku klawiszy debuggowania dla modów oraz kamerę filmową na F10.
* Rocket Boost samolotu na >, bo wygląda jak rakieta, a B był zajęty przez Traveler's Backpacks.
* Włączono przybory operatora (dostęp do command blocków, etc. z creative menu).
* Włączono i ustawiono kolejność resourcepacków (poza Dramatic Skies, żeby Iwo nie marudził oraz Better Leaves, bo ma duży performance impact i o ile na release przydałoby się to ponownie włączyć, o tyle podczas dev nie musimy się przejmować visuals aż tak bardzo, a kilka dodatkowych FPSów zawsze się przyda).
* Polski się automatycznie wczytał
* Biome Blend podkręcone do 5 z 2
* FOV: 86 z default 90 (co chyba też jakiś mod zmienia, bo powinno być Normalne)
* Max. jasność
* Grafika na Fast, ale kilka rzeczy na Fancy (np. liście i chmury)
* Zasięg chmur: 300%
* Wskaźnik ataku na hotbar (chciałem to zmienć na default, but I forgor)
* Ograniczono efekty pola widzenia (chciałem to zmienć na default, but I forgor)
* Wyłączono gaszenie dynamic lights pod wodą; włączono DynLight dla entities; włączono fast DL dla Creeperów
* Shadowyness ścieżek na 50%
* Włączona nakładka Sodium (prawy górny róg; tylko basic FPS)
* Włączone advanced tooltips.
* Wyłączono pauzę po od-focusowaniu okna gry.
* Generalnie pogrzebano w opcjach Distant Horizons; na bazie presetu Low; turned it off before exporting
* Generalnie pogrzebano w opcjach Miniature Shader; na bazie presetu Low
* Wyłączono View Bobbing / Animację chodzenia. (chciałem to zmienć na default, but I forgor)
* Wyłączono fullscreen (z jakiegoś powodu, gra domyślnie wystartowała za pierwszym razem w tym trybie). Dwukrotnie, lol.
* Zamknięto 1st-launch warning narratora MC, FancyMenu, Observable oraz Controlify.
* Render distance na 12
* Winieta była domyślnie wyłączona, ale to chyba zmienił jakiś mod - bo nie powinna być.
* Zoom pod C (jak za starych dobrych OptiFineowych czasów)

### Credits/Licensing:
* Licensed under MIT (ie. the „Do whatever the fuck you want”-clause), with the exception of a single file (mentioned later).
* [Guzio](https://github.com/GuzioMG), [MidnightSP](https://github.com/Midnight-SP), other people who didn't push any patches, but nevertheless helped us in some way on [our Discord](https://discord.gg/qCNUYBXY7P).
* *#GhostLand Project* – by [Jifo](https://github.com/JIFO0)
* Inside an `.mrpack` uploaded to this repo, sits a JAR downloaded from [this amazing repo](https://github.com/Bliss-tbh/Async-1.20.1/) (seriously, those commit messages are awesome). Said JAR is a 1.20.1 port of Async. I *realllly* wanted to avoid embedding JARs inside the modpack file because this usually means I'm basically robbing the creator of prestige (from download count) and ad revenue, but that couldn't be avoided, as this mod has *never* been published onto any mod repository. I had to grab it directly from GH. ...Which also means that I'm not affecting any download/money numbers (they don't exist yet), so I hope this is fine. License-wise, I'm *pretty sure* it would be fine, as MIT is GPL-compatible (tho I believe GPL-compat *may* work the other way (ie. re-licensing MIT code under GPL (not GPL under MIT, as it would *seem* here), so I'd like to clarify that **I'M NOT trying to relicense that mod under MIT**, but rather it's merely a GPL file (that'll stay GPL, no matter what I do) embedded inside an MIT repo, and if you ever try to use said repo in an MIT-compliant way (but one that'd break the GPL), this file MUST be removed), but I *also* believe that it's possible to do what I did here, ie. for a non-GPL app to embed GPL code (so long as said code isn't modified in any way - which it wasn't, in this case) - eg. various proprietary GTK/Qt-based apps) - but some mod authors often have their own policies for modpack embedding, that extend outside a normal license. I couldn't find any said policies attached to this port of Async (and didn't check the original because - well - they're both *very* different mods, with this one having a lot of code modified, so that old policy shouldn't apply here), so I followed the license instead. If that's a problem, please contact us. I'm sure a solution can be worked out.