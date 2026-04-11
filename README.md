# 3D-печать в электронике

Этот репозиторий собран как одна последовательная серия про `FDM-принтеры в электронике`:

- где они действительно полезны;
- где они удобны как оснастка для обычной `PCB`;
- где начинаются интересные, но тяжёлые гибридные процессы;
- и где попытка заменить медь печатным пластиком перестаёт быть практичной.

Главная идея серии простая: `3D-печать почти всегда сильнее как механика, оснастка и носитель процесса, чем как замена нормального металлического проводника`.

Вся документация лежит в [`docs/`](docs/), а основной индекс находится здесь:

- [docs/README.md](docs/README.md)

Справочный вход:

- [docs/DIY_PCB_00_glossary_terms_and_procurement.md](docs/DIY_PCB_00_glossary_terms_and_procurement.md) - единая терминология `RU / EN`, поисковые слова и закупка

## Что изменилось в логике серии

Серия теперь чётче делится на три маршрута:

1. `Практичный PCB-маршрут`
   Обычная плата, где принтер помогает как координатная и механическая платформа.
2. `Экспериментальная ветка`
   Фольга, химическая и гальваническая металлизация подложки, conductive plastic как основа под последующее наращивание металла.
3. `Не-PCB ветка`
   3D-подложки, `point-to-point`, `turret`, `eyelet`, `wire-wrap`, где 3D-печать используется прежде всего как механика.

Это важно, потому что `химическая и гальваническая металлизация` теперь встроена не как случайная боковая заметка, а как отдельный гибридный этап между:

- фольгой на подложке;
- и идеей печатать сами проводники из conductive filament.

## Если нужно быстро понять, с чего начинать

Для домашнего `Ender` самый практичный порядок такой:

1. [docs/DIY_PCB_01_overview_and_routes.md](docs/DIY_PCB_01_overview_and_routes.md)
2. [docs/DIY_PCB_02_masks_stencils_and_direct_print.md](docs/DIY_PCB_02_masks_stencils_and_direct_print.md)
3. [docs/DIY_PCB_03_drilling_two_sided_and_ender.md](docs/DIY_PCB_03_drilling_two_sided_and_ender.md)
4. [docs/DIY_PCB_04_etching_chemistry_and_safety.md](docs/DIY_PCB_04_etching_chemistry_and_safety.md)

Если нужен обзор пределов метода и альтернатив:

5. [docs/DIY_PCB_05_foil_and_experimental_methods.md](docs/DIY_PCB_05_foil_and_experimental_methods.md)
6. [docs/DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md](docs/DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md)
7. [docs/DIY_PCB_06_conductive_filament_and_printed_conductors.md](docs/DIY_PCB_06_conductive_filament_and_printed_conductors.md)
8. [docs/DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md](docs/DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md)

## Короткий вывод серии

Если формулировать совсем сжато:

- `обычная PCB + 3D-печатная оснастка` остаётся главным домашним маршрутом;
- `металлизация подложки` реальна, но относится к экспериментально-гибридной ветке;
- `conductive filament` слаб как конечный проводник, но может быть интересен как `starter scaffold` под гальванику;
- для крупной аналоговой, ламповой и силовой электроники 3D-печать чаще сильнее как `механика`, чем как способ делать дорожки.
