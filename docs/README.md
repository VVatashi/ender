# 3D-печать в электронике

Это основной `index` всей серии.

Папка собрана не как россыпь заметок, а как одна инженерная линия про то, `как использовать 3D-печать в электронике без романтизации и без лишнего самообмана`.

Серия отвечает на три разных вопроса:

1. как применять `FDM-принтер` в обычном домашнем PCB-процессе;
2. где начинаются экспериментальные гибриды вроде фольги, химической металлизации и conductive plastic под гальванику;
3. где правильнее вообще отказаться от идеи "печатать дорожки" и использовать 3D-печать как механику.

## Главная мысль серии

Если сжать всю подборку до нескольких тезисов, получится так:

- 3D-печать сильна как `механика`, `оснастка` и `позиционирование`;
- для домашней электроники наиболее практичен маршрут `обычная PCB + 3D-печатные приспособления`;
- химическая и гальваническая металлизация подложки реальна, но относится к `экспериментально-гибридной` ветке;
- conductive filament почти всегда слаб как финальная дорожка, но может быть интересен как `стартовая проводящая геометрия` под последующее наращивание металла;
- в крупной аналоговой, ламповой и силовой технике 3D-печать часто полезнее как `носитель монтажа`, а не как замена меди.

## Как читать эту папку

Есть три нормальных маршрута входа.

### 1. Нужен самый практичный путь

Если цель - домашние платы под `Ender` без лишней экзотики, читайте так:

1. [DIY_PCB_01_overview_and_routes.md](./DIY_PCB_01_overview_and_routes.md)
   Общая карта методов и главный выбор всей серии.
2. [DIY_PCB_02_masks_stencils_and_direct_print.md](./DIY_PCB_02_masks_stencils_and_direct_print.md)
   Маски, трафареты, прямое нанесение по меди.
3. [DIY_PCB_03_drilling_two_sided_and_ender.md](./DIY_PCB_03_drilling_two_sided_and_ender.md)
   Сверление, регистрация, двусторонние платы.
4. [DIY_PCB_04_etching_chemistry_and_safety.md](./DIY_PCB_04_etching_chemistry_and_safety.md)
   Травление, чистота процесса, бытовая безопасность.

### 2. Нужны пределы метода и экспериментальная ветка

Если хочется понять, что находится за пределами обычной платы:

5. [DIY_PCB_05_foil_and_experimental_methods.md](./DIY_PCB_05_foil_and_experimental_methods.md)
   Фольга на 3D-подложке и первые безтравильные обходные пути.
6. [DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md](./DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md)
   Химическая и гальваническая металлизация подложки, включая гибридный сценарий `conductive plastic -> металл`.
7. [DIY_PCB_06_conductive_filament_and_printed_conductors.md](./DIY_PCB_06_conductive_filament_and_printed_conductors.md)
   Проводящий пластик и печатные проводники. Здесь разбирается, почему conductive filament слаб как замена меди, но может быть полезен как `starter scaffold` под гальванику.

### 3. Нужен зрелый не-PCB вывод

Если задача ближе к крупной сборке, механике и ручному монтажу:

8. [DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md](./DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md)
   3D-подложка без дорожек, `point-to-point`, `turret`, `eyelet`, `wire-wrap`.

Это не "запасная" глава, а одна из самых сильных конечных точек всей серии.

## Структура серии

### 0. Справочная база

0. [DIY_PCB_00_glossary_terms_and_procurement.md](./DIY_PCB_00_glossary_terms_and_procurement.md)
   Единая терминология `RU / EN`, поисковые слова и закупка. Этот файл удобно держать открытым рядом с основной главой.

### 1. Практичный PCB-маршрут

1. [DIY_PCB_01_overview_and_routes.md](./DIY_PCB_01_overview_and_routes.md)
2. [DIY_PCB_02_masks_stencils_and_direct_print.md](./DIY_PCB_02_masks_stencils_and_direct_print.md)
3. [DIY_PCB_03_drilling_two_sided_and_ender.md](./DIY_PCB_03_drilling_two_sided_and_ender.md)
4. [DIY_PCB_04_etching_chemistry_and_safety.md](./DIY_PCB_04_etching_chemistry_and_safety.md)

### 2. Экспериментально-гибридная ветка

5. [DIY_PCB_05_foil_and_experimental_methods.md](./DIY_PCB_05_foil_and_experimental_methods.md)
6. [DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md](./DIY_PCB_05A_chemical_and_galvanic_metallization_of_substrates.md)
7. [DIY_PCB_06_conductive_filament_and_printed_conductors.md](./DIY_PCB_06_conductive_filament_and_printed_conductors.md)

Внутренняя логика здесь теперь такая:

- `фольга` - самый простой обходной путь;
- `металлизация подложки` - более технологичный, но химически тяжёлый гибрид;
- `conductive filament` - слабый конечный проводник, но иногда полезная стартовая геометрия под металл.

### 3. Не-PCB ветка

8. [DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md](./DIY_PCB_07_3d_substrate_point_to_point_and_wire_wrap.md)

## Если нужен один короткий вывод

Для домашнего `Ender` здравый приоритет обычно такой:

1. сначала выжать максимум из `обычной PCB` и 3D-печатной оснастки;
2. потом смотреть на фольгу и металлизацию только если есть ясная причина;
3. conductive filament рассматривать не как "напечатанную медь", а как очень ограниченный специальный материал;
4. для крупных и горячих устройств всерьёз держать в голове `3D-механику + металлический монтаж`.
