---
title: Шаман Стихии в препатче Shadowlands
layout: page
last_update: 2020-10-22
wow: 9.0.1
toc: true
author: "Amani. Оригинал: Gistwiki"
---

# Вступление

Во время альфа- и бета-тестирования Элем шаман прошел через множество больших изменений, связанных со вводом и удалением Сверкания, но в итоге мы все равно вернулись к Энергии Водоворота. Основа нашей специализации не изменилась – генерируем ресурс с помощью {{ site.data.spells.lb }} и {{ site.data.spells.lvb }} (а также талантами {{ site.data.spells.if }} и {{ site.data.spells.eb }}), и тратим на {{ site.data.spells.es }}. На АОЕ основным генератором становится {{ site.data.spells.cl }}, а спендером – {{ site.data.spells.quake }}.

Главное отличие Элема в препатче от его версии в 8.3 связано с удалением системы оскверненных предметов, они же «корапты». Благодаря тому, что в 8.3 у нас была возможность разогнать наш показатель Критического удара до значений выше 80%, самым популярным и эффективным вариантом сборки был так называемый «мем-билд», который практически полностью исключал {{ site.data.spells.lvb }} из нашей ротации (не считая мгновенных проков {{ site.data.spells.lava_surge }}). Но после выхода препатча это останется в прошлом – Элем, по сути, возвращается к геймплею времен патчей 8.1 и 8.2 (Битва за Дазар’алор и Вечный Дворец). 

Между тем, в препатче будут работать Азеритовые трейты и сущности Сердца Азерот, а отключатся они только на территориях Темных Земель. Они не так сильно меняют наш геймплей как корапты, однако на их выбор повлияет возврат к стандартному билду. 

Еще один важный момент – в препатче не будет поддержки Симкрафта (как и [Raidbots.com](https://www.raidbots.com/simbot), который является его web-оболочкой), так что можно заниматься филкрафтом сколько захочется, никто не осудит =)

# Кратко и быстро

**Основные моменты из статьи:**

* **Симкрафт не работает до релиза.**  
* **Таланты против одной цели**: <a href="https://ru.wowhead.com/spell=333919" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=320125" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=260878" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=16166" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=30884" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=210714" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=191634" target="blank" data-wh-icon-size="small" ></a> [(Ссылка на калькулятор талантов).](https://ru.wowhead.com/talent-calc/shaman/elemental/mT1M)  

* **Таланты на АОЕ**: <a href="https://ru.wowhead.com/spell=333919" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=273221" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=260878" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=16166" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=30884" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=117013" target="blank" data-wh-icon-size="small" ></a><a href="https://ru.wowhead.com/spell=191634" target="blank" data-wh-icon-size="small" ></a> [(Ссылка на калькулятор талантов).](https://ru.wowhead.com/talent-calc/shaman/elemental/mNBM)  
* **Азерит**: 3x {{ site.data.spells.potential }}, 3x {{ site.data.spells.harmony }}  
* **Сущности против одной цели**:   
  * Большой слот: {{ site.data.spells.condensed }}  
  * Малые слоты: {{ site.data.spells.tigel}}, {{ site.data.spells.breath }}, {{ site.data.spells.iris }},  {{ site.data.spells.conflict }}  
* **Сущности на АОЕ**:  
  * Большой слот: {{ site.data.spells.iris }}  
  * Малые слоты: {{ site.data.spells.breath }}, {{ site.data.spells.tigel }}, {{ site.data.spells.iris }}, {{ site.data.spells.conflict }}, {{ site.data.spells.protocol }}  

* **Статы**: Критический удар = Скорость = Универсальность >>> Искусность

<p></p>

{% include button.html name="Weakauras для Элем Шамана в Препатче" link="/ele/weakauras.html" %}  

<p></p>

# Изменения способностей

• {{ site.data.spells.fe }} – пассивный эффект был полностью переработан. Теперь во время действия {{ site.data.spells.fe }}, наш {{ site.data.spells.fs }} наносит периодический урон на 25% чаще. На 58 уровне добавляется новый эффект, {{ site.data.spells.fe2 }}, который увеличивает длительность всех наложенных {{ site.data.spells.fs }} в два раза, то есть до 36 секунд.

За счет ускорения тиков {{ site.data.spells.fs }} будет чаще срабатывать {{ site.data.spells.lava_surge }}, что даст нам больше мгновенных {{ site.data.spells.lvb }}. Максимальную пользу обновленный {{ site.data.spells.fe }} даст в боях с разрозненными целями.

• {{ site.data.spells.fs }} – длительность снижена с **24** сек. до **18** сек. Общий урон способности уменьшен (с 35% + 210% за 24 сек до 19.5% + 104% за 18 сек).  Неприятный нерф длительности, который в Shadowlands частично перекрывается {{ site.data.spells.fe }} за счет {{ site.data.spells.fe2 }}. Но не в препатче, так как мы будем ограничены 50 уровнем.

• {{ site.data.spells.lvb }} – урон повышен на **~50%**.  
Эффект трех азеритовых трейтов {{ site.data.spells.potential }} теперь базово заложен в специализацию, но без бонусных 3% к шансу срабатывания {{ site.data.spells.lava_surge }}. В препатче работает и {{ site.data.spells.potential }}, и базовое увеличение урона {{ site.data.spells.lvb }}, что делает это заклинание еще полезнее.

• {{ site.data.spells.lb }} – урон повышен на **~25%**.  

• {{ site.data.spells.cl }} – урон повышен на **~25%**.  

• {{ site.data.spells.quake }} – урон понижен на **~20%**.  

Все три изменения выше, по сути, это внутренний баланс урона специализации. Как это повлияет на общий урон Элема по сравнению с другими классами нужно будет смотреть уже на релизе Shadowlands.

# Новые способности

• {{ site.data.spells.swg }} – в Легионе у нас забрали эту способность, но дали {{ site.data.spells.gust }}. В BFA у нас забрали {{ site.data.spells.gust }}, но забыли вернуть {{ site.data.spells.swg }}. Сейчас справедливость восстановлена, и мы наконец-то снова можем дамажить во время перебежек. Будет особенно полезно с талантом {{ site.data.spells.asc_ele }}. В сочетании с {{ site.data.spells.if }} Элем становится одним из самых мобильных бойцов дальнего боя.

• {{ site.data.spells.ch }} – стоит чуть дороже чем {{ site.data.spells.hs }}, а также дольше кастуется. Будет полезно в те моменты боя, когда невозможно атаковать, но необходимо переживать урон – в рейде есть несколько боев с подобными фазами. Но в бою мы вряд-ли будем часто использовать это заклинание.

• {{ site.data.spells.hst }} – мгновенно кастуется и имеет сниженный ГКД, как и у всех тотемов (1 сек.). Стоит достаточно мало маны. Этот тотем будет полезен на перебежках, а также в соло контенте.

• {{ site.data.spells.ls }} – этот щит будет полезен на прокачке и в ПВП за счет генерации Энергии Водоворота. Его урон крайне слаб, а срабатывает он только от прямых атак, то есть практически бесполезен в рейде и Мифик+.

• {{ site.data.spells.ftw }} и {{ site.data.spells.primal }} – бесполезные способности для элема. Находятся в книге заклинаний для прокачки до 10 уровня, чтобы показать весь будущий арсенал шамана. Нет никакого смысла выставлять эти способности на панель скиллов.

# Пассивки, которых не будет в препатче

Помимо ковенантов, медиумов и проводников, в Shadowlands по ходу прокачки у нас откроются дополнительные ранги уже имеющихся способностей:  

• {{ site.data.spells.critdamage2 }} – открывается на 52 уровне.  

• {{ site.data.spells.as2 }} – открывается на 54 уровне.  

• {{ site.data.spells.hex2 }} – открывается на 56 уровне.  

• {{ site.data.spells.fe2 }} – открывается на 58 уровне.  

# Изменения талантов

• {{ site.data.spells.discharge }} – крайне слабый талант, если рассматривать его как активную способность с кулдауном в 30 сек. Он поражает всего одну цель и наносит урона меньше, чем пассивное {{ site.data.spells.er }} в этом же тире талантов, а соседство с {{ site.data.spells.eote }} не дает ему никаких шансов.  

• {{ site.data.spells.ecs }} – достаточно интересный талант, который отлично сочетается с {{ site.data.spells.sk }}. Усиливает его потенциал на 50%, как в бою против одной цели, так и на АОЕ. С использованием этого таланта есть небольшие хитрости. Он повторяет использованное после него заклинание спустя одну секунду задержки, но не копирует его баффы. Однако, во время срабатывания повторного заклинания активные на данный момент баффы усиливают дублированный спелл.

Например, если использовать {{ site.data.spells.sk }}, а затем {{ site.data.spells.ecs }} и {{ site.data.spells.lb }}, то поглотится один стак {{ site.data.spells.sk }}, вылетит обычная {{ site.data.spells.lb }} и следом за ней дублированная {{ site.data.spells.lb }}, которая получит усиление за счет оставшегося стака от {{ site.data.spells.sk }}. Однако если использовать {{ site.data.spells.sk }}, потом сразу же {{ site.data.spells.lb }}, и только потом {{ site.data.spells.ecs }}, то дублированная {{ site.data.spells.lb }} будет не усилена баффом от {{ site.data.spells.sk }}.

> **Важно!** На Бете на данный момент есть баг, из-за которого повторная {{ site.data.spells.lb }} от {{ site.data.spells.ecs }} поглощает бафф от {{ site.data.spells.sk }}. Но на ПТР препатча все работает так, как описано выше.

На АОЕ все еще интереснее. Так как дублированное заклинание вылетает не сразу, у нас есть возможность скастовать на одно {{ site.data.spells.quake }} больше при использовании {{ site.data.spells.sk }} и {{ site.data.spells.ecs }}. Порядок действий будет следующим:

1. Кастуем {{ site.data.spells.sk }} и {{ site.data.spells.ecs }}.  
2. Кастуем {{ site.data.spells.cl }}.  
3. Сразу же кастуем {{ site.data.spells.quake }} два раза – задержка перед применением дублированного заклинания позволяет это провернуть, но потребуется немного опыта (и желательно макрос {{ site.data.spells.quake }} по курсору).  
4. Кастуем {{ site.data.spells.cl }} со вторым стаком от {{ site.data.spells.sk }}.  
5. Кастуем третье {{ site.data.spells.quake }}.  

Эта комбинация ощутимо усиливает наш АОЕ бурст раз в минуту, но требует не менее 4 целей для активации.

В итоге приоритет заклинаний для усиления их с помощью таланта {{ site.data.spells.ecs }} выглядит так:

**В бою против одной цели:**
1. {{ site.data.spells.lb }} под баффом от {{ site.data.spells.sk }}
2. {{ site.data.spells.lvb }}

**На АоЕ:**
1. {{ site.data.spells.cl }} под баффом от {{ site.data.spells.sk }}
2. {{ site.data.spells.quake }}

• {{ site.data.spells.eb }} – талант был перенесен из первого тира во второй, и он больше не конкурирует с {{ site.data.spells.eote }}. В Shadowlands урон этого заклинания был повышен (с 63% до 140% от силы заклинаний), а также добавлена генерация Энергии Водоворота – базово 30 ед., и 45 ед. энергии с проком искусности. 

• {{ site.data.spells.if }} – этот талант получил существенное усиление по сравнению с BFA (базовый урон вырос с 55% до 82.5%, а бафф повышен с 200% до 300%), и теперь это наш самый лучший вариант в этом тире для боя против одной цели. Но в Мифик+ этот талант все также неэффективен. Урон {{ site.data.spells.frs }} под усилением от {{ site.data.spells.if }} практически сравнивается с уроном {{ site.data.spells.es }}.

• {{ site.data.spells.asc_ele }} – добавлен новый эффект при активации – обновляет {{ site.data.spells.fs }} на всех целях и использует на них {{ site.data.spells.lvb }}. Будет полезно на клив боях. При активном {{ site.data.spells.fe }} длительность {{ site.data.spells.fs }} при активации {{ site.data.spells.asc_ele }} увеличивается до 36 сек. {{ site.data.spells.lvb }} при активации дает Энергию Водоворота.

В теории этот талант может быть лучше чем {{ site.data.spells.sk }}, особенно в препатче, но его эффективность зависит от времени боя. Плюс он все также бесполезен на АОЕ, так как {{ site.data.spells.lava_beam }} мало чем отличается от {{ site.data.spells.cl }}.

# Ограничение количества целей на АОЕ 

Одно из важных изменений для многих спеков практически не затронуло геймплей Элем шамана, хотя мы и получили нерф {{ site.data.spells.storm }}. Вот полный список ограничений количества целей для АОЕ заклинаний:

* {{ site.data.spells.quake }} и {{ site.data.spells.lmt }} – софт-кап на 20 целей.  
* {{ site.data.spells.meteor }} – 8 целей.  
* {{ site.data.spells.eye_storm }} – 6 целей.  
* {{ site.data.spells.cl }} и {{ site.data.spells.lava_beam }} – 5 целей (без изменений).  

Самый заметный нерф это ограничение {{ site.data.spells.eye_storm }} шестью целями. Его можно будет заметить в Мифик+, а также в Ни’алоте на Вексионе, Коллективном разуме и Панцире Н’Зота. Подробнее про ограничение количества целей на АоЕ [в этой статье](https://stormkeeper.ru/info/target_cap.html).

# Удаление ГКД со способностей

В Shadowlands многим заклинаниям других классов убрали ГКД, которое было добавлено в начале BFA. Но у шамана единственная способность, на которую повлияло это изменение – талант пятого тира {{ site.data.spells.ag }}. Он все еще достаточно слаб в бою против одной цели, но может быть полезен в Мифик+ во время бурстового АОЕ (особенно в сочетании с {{ site.data.spells.sk }} и {{ site.data.spells.ecs }}). По крайней мере теперь использование этого таланта больше не приводит к потере урона, что очень приятно.

# Потеря эффектов осквернения

Потеря кораптов это одно из самых больших изменений для Элема при переходе с патча 8.3 на 9.0. «Мем-билд» отправляется на отдых на ближайшие пару лет, а мы возвращаемся к стандартному билду через {{ site.data.spells.potential }}. В результате мы станем более мобильны (за счет {{ site.data.spells.if }} и {{ site.data.spells.swg }}) и не так зависимы от бурста, а также гораздо сильнее на кливе разрозенных целей. Но для тех кто начал играть в середине патча 8.3 этот переход может быть болезненным =)

# Таланты

> Помните, что в отсутствие Симкрафта на Бете все расчеты проводились вручную и могут быть не полностью точны.

**Таланты против одной цели, вариант первый:** 

{% include ele_talents.html active="2201032" %}

**Таланты против одной цели, вариант второй:** 

{% include ele_talents.html active="2301033" %}

Первый вариант через {{ site.data.spells.ecs }} и {{ site.data.spells.sk }} позволяет нам достаточно сильно бурстить в одну цель раз в минуту, а второй вариант через {{ site.data.spells.eb }} и {{ site.data.spells.asc_ele }} дает ощутимый бурст раз в 3 минуты (который отлично сочетается с азеритовыми трейтами {{ site.data.spells.potential }}). Но вариант через {{ site.data.spells.asc_ele }} зависит от времени боя, то есть на 3:30 он может быть сильнее билда через {{ site.data.spells.sk }}, а на 5:50 уже слабее.  

Талант {{ site.data.spells.eb }} может браться и без {{ site.data.spells.asc_ele }}, но по грубым тестам он показывает результат хуже, чем {{ site.data.spells.ecs }} в сочетании с талантом {{ site.data.spells.sk }}. Но на препатче это не так важно, и ничто не помешает вам его использовать.

**Таланты на АОЕ:**

{% include ele_talents.html active="2101022" %}

Данный набор талантов в препатче показывает наилучший результат. Альтернативный вариант через {{ site.data.spells.ecs }} и {{ site.data.spells.sk }} позволяет достаточно сильно бурстить раз в минуту. Однако, талант {{ site.data.spells.afs }} в целом дает больше кастов {{ site.data.spells.quake }}.

# Ротация

В бою против одной цели все осталось без изменений. Не уходим в оверкап Энергии Водоворота, тратя её на {{ site.data.spells.es }}, поддерживаем {{ site.data.spells.fs }}, а все остальные заклинания отдаем по кулдауну. Если нечего больше кастовать – {{ site.data.spells.lb }}.

На АОЕ все немного интереснее. В связи с увеличением базового урона {{ site.data.spells.lvb }} и наличия Азеритового трейта {{ site.data.spells.potential }}, мы станем использовать {{ site.data.spells.lvb }} на АОЕ гораздо активнее.
Кастуем его без прока в бою против 1-4 целей, и на 5 целей по проку {{ site.data.spells.lava_surge }} (при взятом таланте {{ site.data.spells.mote }}) или при передвижении. Но сокращение длительности {{ site.data.spells.fs }} не позволит поддерживать его более чем на 3 целях.

## Открывающая ротация

В бою против одной цели, при игре в основном билде через {{ site.data.spells.ecs }} и {{ site.data.spells.sk }}, опенер будет выглядеть следующим образом:

1. {{ site.data.spells.sk }} 
2. {{ site.data.spells.lvb }} 
3. {{ site.data.spells.fs }} 
4. {{ site.data.spells.fe }} 
5. {{ site.data.spells.ecs }} 
6. {{ site.data.spells.lb }} 
7. {{ site.data.spells.if }} 
8. {{ site.data.spells.lvb }} 
9. {{ site.data.spells.lb }} 
10. Дальше согласно приоритетам.

# Характеристики

В препатче приоритет характеристик вернулся к тому же значению, которое было до ввода кораптов:

1. **Критический удар = Скорость = Универсальность**.  
2. **Искусность.**  

Искусность все также наша самая слабая характеристика и Shadowlands не принес никаких изменений в этом плане. Даже возвращение масштабирования вторичных характеристик (т.н. «Diminishing Returns») вряд-ли повлияет на это.

# Азеритовые трейты

Лучшими азеритовыми трейтами снова стали {{ site.data.spells.potential }}, {{ site.data.spells.harmony }} и {{ site.data.spells.lava_shock }}, как и во времена патчей 8.1 и 8.2. {{ site.data.spells.darkness }} хоть и работает в препатче, но в целом оно хуже чем {{ site.data.spells.harmony }}, поэтому из двух этих трейтов мы берем именно гармонию.

# Сущности Сердца Азерот

* **Сущности против одной цели:**   

  * Большой слот: {{ site.data.spells.condensed }}  
  * Малые слоты: {{ site.data.spells.tigel }}, {{ site.data.spells.breath }}, {{ site.data.spells.iris }}, {{ site.data.spells.conflict }}. 

* **Сущности на АОЕ:**  

  * Большой слот: {{ site.data.spells.bote }} (если через {{ site.data.spells.storm }}) или {{ site.data.spells.iris }}.  
  * Малые слоты: {{ site.data.spells.tigel }}, {{ site.data.spells.breath }}, {{ site.data.spells.iris }}, {{ site.data.spells.protocol }}, {{ site.data.spells.conflict }}  

# Итоги

В целом Элем шаман в препатче в достаточно хорошем положении. У нас будет приятный  урон на кливе разрозненных целей и при передвижении, но многим игрокам придется привыкать играть в стандартном билде, после полугода спама {{ site.data.spells.lb }} в мем-билде.
