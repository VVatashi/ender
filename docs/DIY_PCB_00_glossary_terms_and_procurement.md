# 3D-печать в электронике 00: единая терминология, поисковые слова и закупка

## Зачем нужен этот файл

Этот файл задаёт `единый словарь` для всей серии и собирает в одном месте:

- рекомендуемые русские и английские термины;
- поисковые формулировки для даташитов, форумов и маркетплейсов;
- примеры ссылок на материалы и компоненты, которые можно искать на российских и международных площадках.

Во всей серии удобно придерживаться такого правила:

- основной термин в тексте давать по-русски;
- при первом важном упоминании рядом давать английский эквивалент в скобках;
- для поиска на маркетплейсах использовать и русский, и английский варианты.

Практически этим файлом лучше пользоваться так:

1. читать основную главу серии;
2. если термин звучит знакомо, но не до конца ясно, сверяться с таблицей ниже;
3. если нужен зарубежный источник, брать английский термин;
4. если нужен локальный поиск по площадкам, брать русский термин и связанный поисковый запрос.

## Важная оговорка по ссылкам

Часть российских площадок (`Ozon`, `Wildberries`, `Chip-Dip`) активно используют `JavaScript` и антибот-защиту. Поэтому ниже ссылки часто даны не как "вечные карточки товара", а как:

- `поисковые ссылки`;
- `ссылки на категории`;
- либо как устойчивые точки входа, которые обычно удобнее конкретного одноразового лота.

Для `AliExpress` удалось дополнительно привязать часть ссылок к живым поисковым страницам и нескольким конкретным лотам.

## Единая терминология серии

| Русский термин | English term | Как понимать в серии | Что вводить в поиск |
| --- | --- | --- | --- |
| печатная плата | printed circuit board, `PCB` | обычная плата с медными дорожками | `PCB`, `printed circuit board`, `печатная плата` |
| медный ламинат, фольгированный стеклотекстолит | copper-clad laminate, copper-clad board | заготовка `FR4` или `FR1` с медной фольгой | `fr4 copper clad laminate`, `фольгированный стеклотекстолит` |
| травильная маска | etch resist | любой слой, который защищает медь при травлении | `etch resist`, `pcb resist ink`, `травильная маска` |
| фотошаблон | photomask, artwork | прозрачная маска для экспонирования фоторезиста | `pcb photomask`, `uv artwork`, `фотошаблон для печатных плат` |
| сухой фоторезист | dry film photoresist, `DFR` | рулонная сухая светочувствительная плёнка для плат | `dry film photoresist pcb`, `сухой фоторезист` |
| жидкий фоторезист | liquid photoresist | жидкая светочувствительная маска для платы | `liquid photoresist pcb`, `жидкий фоторезист` |
| химическая металлизация меди | electroless copper plating | химическое осаждение тонкого медного seed-слоя без внешнего тока | `electroless copper plating pcb`, `химическая металлизация меди` |
| гальваническое наращивание меди | electroplating, electrolytic copper plating | утолщение уже проводящего медного слоя с помощью тока | `electroplating copper pcb`, `electrolytic copper plating pcb` |
| металлизация отверстий | plated through hole, `PTH` | проводящий слой на стенках отверстий двусторонней или многослойной платы | `plated through hole pcb`, `PTH pcb`, `металлизация отверстий` |
| затравочный слой | seed layer | первый тонкий проводящий слой перед гальваническим утолщением | `seed layer electroless copper`, `затравочный слой металлизация` |
| сверловка | `Excellon`, `NC Drill` | файл координат и диаметров отверстий | `Excellon drill`, `NC Drill`, `сверловка Excellon` |
| регистрационные отверстия | tooling holes, registration holes | базовые отверстия для совмещения сторон и шаблонов | `tooling holes pcb`, `registration holes pcb`, `регистрационные отверстия` |
| сквозной монтаж | through-hole, `THT` | монтаж выводных компонентов | `through-hole`, `THT` |
| поверхностный монтаж | surface mount, `SMD/SMT` | монтаж без длинных выводов | `SMD`, `SMT`, `surface mount` |
| макетная плата | perfboard, protoboard | перфорированная плата для ручного монтажа | `perfboard`, `protoboard`, `макетная плата` |
| монтаж навесом | point-to-point wiring | соединение напрямую проводами и выводами | `point-to-point wiring`, `point-to-point construction` |
| монтаж навивкой | wire-wrap | соединение проводом, намотанным на квадратный штырь | `wire-wrap`, `wire wrapping tool`, `монтаж навивкой` |
| турретная стойка | turret terminal, turret lug | металлическая стойка для ручного монтажа | `turret terminal`, `turret board terminal`, `турретная стойка` |
| люверс | eyelet terminal, eyelet | металлический глазок для платы или монтажной планки | `eyelet terminal`, `pcb eyelet`, `люверс для платы` |
| клеммная колодка | terminal block, barrier strip | винтовая или барьерная колодка для соединений | `terminal block`, `barrier strip`, `клеммник` |
| медная лента | copper foil tape, copper tape | клейкая медная лента или фольга | `copper foil tape`, `conductive copper tape`, `медная лента` |
| проводящий филамент, проводящий пластик | conductive filament, conductive PLA | филамент с углеродным наполнителем | `conductive pla filament`, `conductive filament`, `проводящий PLA` |
| conductive plastic как основа под гальванику | conductive substrate for plating, selective electroplating on conductive traces | проводящий полимер не как финальный проводник, а как стартовый путь для селективного наращивания металла | `conductive substrate for electroplating`, `selective electroplating conductive traces`, `electroplating conductive filament` |
| закладная латунная втулка | brass insert, heat-set insert | латунная вставка в пластик для механики и иногда контактов | `heat-set insert`, `brass insert`, `латунная втулка` |
| персульфат натрия | sodium persulfate | один из самых удобных бытовых травителей | `sodium persulfate pcb`, `персульфат натрия` |
| хлорное железо | ferric chloride, `FeCl3` | классический травитель, но очень грязный в быту | `ferric chloride pcb`, `хлорное железо` |

## Термины, которые лучше больше не путать

- `травильная маска (etch resist)` не равна `паяльной маске (solder mask)`.
- `фотошаблон (photomask)` не равен `трафарету для паяльной пасты (solder paste stencil)`.
- `макетная плата (perfboard)` не равна `печатной плате (PCB)`.
- `проводящий пластик (conductive filament)` не равен `металлизации` и не равен `медной дорожке`.
- `химическая металлизация (electroless plating)` не равна `гальванике (electroplating)`: первая создаёт стартовый проводящий слой, вторая его утолщает.
- `3D-подложка` в этой серии означает именно `механическую основу`, а не автоматически готовую электрическую плату.

## Иллюстративные примеры

Ниже не "идеальные товары", а просто наглядные примеры того, как обычно выглядят типовые позиции.

### Проводящий PLA-филамент

![Проводящий PLA-филамент: пример карточки товара](https://ae01.alicdn.com/kf/S877132b3e4944856bdc8313d9d855ebeG.jpg)

Пример карточки: `AliExpress`

- `https://aliexpress.ru/item/1005006688614635.html`

### Типичный расходник для 3D-печати и электроники на маркетплейсе

![Типичный товар из ветки DIY-электроники на AliExpress](https://ae01.alicdn.com/kf/Sdbff8335d756475b89466e21cede161fC.jpg)

Эту картинку лучше воспринимать как иллюстрацию формата лота, а не как рекомендацию без проверки.

## Что и где искать

Эта часть не заменяет полноценный подбор поставщика, но помогает быстро стартовать:

- понять, какие типы товаров вообще существуют;
- как именно они обычно называются на российских и зарубежных площадках;
- и какие категории имеет смысл проверять в первую очередь.

### 1. Практичный PCB-маршрут

| Что нужно | Русский / English | Российские площадки | Международные площадки |
| --- | --- | --- | --- |
| заготовка платы | фольгированный стеклотекстолит / copper-clad laminate | `Ozon`: `https://www.ozon.ru/search/?text=%D1%84%D0%BE%D0%BB%D1%8C%D0%B3%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D1%8B%D0%B9%20%D1%81%D1%82%D0%B5%D0%BA%D0%BB%D0%BE%D1%82%D0%B5%D0%BA%D1%81%D1%82%D0%BE%D0%BB%D0%B8%D1%82` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=fr4%20copper%20clad%20laminate%20board` |
| сухой фоторезист | сухой фоторезист / dry film photoresist | `Ozon`: `https://www.ozon.ru/category/fotorezist-dlya-pechatnyh-plat/` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=dry%20film%20photoresist%20pcb` |
| травитель | персульфат натрия / sodium persulfate | `Chip-Dip`: `https://www.chipdip.ru/catalog/popular/persulfat` ; `Ozon`: `https://www.ozon.ru/search/?text=%D0%BF%D0%B5%D1%80%D1%81%D1%83%D0%BB%D1%8C%D1%84%D0%B0%D1%82%20%D0%BD%D0%B0%D1%82%D1%80%D0%B8%D1%8F` | `AliExpress`: искать имеет смысл только как запасной вариант, обычно выгоднее локально |
| свёрла для PCB | свёрла для печатных плат / PCB drill bits, tungsten carbide micro drills | `Chip-Dip`: `https://www.chipdip.ru/search?searchtext=%D1%81%D0%B2%D0%B5%D1%80%D0%BB%D0%BE%20%D0%B4%D0%BB%D1%8F%20%D0%BF%D0%B5%D1%87%D0%B0%D1%82%D0%BD%D1%8B%D1%85%20%D0%BF%D0%BB%D0%B0%D1%82` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=pcb%20drill%20bits%20tungsten%20carbide` |
| UV-источник | УФ-лампа / UV nail lamp, UV exposure lamp | `Ozon`: `https://www.ozon.ru/search/?text=uv%20%D0%BB%D0%B0%D0%BC%D0%BF%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%BD%D0%BE%D0%B3%D1%82%D0%B5%D0%B9` ; `WB`: `https://www.wildberries.ru/catalog/0/search.aspx?search=uv%20%D0%BB%D0%B0%D0%BC%D0%BF%D0%B0%20%D0%B4%D0%BB%D1%8F%20%D0%BD%D0%BE%D0%B3%D1%82%D0%B5%D0%B9` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=uv%20nail%20lamp` |

### 2. Экспериментальная ветка

| Что нужно | Русский / English | Российские площадки | Международные площадки |
| --- | --- | --- | --- |
| медная лента | медная лента / copper foil tape | `Ozon`: `https://www.ozon.ru/search/?text=%D0%BC%D0%B5%D0%B4%D0%BD%D0%B0%D1%8F%20%D0%BB%D0%B5%D0%BD%D1%82%D0%B0` ; `WB`: `https://www.wildberries.ru/catalog/0/search.aspx?search=%D0%BC%D0%B5%D0%B4%D0%BD%D0%B0%D1%8F%20%D0%BB%D0%B5%D0%BD%D1%82%D0%B0` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=copper%20foil%20tape%20conductive%20adhesive` |
| наборы для химической металлизации | electroless copper kit, PTH kit | локально встречаются нерегулярно, чаще проще искать по англоязычным названиям | `Google`: `electroless copper kit pcb`, `plated through hole kit pcb`, `Nano3D electroless copper kit`, `MG Chemicals 41600A` |
| проводящий филамент | проводящий PLA / conductive PLA filament | `Ozon`: `https://www.ozon.ru/search/?text=%D0%BF%D1%80%D0%BE%D0%B2%D0%BE%D0%B4%D1%8F%D1%89%D0%B8%D0%B9%20PLA` ; `WB`: `https://www.wildberries.ru/catalog/0/search.aspx?search=%D0%BF%D1%80%D0%BE%D0%B2%D0%BE%D0%B4%D1%8F%D1%89%D0%B8%D0%B9%20pla` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=conductive%20pla%20filament` |
| конкретный пример conductive PLA | conductive PLA filament | локальные площадки удобнее смотреть поиском | пример лота: `https://aliexpress.ru/item/1005006688614635.html` ; альтернативный лот: `https://aliexpress.ru/item/1005008837855530.html` |

### 3. Не-PCB ветка

| Что нужно | Русский / English | Российские площадки | Международные площадки |
| --- | --- | --- | --- |
| макетная плата | макетная плата / perfboard, protoboard | `Ozon`: `https://www.ozon.ru/search/?text=%D0%BC%D0%B0%D0%BA%D0%B5%D1%82%D0%BD%D0%B0%D1%8F%20%D0%BF%D0%BB%D0%B0%D1%82%D0%B0` ; `Chip-Dip`: `https://www.chipdip.ru/search?searchtext=%D0%BC%D0%B0%D0%BA%D0%B5%D1%82%D0%BD%D0%B0%D1%8F%20%D0%BF%D0%BB%D0%B0%D1%82%D0%B0` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=perfboard%20protoboard` |
| клеммники | клеммник / terminal block, barrier strip | `Chip-Dip`: `https://www.chipdip.ru/search?searchtext=%D0%BA%D0%BB%D0%B5%D0%BC%D0%BC%D0%BD%D0%B8%D0%BA` ; `Ozon`: `https://www.ozon.ru/search/?text=%D0%BA%D0%BB%D0%B5%D0%BC%D0%BC%D0%BD%D0%B8%D0%BA` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=terminal%20block%20barrier%20strip` |
| инструмент и провод для навивки | монтаж навивкой / wire-wrap tool, wire-wrap wire | локально встречается нерегулярно, проще искать по словам `wire-wrap` и `навивка` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=wire%20wrap%20tool` |
| турреты | турретная стойка / turret terminal | на локальных площадках встречается редко, часто проще искать по словам `turret terminal` | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=turret%20terminal%20board` |
| люверсы | люверс для платы / eyelet terminal | локально часто продаются как крепёж, а не как радиоэлектронный компонент | `AliExpress`: `https://www.aliexpress.ru/wholesale?SearchText=eyelet%20terminal%20board` |

## Практические замечания по закупке

- Для `химии` и расходников вроде `персульфата натрия` локальные поставщики обычно удобнее по срокам и предсказуемости.
- Для `PCB-свёрл`, `сухого фоторезиста`, `медной ленты` и особенно `turret / eyelet / wire-wrap` выбор на `AliExpress` обычно шире.
- Для `conductive PLA` особенно важно читать не только карточку товара, но и `datasheet`, потому что надпись "проводящий" почти ничего не гарантирует.
- Для `FR4`, `медной ленты` и `макетных плат` российские маркетплейсы полезны как быстрый старт, но наименование товара там часто слишком размыто, поэтому английские поисковые слова всё равно нужны.

## Как это использовать дальше

При чтении остальных файлов серии удобно делать так:

1. читать русское объяснение в основном документе;
2. брать английский термин из этого глоссария;
3. искать по английскому названию `datasheet`, `forum`, `application note` и зарубежные лоты;
4. искать по русскому названию на `Ozon`, `WB` и `Chip-Dip`.

В логике всей серии этот файл лучше воспринимать как `приложение`, к которому удобно возвращаться, а не как главу, которую нужно учить отдельно.
