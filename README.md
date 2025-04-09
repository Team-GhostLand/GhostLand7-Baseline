# GL baseline
A list of „modded MC essentials” that for whatever reason must be inside GhostLand 7 (and preferably future GL editions). Note: the rest of this doc (apart from the very last section) is in Polish.

O ile nie podano inaczej, `[tagi]` oznaczają, że mod należy do kategorii z której się wziął, ale posiada też aspekty pasujące do tej z taga (np. Mod w QoL z `[Ambience]` jest QoL, ale ma w sobie elementy Ambience-moda).

## Dependencje (16 udało mi się „złapać”; 20 musiało dojść „gdzieś po drodze”; pewnie można część usunąć (była Wielka Czystka, after all - część dependencji na pewno straciła swoje „dzieci”), ale to lepiej robić jak przeczyścimy wszystko inne):
* Fabric API (prawie wszystko)
* Cloth Config API (prawie wszystko)
* YACL (idk co, ale był w FO - więc pewnie coś stamtąd)
* Fabric Language Kotlin (dość sporo)
* Main Menu Credits (idk co, ale był w FO - więc pewnie coś stamtąd; jest szansa, że nic, bo ma funkcjonalność stand-alone, która może być wykorzystywana przez FO) - *daje opcję ustawienia credistwów w Main Menu - jeśli tylko po to był w FO i nie ma dependencji, to można go wywalić, bo to samo możemy zrobić przez Fancy Menu*
* Indium (Pozwala używać z Sodium wieloma modami)
* Omnicore (Mod Menu Stylizer)
* Sodium Options API (niektóre mody dodające rzeczy do ustawień Sodium, które z jakiegokolwiek powodu nie robią tego przez wbudowane API Sodium) - *W połączeniu z Reese's Options: Dodaje ikonki pokazujące, który mod dodał co do ustawień Sodium. Dział dla wszystkich modów; nie tylko do tych rejestrujących przez to.*
* CreativeCore (AmbientSounds)
* Konkrete (FancyMenu, Drippy Loading Screen)
* Melody (FancyMenu)
* Architectury API (dość sporo)
* Balm (wszelkie mody Blaya, ale nie wiem kim jest Blay)
* libIPN (IPN *(duh)*)
* Searchables (Controlling)
* Immersive Aircraft (Man of Many Planes) - *Niby dodaje jakieś własne basic-ass samolociki, but let's face it: it's no fun without MoMP.*
* *Niezidentyfikowane (auto-dodały się gdzieś w miedzyczasie i nie zauważyłem kiedy): Almanac, Athena, Bookshelf, Cardinal Components API, CICADA, Cobweb, Forge Config API Port, FrozenLib, Iceberg, Lithostitched, Moonlight Lib, OmniCore, Puzzles Lib, Resourceful Lib, Silk, SuperMartijn642's Config Lib, SuperMartijn642's Core Lib, TCDCommons API, Textile, UniLib*

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
* Nvidium - *Nie trzeba mieć GPU Nvidii - bez Nvidia, po prostu nic nie będzie robił.*
* Sodium
* ThreadTweak **[WYMAGA CONFIGU! - śmiem założyć, że taki już dodali, ale trzeba się upewnić i possibly dostosować go do naszych modów]**
* Very Many Players
* *biblioteki: FAPI, CCAPI, Indium*

## Z Fabulously Optimised (27 (licząc replacements)  *+6 libs, +9 z SO, +6 usuniętych*):
Ahhhh, Fabulously Optimised... Legenda GhostLanda. The One the Makes GhostLands. Bez FO nie byłoby GL na Fabricu. Problem jest tylko taki, że FO to kinda średni modpack pod optymalizację! Dodaje niecałą połowę rzeczy z SO, który jest złotym standardem optymalizacji (UPDATE: Apparently nie, Performium is (too bad I found out so late). Ale jest wciąż bardzo dobry.); nawpychali dużo modów typu QOL (to be fair - my też, ale my nie udajemy, że głównym celem GhostLand Baseline jest optymalizacja, nawet jeśli nam na niej bardzo zależy), z których większość jest mid i musiałem usunąć; mówią, że jest well-researched, ale to clearly bullshit (inaczej dodaliby C2ME, a nie dodali by Debugify oraz Borderless Mining - patrz: mój rant poniżej, oraz warning autora Cubes Without Borders na temat podobnych modów). Overall - no, takie mocne 2/10. Mimo wszystko, mieli tu parę ciekawych pomysłów. Więc zaimportowałem niektóre co to lepsze mody stąd z powrtoem na naszą paczkę. Poniżej jest ich lista. Gwiazdką oznaczyłem rzeczy, które już były w SO. Also, dołączyłem tagi (bo FO dotyka sporo gałęzi poza optymalizacją, so it's not as simple as it was on SO) i opisy (bo niektóre mody są mało oczywiste - ofc, jeśli po samej nazwie widać, to nie pisałem). Btw! FO dodaje sporo modów, które mogą być wykorzystywane przez texturepacki. Ale tego typu mody często są dependencjami dla innych modów, po prostu. Więc raczej dobrze, że tu są (nawet, jeśli nie mamy żadnego texturepacka, który akurat *jakiegoś konkretnego* używa). Not to mention, że ktoś może chcieć zsideloadować jakąś paczkę (a konieczność pobierania dodatkowych modów dla jej obsługi zawsze jest irytująca - trust me, I've been there).
* ~~LambDynamicLights~~ `[QOL, Ambience]` **ZASTĄPIONE: Sodium Dynamic Lights**
* FabricSkyBoxes Interop `[Tekstury]` - *Dodaje support dla większej ilości formatów skyboxa w Fabric Skyboxes.*
* Dynamic FPS `[Optymalizacja, QOL]` - *Spowalnia grę w tle, żeby nie zabierała zasobów, gdy np. szukasz czegoś w necie.*
* Better Mount HUD `[QOL]` - *Pozwala widzieć jedzenie oraz XP-bar, gdy jedziesz konno.*
* ~~Borderless Mining~~ `[QOL]` **ZASTĄPIONE: CUBES WITHOUT BORDERS**
* \*MoreCulling `[Optymalizacja]`
* \*ImmediatelyFast `[Optymalizacja]`
* Memory Leak Fix `[Poprawki błędów]`
* \*FerriteCore `[Optymalizacja]`
* \*Enhanced Block Entities `[Optymalizacja]`
* ~~FADELESS~~ `[QOL]` **USUNIĘTY: ŹLE WYGLĄDA**
* FabricSkyboxes `[Tekstury]` - *Wymagany przez Dramatic Skies.*
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
* Animatica `[Tekstury]` - *animowane tesktury dla rzeczy które ich nie mają by default*
* Reese's Sodium Options `[QOL]` - *Lepsze UI ustawień dla Sodium. Jeśli UI Sodium wygląda jakoś „dziwnie” (np. GL6), to pewnie dlatego, że nie było tego moda.*
* Controlify `[QOL]` - *Dodaje wsparcie kontrolera* **[WYMAGA CONFIGU! - Chować informację o potrzebie natywnej biblioteki by default]**
* ~~Capes~~ `[Social]` **USUNIĘTY: NIKT Z NAS NIE MA O.F. CAPE** *(jak masz, to powiedz - przywrócimy)*
* ~~Debugify~~ `[Poprawki błędów]` **USUNIĘTY: AUTOR KOMPLETNIE NIE WIE CO ROBI; KRADNIE BUGFIXY INNYM MODOM I PAKUJE JE DO SWOJEGO; JAK BĘDZIE Z TYM PROBLEM, TO NIE DOSTANIEMY SUPPORTU, BO SAM NIE BĘDZIE WIEDZIAŁ; LEPIEJ BEZPOŚREDNIO DODAĆ MODY NA BUGFIXY**
* Lanuguage Reload `[QOL]` - *Pozwala ustalić priorytet języków oraz zmieniać ustawienia języka bez reloadu tekstur*
* OptiGUI `[Tekstury]` - *Pozwala teksturpackom zmieniać układu GUI*
* Fabrishot `[QOL]` - *Zrzuty ekranu w 4K* **[WYMAGA CONFIGU! - keybind i rozdzielczość]**
* *biblioteki: YACL, CCAPI, FAPI, Kotlin, MMC, Indium*

## Debugging (7  *+1 z FO*)
3 mody, które nie mają opisu (i MixinTrace z FO) nie mają go dlatego, że byłby za długi lub zbyt techniczny. But trust me bro, we need them. TL;DR: 2 na Mixiny, 2 na concurrency.
* spark - *Pokazuje graf TPSów over time, among many other things.*
* BadStdOut - *Ogranicza sytuacje, w których nie da się poznać, jaki mod wysłał coś na logu. Nie eliminuje ich zupełnie, ale at least pomaga. A biorąc pod uwagę, że było to jedno z większych źródeł naszej frustracji przy debugowaniu paczki - mod bardzo przydatny, imo.*
* CME is bad
* Unsafe World Random Access Detector
* Mixin Conflict Helper
* StackDeobfuscator - *Zastępuje w logu obfuscated nazwy (typu `net.minecraft.class_234535`) na ich prawdziwe (np. `net.minecraft.entity.Creeper`). To było drugie największe źródło naszej frustracji, więc bardzo dobrze, że udało się je wyeliminować.*
* Observable - *Pokazuje, jakie bloki i moby generują lagi. Przydatne do wykrywania powodu spadku TPSów w niektórych chunkach oraz do obalania Palmerowego mitu, że Create zabija TPSy.*
* *z FO: MixinTrace*

## Optymalizacja (10 *+3 z FO, +14 z SO*)
* LazyDFU - *Przyspiesza wczytywanie świata, poprzez opóźnianie startu DFU do wczytania chunku wymagającego DFU (zamiast robienia tego na starcie świata - ZAWSZE, nawet gdy DFU nie jest potrzebny). Może spowolnić pierwszy chunk-loading po updacie jakiegoś z modów, ale to raczej nie będzie częsty problem.*
* Chunky - *Sam w sobie nie optymalizuje, ale jest wymagany do pregenu - a to DUŻO daje performace-wise*
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

## Poprawki błędów (5  *+3 z FO*)
* Video Tape - *Jak „Memory Leak Fix”, ale dla GPU.*
* Nether Portal Fix - *Ułatwia łączenie portali.*
* AntiGhost - *Usuwa ghost blocki* **[DEPRECATED - jak będzie powodował niekompatybilność, to usuniemy]**
* ServerCore `[Optymalizacja]` - *Port bugfixów i optymalizacji z PaperMC. Wszystkie te, co zmieniają vanilla behaviour, są disabled by default (w przeciwieństwie do PaperMC, który rutynowo psuje vanilla features).*
* Adaptive Tooltips - *Naprawia tooltipy, które na Vanilla lubią uciekać poza ekran.* **[WYMAGA CONFIGU! - USTALIĆ JAKIŚ STYL TOOLTIPÓW Z DOSTĘPNYCH]**
* *z FO: Memory Leak Fix, Model Gap Fix, ModernFix*

## Ambience (13  *+2 z FO*)
* Dynamic Surroundings - *ambient audio*
* Sodium Shadowy Path Blocks - *przywraca naprawiany przez Sodium bug renderowania, który sprawia, że zagłębione bloki (farmland, ścieżki) wyglądają ciemniej - imo tak jest lepiej, ale that's up for debate*
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

## QOL (28 *(1 off);  +13 z FO*)
Nie wpisywałem tu storage modów (poza Traveller's Backpack - tylko po to, żeby przekupić Tymusia), mimo że bardzo chciałem. Ale storage mody raczej powinny być zostawione pod głosowanie (np. jaki tech-styled storage mod, spośród AE2 i RS2; które drawery lubisz; etc.). Oh, btw! Apropos przekupienia Tymusia: IIRC, ty mówiłeś, że masz jakiegoś konkretnego moda na mapę, którego lubisz. Feel free to replace Xaero with it. Nie wydaje mi się, że ktoś poza tobą ma tu silną preferencję w stronę map modów, więc się dostosujemy. (Szczególnie, że Xaero zajmuje obecnie 3 sloty, a bardziej zintegrowane rozwiązanie by to zmniejszyło do jednego.)
* Better Statistics Screen - *Poprawia ekran statystyk*
* Better Advancements - *Poprawia ekran acheivementów*
* Better Ping Display - *Pokazuje prawdziwe milisekundy na TABie, nie jakieś kreski.*
* Remove GFRAB - *Usuwa zgłaszanie błędów i przekazywanie opinii z menu pauzy (skoro i tak jesteśmy na modpacku, więc Mojangowy bugtracker nas nie dotyczy)* **[Potencjalnie replikowalne przez FancyMenu - but whoever decides to remove it from here MUST PROMISE THAT THEY'LL ACTUALLY DO IT VIA FANCYMENU]**
* Controlling - *Search bar w menu keybindów.*
* Apple Skin - *Pokazuje więcej statystyk głodu.*
* Xaero's Minimap
* Xaero's World Map
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
* Man of Many Planes - *Samolotyyyyy ^-^*
* Harvest with ease - *right-click harvest* **[WYMAGA CONFIGU! - WŁĄCZYĆ WYMAGANIE MOTYKI, for balancing sake, and to prevent bugs *(patrz: ich opis)*]**
* Panoramics - *Robienie panoram. Mostly useful for dev; potem będzie można usunąć.*
* Toggle Item Frames - *Pozwala ukrywać itemframey (bez komend), robiąc niejako survival-friendly item display.*
* Remove Terralith Into Message - *Usuwa spam na chacie z Terralitha. Wyłączony, bo na razie nie mamy Terralith, ale chciałem to przygotować na później, gdy już będziemy implementować wyniki głosowania.*
* *z FO: za dużo (13), żeby je tu wymieniać; liczę tylko włączone*

## FancyMenu (2)
* FancyMenu - *Pozwala ustawić customowe menu.*
* Drippy Loading Screen - *Pozwala ustawić customowy loading screen.*

## Tekstury (2  *+8 z FO*)
* ESF - *Entity Sound Features*
* Celestial - *Wymagany przez Dramatic Skies. Tak, wiem, Iwo nie lubi DS. Ale trzeba przyznać, że dla ludzi, którzy nie mogą odpalić shaderów - DS pozwala osiągnąć trochę tego shader-like feel.*
* *z FO: za dużo (8), żeby je tu wymieniać*

## Compat (5 *(4 off)*)
* Iris-GeckoLib Compat - *Dodaje compat GeckoLiba i Iris (bez tego, cienie modeli z GcL są zbugowane). Wyłączony, bo na razie nie mamy GeckoLib, ale to się bardzo szybko zmieni, gdy dodamy jakieś mody na entities, więc chciałem to przygotować na później.*
* Iris-Flywheel Compat - *Dodaje compat Flywheel i Iris (Bez tego, blok-entities z Flywheel (np. pociągi i wiatraki z Create) BARDZO lagują na shaderach. Stąd musiał się wziąć Iwoski mit, że Create zabija FPS.). Wyłączony, bo nie mamy Create/Flywheel, ale to się (mam nadzieję) zmieni, więc chciałem to przygotować na później.*
* Dynamic Crosshair Compat - *Lepszy compat DCh z modded blokami.*
* Pufferfish's Skills x Origins - *Compat modów wymienionych w nazwie. Nie mamy żadnego, więc jest disabled - ale jest spora szansa, że się pojawi choćby jeden z nich (na Originsy będzie głosowanie, jeśli mam zgadywać), a PufferSkils dodaje levelling&skills system - **bardzo podobny do tego, z CraftMine**, z tą różnicą, że mają wewnętrzny system XP, domyślnie nie ma żadnego drzewka (trzeba użyć datapacka - można wziąć od nich przykładowy lub zrobić własny (np. inspirowany drzewkiem CraftMinea lub dopasowany do progression samego GhostLanda)) i (oczywiście) nie ma tego całego aspektu budowania światów (XP zdobywasz „naturalnie”). Michau dodał PufferSkills do swojej paczki (GL7CEu Modern) i - tbh - I'm VERY IMPRESSED. Świetny pomysł. Nie zdziwiłbym się, jeśli Mojang właśnie tym modem się inspirowało robiąc CM. Anyway, dodaję go tu w mniejszym stopniu, żeby się przygotować na obecność PufferSkills/Origins w przyszłości, a w większym, żeby po prostu rozpocząć dialog na ich temat.*
* Create Man of Many Planes - *Wyłączony, bo na razie nie mamy Create, ale to się (mam nadzieję) zmieni, więc chciałem to przygotować na później.*

## Social (6  *+2 Z FO*)
* Smooth Chat - *smooth-scrolluje nowe wiadomości, zamiast pokazywać je znikąd*
* 3D Skin Layers - *Dodaje trochę objętości do skinów.*
* Chat Heads - *Pokazuje na chacie skina osoby, która pisze.*
* Bobby `[QOL, Compat]` - *Zapisuje chunki na kliencie, umożliwiając szybsze wczytywanie świata oraz granie na ogromnych Render Distance z Distant Horizons.*
* CraftPresence - *RichPresnece na Discordzie.* **[WYMAGA CONFIGU! - Ustawić mu naszą paczkę]**
* Skin Restorer - *SkinsRestorer działający po stronie serwera. OD ZAWSZE GhostLand używa client-side skin restoring (co jest mało optymalne, bo bez sensu obciąża sieć klienta, który musi pobrać każdego nowo-napotkanego skina; blokuje też pewne funkcje, np. customizacja wyświetlania warstw). I - tbh - byłem pewien, że systemów serwerowych po prostu nie ma na Fabricu. A jednak był! Po prostu nigdy go nie znaleźliśmy.*
* *custom: Coś na integrację z Discordem (są pre-made, ale w porównaniu ze standardem ustawionym przez DiscordSRV na szkolnym - they all SSSUUUUUUCK).*
* *z FO: NCR (also in SO) i More Chat History*

## Dekoracje - **USUNIĘTE; TU ZOSTAJĄ TYLKO JAKO OSOBISTE NOTATKI**
Mody:
* ~~Supplementaries - *Zestaw losowych dekoracji. Często widywany na GhostLandach.*~~
* ~~Rechiseled - *Dodaje wersje bloków.*~~
* ~~Chipped - *Dodaje wersje bloków.*~~
* ~~All The Trims - *Pozwala użyć więcej materiałów do robienia armor-trimów. Działa z Dynamic Trim.*~~
* ~~Decorative Blocks - *Zestaw losowych dekoracji.* **[DEPRECATED - jak będzie powodował niekompatybilność, to usuniemy]**~~

Compat:
* ~~Chipped Express - *Pozwala używać wielu różnych modów (np. Create i AE2 - to mention stuff we (likely will) have), żeby auto-craftować rzeczy z Chipped.*~~
* ~~Chipped x Create - *Pozwala używać Create, żeby auto-craftować i auto-un-craftować rzeczy z Chipped. Wyłączony, bo na razie nie mamy Create. NOTE: UnChipped nie pozwala automatyzować, a Chipped Express wspiera więcej modów niż Create, więc każdy z tych modów ma powód, by tu być. (Nawet, jeśli mają lekki feature overlap).*~~
* ~~Rechiseled: Create - *Pozwala używać Create, żeby auto-Chiselować. Wyłączony, bo na razie nie mamy Create, ale to się (mam nadzieję) zmieni, więc chciałem to przygotować na później.*~~

Related:
* ~~UnChipped `[QOL]`- *Pozwala przywracać z-chipped-owane bloki do ich stanu pierwotnego.*~~
* ~~Reintegrated: Chipped `[Ambience]` - *Dodaje bloki z Chipped do naturalnego worldgenu i struktur. Nie do końca ambience, ale ciężko mi to inaczej określić.*~~

## **>>*MODÓW ŁĄCZNIE*<<**
### _**`154`**_
Z sumy wszystkiego powyżej wychodzi 156, ale Modrinth mówi, że modów jest 154. Wydaje mi się, że jakieś 2 zostały pominięte w ramach Wielkiej Czystki (tzn. usunąłem je z MR, ale nie stąd), ale staram się jak mogę i nie potrafię znaleźć żadnego pominiętego z tej listy w paczce. (Jak ktoś znajdzie, wyślę Blikiem piątaka. Nie żartuję.) Jako kanoniczną ilość przyjmijmy wartość z Modrinth (Bo... Well... Tyle *rzeczywiście* jest w paczce) i po prostu pamiętajmy, że jak matma się nie zgadza, to mamy odjąć/dodać 2.
* Debugging: 7 dodanych + 1 FO = **8**
* Optymalizacja: 10 dodanych + 3 FO + 14 SO + 1 PoBł = **28**
* Poprawki błędów: 5 dodanych + 3 FO + 1 Opt = **9**
* Ambience: 13 dodanych + 2 FO + 1 QoL = **16**
* QOL - aktywne: 27 dodanych-aktywnych + 13 FO + 1 Amb + 1 Soc = **42**
* QOL - wszystkie: 28 dodanych + 13 FO + 1 Amb + 1 Soc = **43**
* FancyMenu: **2** dodane
* Tekstury: 2 dodane + 8 FO = **10**
* Compat - aktywne: 1 dodane-aktywne + 1 Soc = **2**
* Compat - wszystkie: 5 dodanych + 1 Soc = **6**
* Social: 6 dodanych + 2 FO = **8**
* Biblioteki: 16+20 = **36**

Powyższe sumy zawierają w sobie dużo powtarzających się modów - by design. Wypisałem je tak „poglądowo”: żeby było wiadomo, ile modów pełni w paczce jakąś rolę - więc jak pełni kilka ról, to będzie w kilku miejscach. Anyway... To nie jest tak, że twój MC ładuje 167 modów (a tyle wychodzi z sumy powyższych). Tyle przecież nawet nie ma w paczce! Spokojnie: nie jest *aż tak* źle.

Btw, jak już jesteśmy w tym temacie: MC ładuje 154-1-4=150 - czyli  mniej, ale nadal „trochę” za dużo. Ja bym to ograniczył tak do 100 - czyli musimy „nieco” to jeszcze obciąć (nieco/trochę = dosłownie jedna trzecia xD). Ale co ciekawe, nawet usunięcie WSZYSTKICH QOL modów (które, rzeczywiście, stanowią niezbalansowanie duży odsetek paczki) nie umieści nas poniżej setki, a SZCZERZE myślałem, że tak się stanie i że większość kłótni w fazie minimalizacji paczki będzie właśnie o importance konkretnych QOLek (szczególnie, że są dość subiektywne) i że wynikiem tych kłótni (tylko tych, czyli bez zahaczania o inne kategorie modów) będzie pozbycie się tylu modów, że nas to dobije do celu (setki). A tak jednak nie będzie. Cóź, szykuje się ciekawy dyskurs, ig...
### 120? Rly?
If Tymon's limits are to be followed - trzymanie się celu setki modów w baseline, would keep us at **just 20 gameplay mods**. To ofc niedorzecznie za mało (nawet przy jego (imo mocno drakońskim) capie 3 odpowiedzi na osobę - wystarczy tylko 10 odpowiedzi w ankiecie i już przelatujemy). Here's the thing: twój szacunek 120 modów był imo O WIEEELEE zbyt optymistyczny. Od samego początku. Wszystkie Fabricowe GhostLandy do których mam dostęp miały dużo więcej. GL3 w wersji pierwszej miał ich 216, a GL5 (((which (imo) is an absolute *master-class* in vanilla-feeling packs (a przecież obecny GhostLand ma być podobny, jeśli rozumiem intencję); jeśliby wywalić z tego AE2 i MI oraz nigdy bym nie wiedział o Create (ie. nie potrafiłbym go poznać jako moda), to gdyby ktoś mi powiedział, że tak będzie wyglądać MC za 20 lat - I'd probably believe them))) dużo mniej, ale wciąż powyżej sporo 120: 173 (chociaż wzrosło do 177 w ostatniej wersji). Takie precyzyjne wartości są trochę arbitrary, ale stanowią dobry punkt odniesienia. Imo, cel zbliżony do tego z GL5 jest o wiele bardziej osiągalny. Ja bym dał cap na <190, a oficjalnie ogłosił 180 - te 9 zapasu na potencjalne integracje między zainstalowanymi modami, lub scenariusze typu „Oj pliiiisss... 180-ileś, a 180? To prawie brak różnicy. Come on, dodajcie *moda X*!”. 80 modów na gameplay features i worldgen to prefekcyjnie fine liczba, jeśli paczka ma być vanilla-like.
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
### Performace analysis:
Overall, paczka działa niesamowicie płynnie. Pragnę szczególną uwagę zwrócić na kategorię Potato: Wygląda prawie tak samo, jak GL6. Przedziały FPS dla danych render distance były bardzo podobne. Ustawienia graficzne też: Better Leaves i Dramatic Skies nie było w ogóle (analogiczne do ich wyłączenia w kategorii Potato), a inne ustawienia MC prawie zawsze robię takie same (więc na GL6 i w Potato probably były podobne). For all it's gameplay flaws, GL6 was *insanley* well optimised. Pamiętam mój szok z tego powodu i jak gratulowałem Iwowi (szczególnie, że paczka była na NeoForge, który historycznie radził sobie z tym średnio). Więc jak ta paczka trzyma podobny poziom, to na pewno będzie git.

Różnice z GL6 pojawiają się, gdy włączymy DH i shadery. Przede wszystkim, tam DH był kompletnie unplayable dla mnie. Większości ludzi działało, ale mi lagowały niemiłosiernie, nawet na najniższych możliwych ustawieniach (i DH, i vanilla graphics - np. 2 chunki zwykłego RD, a 32 (minimum) chunków LOD). Z Shaderami było odwrotnie: o tyle też Miniature Shader ostro bił FPS, o tyle *raczej* nie zchodziły poniżej 30 (a tu się to zdarza regularnie), chociaż zazwyczaj nie były też dużo wyższe (jak tu - so it's not like shader pefromace here is all that worse compared to GL6). Finalnie - DH i Miniature Shader działały razem, a tu tak nie ma (for the record, to samo się dzieje na prawie surowym SO z DH i tym shaderem, więc to nie jest wina mojej paczki - ig they just don't like each other on Fabric 1.20.1).

To wszystko może brzmieć trochę źle („Shadery robią duży performace hit, większy niż robiły na GL6? Ale ja kocham shadery! Nie chcę, żeby źle działały.”), ale chcę przypomnieć, że o ile performace hit jest duży (ale tak jest zawsze, so it's not my pack's fault), o tyle *relatywnie do GL6* jest *marginalnie* bardziej duży. Ja mam *absolutnego potato PC* (I mean... OK, it's not bad. CPU jest perfekcyjnie adekwatny do współczesnych zadań, a RAMu mam stupidly dużo (20GB). Ale integrated GPU z Ryzena 7 z 2020r. zaczyna zdecydowanie pokazywać swój wiek.), więc oczywiście, że shadery powodują dla mnie dużo większy performance drop, niż dla normalnych ludzi! U mnie było *nieco* gorzej niż na GL6. Na lepszym kompie, to „nieco” pewnie przetłumaczy się na jakieś 5FPS mniej. Barely noticable. Generalnie, zasada jest taka, że „Cokolwiek ja mam dla danego zestawu ustawień graficznych (render distance, paczki tekstur, DH, ustawienia vanilla typu smooth lightning) bez shaderów - to Iwo będzie miał 2x tyle na shaderach (zakładając, że pozostałe ustawienia graficzne są takie same)”. A wydaje mi się, że na **120-160** FPS (lub **60-120** z liśćmi, albo **60-80** z liśćmi i DH) raczej narezkać nie będzie. Ofc, mało kto ma tak dobrego PC jak Iwo. Ale łącznie on i ja reprezentujemy spektrum, w środku którego mieści się większość graczy GhostLanda (tak Tymon, ty też - masz mocniejszego kompa ode mnie, wierz mi lub nie). Skoro ja nie narzekam, a Iwo probably też nie będzie - to dasz sobie radę i ty, człowieku leżący gdzieś między nami na skali hardwareu.

Poza FPS, warto też zwrócić uwagę na bardzo dobry czas startu (zazwyczaj poniżej minuty, okazjonalnie poniżej półtorej - szczególnie przy pierwszym uruchomieniu od włączenia kompa, co ma sens, bo OS jeszcze nie zdążył zapisać plików w cache). Ma też bardzo niskie zużycie RAMu - nie przekroczyło u mnie ani razu 20% (dałem mu ok. 12,5GB - co znaczy, że paczka nie przekracza nawet 3GB i to z dużym zapasem). Tak więc jest jeszcze DUUUŻO miejsca na zapchanie jej pierdylionem modów dodających custom modele/tekstury (ie. like... 99% of all gameplay-features-focused mods), które zawsze zajmują najwięcej RAMu i czasu na starcie. :-P
#### Potato:
* DH off
* Better Leaves off
* Dramatic Skies off
* Shadery off
* Render distance: różne

Przy RD16 FPSy zachowywały tak, jak przy RD10-12 w Balanced Performace (tylko rzadziej zchodziły do 30); przy RD24 wsm też (ale były bliżej dołu przedziału); przy RD12 oscylowały w zakresie **50-70** (not quite the 2x gain I said would happen if we disabled Better Leaves, but still very good); a przy RD10 - **60-80**
#### Balanced - performace:
* DH off
* Better Leaves on
* Dramatic Skies on
* Shadery off
* Render distance: 10 i 12

**30-60** przy i 10, i 12 (a nawet i 8 - patrz: drugi poniżej). Teoretycznie, powinny być możliwe jeszcze większe, bo zużycie GPU nie przekraczało 70%, RAMu 30%, a CPU nie monitorowałem aktywnie, ale z kilku losowych looków tu i tam mogę stwierdzić, że raczej było dość niskie. Musi gdzieś być nieoczywisty bottleneck, I guess. Dla jaj włączyłem 16 chunków i dalej trzymały się tego zakresu. I nie, nie miałem capped FPS (patrz: powyżej).
#### Balanced - visuals:
* DH off (miała być też wersja z ON, ale nie działo z tym shaderem)
* Better Leaves on
* Dramatic Skies on
* Shadery: Miniature Shaders
* Render distance: 10 i 12

**20-30** FPS, a GPU jest pegged na 100%. Yeeee, niestety nawet Miniature Shader to było za dużo dla mojego kartofelka. Jest *playable*, ale *barely playable*. Fajnie tak włączyć i pooglądać świat (and not have it feel like a slideshow, cuz 20-30 is *just enogh* to maintain an illusion of movemoent), ale probably wyłączę shadery, gdy będę starał się być actually produktywny (np. budując fabrykę pod ziemią, gdzie i tak shaderów nie potrzebuję). I to wszystko przy 10 chunkach! Przy RD12 - minimalne wynoszą 15, a to już *jest* kompletne unplayable.
#### Balanced - max. render distance:
* DH: 48 (*to nie max, ale przy 64 zaczynał ostro umierać)
* Better Leaves on
* Dramatic Skies on
* Shadery off
* Render distance: 8

**30-40** FPS, ale gdy zobaczysz za dużo drzew na raz, to spadną do zakresu **20-30** i (nawet, gdy przestaniesz patrzeć na drzewa) będą się w nim trzymały. Dopiero po kilku minuitach wzrosną znów do zakresu **30-40**. Teoretycznie, powinny być możliwe jeszcze większe, bo zużycie GPU nie przekraczało 70%, RAMu 30%, a CPU nie monitorowałem aktywnie, ale z kilku losowych looków tu i tam mogę stwierdzić, że (mimo podkręcenia DH na „I paid for the whole CPU!”) raczej było dość niskie. Musi gdzieś być nieoczywisty bottleneck, I guess. *(Btw, po wyłączeniu DH jedyna zmiana to było to, że top FPS to teraz 60, zamiast 40 i to, że liście już nie lagują po patrzeniu na nie (Może to jednak chodziło o LOD, nie liście? Bo odkryłem to, gdy podleciałem mocno do do góry, więc ig widziałem oba.); lower bound of 30 and that weird bottleneck stayed. To pokazuje, że DH jest bardzo nisko-profilowy (zjadł 1/3 FPS, ale render distance wzrósł aż 6x), jeśli nie patrzysz na za dużo LODs at once (ie. nie lecisz kilkadziesiąt kratek w górę; normalne patrzenie np. na ocean lub wysoką górę w oddali jest fine). It really is good. Damn, I wish it worked with Miniature Shader! Biorąc pod uwagę, że włączać je będę tylko wtedy gdy widzę ładne rzeczy, to dobrze by było mieć możliwość widzenia więcej owych ładnych rzeczy, bez zabijania FPS.)
#### NASA PC
* DH: 64+
* Better Leaves on
* Dramatic Skies off (bo CU ma własny system nieba)
* Shadery: Complementary Unbound
* Render distance: ???

**DNF:** Mój kartofel tego nie uciągnie; ktoś inny musi je sprawdzić. (Z tego samego powodu nie ustawiałem żadnych wartości render distance - niech przyszły tester zadecyduje, ile jest approperiate.)
### ZMIENIONE DEFAULT USTAWIENIA
* Wyłączenie keybinda na fullscreen, pasek szybkiego dostępu creative (nie mówię o F3+F4, tylko swapowaniu hotbara), Narratora (Ave!), Advancementy i znaczą większości modded klawiszy.
* Włączenie/przepisanie kilku klawiszy debuggowania dla modów oraz kamerę filmową na F10.
* Rocket Boost samolotu na >, bo wygląda jak rakieta, a B był zajęty przez Traveler's Backpacks.
* Włączono przybory operatora (dostęp do command blocków, etc. z creative menu).
* Włączono i ustawiono kolejność resourcepacków (poza Dramatic Skies, żeby Iwo nie marudził).
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
* Wyłączono fullscreen (z jakiegoś powodu, gra domyślnie wystartowała za pierwszym razem w tym trybie).
* Zamknięto 1st-launch warning narratora MC, FancyMenu, Observable oraz Controlify.
* Render distance na 12
* Winieta była domyślnie wyłączona, ale to chyba zmienił jakiś mod - bo nie powinna być.
### FINAL NOTES
* Łącznie projektów: 154 modów + 8 shaderów + 8 texturepacków + 1 plik TXT ustawień shaderów (który Modrinth wykrywa jako shader for some reason) = **171** *Pamiętaj: to nie wszystko mody - a z pośród samych modów: niektóre są wyłączone, a inne będą usunięte. Więc ta liczba wygląda strasznie, ale na prawdę nie jest tak źle.*
* W niektórych miejscach napisałem, że trzeba ustawić keybindy. Ale prawie na pewno będzie ich dużo więcej, niż te kilka wymienionych. Obecnie, tylko powyłączałem większość keybindów, tak żeby dało się gry używać bez 300 konfliktów na guzikach. Ale trzeba będzie je jakoś thoughtfully powłączać.
* **CONFIGI! I CAN'T STRESS THIS ENOUGH!** *z naciskiem na często pomijane rzeczy, np. CraftPresence, BetterCompatChecker lub zamknięcie paska FancyMenu*
* Sprawdź [CONTRIBUTING](CONTRIBUTING.md), jeśli chcesz coś zmieniać w tym repo (a mam nadzieję, że chcesz - bo trochę średnio mam ochotę być jedynym robiącym thinning out tej abominacji).
## **>>*CREDITS*<<**
Inside an `.mrpack` uploaded to this repo, sits a JAR downloaded from [this amazing repo](https://github.com/Bliss-tbh/Async-1.20.1/) (seriously, those commit messages are awesome). Said JAR is a 1.20.1 port of Async. I *realllly* wanted to avoid embedding JARs inside the modpack file because this usually means I'm basically robbing the creator of prestige (from download count) and ad revenue, but that couldn't be avoided, as this mod has *never* been published onto any mod repository. I had to grab it directly from GH. ...Which also means that I'm not affecting any download/money numbers (they don't exist yet), so I hope this is fine. License-wise, I'm *pretty sure* it would be fine, as MIT is GPL-compatible (tho I believe GPL-compat *may* work the other way (ie. re-licensing MIT code under GPL (not GPL under MIT, as it would *seem* here), so I'd like to clarify that **I'M NOT trying to relicense that mod under MIT**, but rather it's merely a GPL file (that'll stay GPL, no matter what I do) embedded inside an MIT repo, and if you ever try to use said repo in an MIT-compliant way (but one that'd break the GPL), this file MUST be removed), but I *also* believe that it's possible to do what I did here, ie. for a non-GPL app to embed GPL code (so long as said code isn't modified in any way - which it wasn't, in this case) - eg. various proprietary GTK/Qt-based apps) - but some mod authors often have their own policies for modpack embedding, that extend outside a normal license. I couldn't find any said policies attached to this port of Async (and didn't check the original because - well - they're both *very* different mods, with this one having a lot of code modified, so that old policy shouldn't apply here), so I followed the license instead. If that's a problem, please contact us. I'm sure a solution can be worked out.