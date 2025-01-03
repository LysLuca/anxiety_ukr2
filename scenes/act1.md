# act1

```
SceneSetup.act1();
```

(...300)

n: А ЦЕ - ЇЇ ТРИВОЖНІСТЬ
n: _*ТИ*_ Є ТРИВОЖНІСТЮ

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: О, здоров! Ми знову тут?

`hong({eyes:"0_neutral"})`

n: ТВОЄ ЗАВДАННЯ - ЗАХИЩАТИ ЛЮДИНУ ВІД *НЕБЕЗПЕКИ*!

`bb({eyes:"look", mouth:"small_lock"})`

n: НАСПРАВДІ, ПЕРЕПРОХОДЖЕННЯ ГРИ ЦЕ ПРЯМА *НЕБЕЗПЕКА* ЗАРАЗ

n: ШВИДКО, ПОПЕРЕДЬ ЇХ!
```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Людино! Слухай, ми в небезпеці! Гравець...

[...знову катуватиме нас!](#act1_replay_torture)

[...не знайде іншої кінцівки!](#act1_replay_alternate)

[...отримає лудонаративний дисонанс!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Вони змусять нас згорнутися калачиком і плакати!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Вони змусять нас розтрощити телефон під час панічки!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Вони змусять нас *НЕ* бити господаря вечірки!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Вони змусять нас вдарити Хорошого Не-Поганця господаря вечірки!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Ну, цього разу ми може не стрибнемо з да--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ВОНИ ЗМУСЯТЬ НАС СТРИБУНТИ З ДАХУ.
{{/if}}

`bb({body:"fear"});`

b: ВСІ ЦІ ЖАХЛИВІ РЕЧІ СТАНУТЬСЯ З НАМИ, А ТОДІ МИ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Звісно, історія *загалом* така сама, проте кожна глава має дві можливі кінцівки, і всі відгалуження діало--

`bb({body:"fear"});`

b: Гравець буде розчарований, закрий цю вкладку, видали операційку, а тоді ми--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Лудо-хто?

`bb({eyes:"normal"});`

b: Ця гра про те, що ти можеш *ОБРАТИ* вибудувати здорові взаємини зі своїм страхом,

`bb({eyes:"normal_right"});`

b: Але перегравання дасть той самий результат, а значить, твій *ВИБІР* не має значення,

`bb({eyes:"narrow_eyebrow"});`

b: А отже це суперечить ігровому наративу та механіці,

`bb({eyes:"fear"});`

b: Це розгойдує канву цього вигаданого світу,

`bb({body:"fear"});`

b: А тоді ми--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: ПОМРЕМОООООООООООООООО

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Окей, повернімося до образу.

```
Game.clearText();
```

n4: (ДОЗВОЛЬ _*ТВОЇЙ*_ ТРИВОЖНОСТІ БЛА БЛА БЛА. ОБЕРИ ТЕ, ЩО _*ТВІЙ*_ СТРАХ БЛА БЛА НУ ТИ ВЖЕ ЗНАЄШ)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: О ні, мій вовк повернувся. Чууууууудово.

`hong({eyes:"0_neutral"})`

n: ТВОЄ ЗАВДАННЯ - ЗАХИСТИТИ ЛЮДИНУ ВІД *НЕБЕЗПЕКИ*
`bb({eyes:"look", mouth:"small_lock"})`

n: НАСПРАДІ, ЦЯ КАНАПКА - ЦЕ ПРЯМА *НЕБЕЗПЕКА* ЗАРАЗ

n: ШВИДКО, ПОПЕРЕДЬ ЇХ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Людино! Слухай, ми у небезпеці! І це...

`bb({body:"squeeze"})`

n4: (ДОЗВОЛЬ _*ТВОЇЙ*_ ТРИВОЖНОСТІ ЗІГРАТИ! ОБЕРИ ТЕ, ЩО САМЕ _*ТВІЙ*_ СТРАХ ПІДКАЗУЄ)

(#act1_normal_choice)

# act1_normal_choice

[Ми їмо самі під час обіду! Знову!](#act1a_alone) `bb({body:"squeeze_talk"})`

[М ине продуктивні, поки їмо!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Цей білий хліб шкідливий для нас!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Хіба ти не знаєш, що самотність впливає на передчасну смерть так само як куріння 15-и цигарок на день?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ем, дякую за цікаву інформацію, проте--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Тож, якщо ми не підемо тусуватися з кимось *саме зараз*, ми--

`bb({body:"panic"})`

b: ПОМРЕМОООООООООООООООООООООООООООООООО

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: ВИ ВИКОРИСТАЛИ *СТРАХ ПОКИНУТОСТІ*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Дістань свій ноут і почни працювати негайно!

`hong({eyes:"0_annoyed"})`

h: Ем, мені краще не смітити крихтами над клавіату--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Якщо ми не працюємо на благо суспільства, це значить, що ми - суспільний паразит!

b: Суспільство не терпітиме паразитів і дістане пестицид, а тоді ми...

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ПОМРЕМОООООООООООО

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: ВИ ВИКОРИСТАЛИ *СТРАХ БУТИ ПОГАНОЮ ЛЮДИНОЮ*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Хіба ті дослідження не бу--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Оброблена пшениця підвищить рівень цукру у твоїй крові, тому тобі будуть змушені ампутувати всі кінцівки, а тоді ми--

`bb({body:"panic"})`

b: ПОМРЕМОООООООООООО

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: ВИ ВИКОРИСТАЛИ *СТРАХ ПОСТРАЖДАТИ*

(#act1b)

# act1b

n: ЦЕ ТАК ЕФЕКТИВНО

`bb({mouth:"smile", eyes:"smile"});`

b: Бачиш, людино? Я твій вірний вовк-охоронець!

`bb({body:"pride_talk"});`

b: Довіряй своїм чуттям! Вони ніколи не збрешуть!
`bb({body:"pride"});`

n: ДОВЕДИ РІВЕНЬ ЕНЕРГІЇ ЛЮДИНИ ДО НУЛЯ

n: ЩОБ ЗАХИСТИТИ ЇХ ФІЗИЧНІ + СОЦІАЛЬНІ + ПСИХІЧНІ ПОТРЕБИ ТИ МОЖЕШ ВИКОРИСТАТИ:

n: СТРАХ *ПОСТРАЖДАТИ* #harm#

n: СТРАХ *ПОКИНУТОСТІ* #alone#

n: І СТРАХ *БУТИ ПОГАНОЮ ЛЮДИНОЮ* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (ПОРАДА: ОБИРАЙ ТЕ, ЩО ОСОБИСТО ЗАЧІПАЄ ТВОЇ НАЙГЛИБШІ, НАЙТЕМНІШІ СТРАХИ!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: знаєш, може саме час глянути, що там у телефоні.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ЗАХИСТИ СВОЮ ЛЮДИНУ

n: ВІД СВІТУ. ВІД ІНШИХ ЛЮДЕЙ. ВІД САМИХ СЕБЕ.

n: ХАЙ ЩАСТИТЬ

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ПЕРШИЙ РАУНД: *ДО БОЮ!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Оу. У Фейсбуці пишуть, що цих вихідних буде вечірка.

`bb({eyes:"uncertain"});`

b: Хіба той дивак не влаштовує їх *щотижня*?

`bb({eyes:"uncertain_right"});`

b: Яку внутрішню порожнечу вони намагаються заповнити? Певно, вони глибоко травмовані!

`hong({eyes:"surprise"});`

h: І я отримали запрошення?

`bb({eyes:"fear", mouth:"normal"});`

b: Ну, що ж!

[Погодься, або ми помремо від самотности!](#act1c_loner)

[Відмовся, там стільки наркоти буде!](#act1c_drugs)

[Проігноруй, ми тільки псуємо всім настрій.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: П'ятнидцять цигарок на день, людино! 15!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: А тоді ніхто не прийде на наш похорон, вони викинуть наші останки в океан і нас з'їсть якийсь кит,
{{/if}}

{{if !_.fifteencigs}}
b: і ми станемо КИТОВИМ ГІВНОМ!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Тому ми мусимо піти на ту вечірку!
{{/if}}

{{if _.parasite}}
b: Просто візьми з собою ноут, тож ми можемо працювати і не бути суспільним паразитом.
{{/if}}

{{if _.whitebread}}
b: Принаймні доки вони не подадуть БІЛИЙ ХЛІБ
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ГОСПОДИ. Якщо це змусить тебе заткнутися, добре.

h: Я погоджуся.

{{if _.whalepoop}}
b: Китове гівно, людинко! Китове гівно!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: чи навіть гірше... БІЛИЙ ХЛІБ
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Ми настільки накидаємось мефом і білим хлібом, що вони навіть не зможуть вмістити наше жирне тіло в кремаційну піч!
{{/if}}

{{if !_.whitebread}}
b: Ми передозуємо настільки, що трунар подумає, що наше тіло *уже* забальзамоване!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Крім того, які вечірки?! Ми повинні працювати, інакше станеммо суспільним паразитом! 
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ГОСПОДИ. Якщо це змусить тебе заткнутися, добре.

h: Я відмовлюся.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Все, що ми робимо це ридаємо в кутку про те, що самотність така ж вбивча які 15 цигарок на день.
{{/if}}

{{if _.parasite}}
b: Все, що ми робимо на вечірках, це переживаємо, що могли б бути продуктивними натомість.
{{/if}}

{{if _.whitebread}}
b: Все, що ми робимо, це переживаємо, що нездорова їжа може нас убити!
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: боже, і чого б це.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Тому, якщо ми підемо, то засмутимо їх, але якщо відмовимось від запрошення, то теж засмутимо!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ВСЕ ЩО МИ РОБИМО, ЦЕ ЗАСМУЧУЄМО ВСІХ, ТОМУ МИ ПОВИННІ ЗАСМУТИТИСЬ ТЕЖ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Угх. Якщо це змусить тебе заткнутись, добре.

h: Я проігнорую запрошення.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: І взагалі. Фейсбук це занадто. Мені треба щось спокійніше, менш тривожно-підживлювальне.

`hong({eyes:"neutral"});`

h: Що нового у Твіттері?

`bb({eyes:"look"});`

[О ні, глянь на ці жахливі новини!](#act1d_news)

[О ні, а що як цей твіт насправді *про нас?*](#act1d_subtweet)

[Гей, гіфка котика, що п'є молоко!](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Боже, здається, що світ скоро збожеволіє, чи не так?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Здається, що це кінець, що всі вмирають і ми приречені, і нічого не можемо вже змінити. 

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Давай поширимо!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Окей, я ретвітну, просто сиди тихо!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: До біса, гляну у Снапчат.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Це підтекст! Підступний завуальований твіт!

`hong({eyes:"annoyed"});`

h: А може ні?

`bb({eyes:"narrow", mouth:"small"});`

b: але що як вони говорять за нашою спиною

h: Вони не--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ПЕРЕД НАШОЮ СПИНОЮ

`hong({eyes:"sad", mouth:"sad"});`

h: Я не--

`bb({eyes:"narrow", mouth:"small"});`

b: але *що як*

h: З--

`bb({eyes:"narrow_eyebrow"});`

b: *що як*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: о-КЕЙ, спробую Снапчат.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Хех, миленько, я щойно ретвітнули, дума--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: КОТАМ НЕ МОЖНА МОЛОКА, І МИ ЖАХЛИВІ, БО НАСОЛОДЖУЄМОСЯ СТРАЖДАННЯМИ ТВАРИНИ

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: о-КЕЙ, спробую Снапчат.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Оу, фотки з минулої ночі. То *от*, що це за щотижневі вечірки.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Уух, там надто багато людей для моєї тривожності.

h: Може, мені не варто було погоджуватись прийти?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Змінимо свій вибір? Як боягуз?](#act1e_yes_dontchange)

[Змінімо свій вибір! Там надто багато людей!](#act1e_yes_changetono)

{{if _.subtweet}}
[О так, то був точно підтекст.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Чекай, ми ретвітнули не перевіривши.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ти знали, що у тебе жахлива постава?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Вони розраховували, що ми прийдемо, а тепер ми зраджуємо їх довіру? Хочеш вмерти на самоті?!

{{if _.fifteencigs}}
b: П'ЯТНАДЦЯТЬ. ЦИГАРОК.
{{/if}}

{{if _.whalepoop}}
b: КИТОВЕ. ГІВНО.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись, заткнись, я не відмовлятимусь!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хіба ти не знаєш, яка буває тиснява?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: У 2003 на Род-Айленді у клубі сталася пожежа, і паніка змусила людей створити тисняву біля дверей. 280 людей згоріли заживо-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ХОЧЕШ ЩОБ ЦЕ СТАЛОСЯ І З НАМИ-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: ВІДМОВСЯ ВІДМОВСЯ ВІДМОВСЯ ВІДМОВСЯ ВІДМОВСЯ ВІДМОВСЯ-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнися, заткнися, я відмовлюся. Господи!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Хм... виглядає так весело.

h: Може, мені не варто було відмовлятися?

`bb({mouth:"normal", eyes:"normal"});`

[Змінимо свій вибір? Як боягуз?](#act1e_no_dontchange)

[Змінімо свій вибір! Не вмираймо самі!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Так, то був точно завуальований твіт.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Чекай, ми ретвітнули не перевіривши.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Ти знаєш, що у тебе жахлива постава?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Всі розраховували на нас!

b: ...щоб ми залишили їх у спокої і не руйнували хорошу вечірку таким жахливим, огидним мерзотником як ти--{{if _.whitebread}}який ще й жує хліб!{{/if}}


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись, заткнись, я відмовлюсь!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хронічна самотність підвищує рівень кортизолу, так само як і ризик серцево-судинних захворювань та інфаркту!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: П'ЯТНАДЦЯТЬ. ЦИГАРОК.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Заткнись, заткнись, я погоджусь. Господи!
(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Усі наші проблемні твіти випливли!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Нас звинуватять і закенселять і протягнуть на мотузці кіньми по інформаційній магістралі!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ну чому ти такий?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ми поширюємо дезінформацію! Ми руйнуємо довіру до вільних ЗМІ!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Ми - причина, чому фашизм повстане на руїнах демократії!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Ну чому ти такий?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Хочеш рогалика замість спини? Перестань так сутулитися!

```
bb({body:"meta"});
```

b: Тебе це теж стосується.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ну чому ти такий?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Хм... Виглядає весело.

h: Може, мені не варто було ігнорувати?

`bb({mouth:"normal", eyes:"normal"});`

[Продовжуй ігнорити, ми тільки все псуєм.](#act1e_ignore_continue)

[Насправді, погодься](#act1e_ignore_changetoyes)

[Насправді, відмовся](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Хіба це не буде нечемно, продовжувати ігнорити?

`bb({eyes:"normal_right"});`

b: Ну, інші нас завжди ігнорують, *тож*

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: тому питання закрите.
(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Ти... дозволяєш мені повеселитися?

b: Ну, типу, самотність *може* нас убити.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Надто багато людей. Натовпи небезпечні.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Пофіг. Нове сповіщення в Тіндері.

`bb({eyes:"uncertain"})`

b: Ще що, додаток для знайомств?

`hong({eyes:"annoyed"})`

h: Ні, це не для знайомств. Просто спосіб познайом--

`bb({eyes:"narrow"})`

b: Це додаток для знайомств.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: О, ти глянь. Вони гарненькі.

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Будь ласка, не руйнуй ще й це--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: НЕБЕЗПЕКА НЕБЕЗПЕКА НЕБЕЗПЕКА НЕБЕЗПЕКА

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Люди нас *використовують*.](#act1f_used_by_others)

[Ми людей *використовуємо*.](#act1f_using_others)

[ЦЕ СЕРІЙНИЙ УБИВЦЯ!](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Безладні стосунки можуть заповнити діру всередині,

b: але вони ніколи не заповнять діру...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *ось тут*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Суть в тому, що МИ ПОМРЕМО САМОТНІМИ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Ти думаєш, що чужі статеві органи - то як покемони для нас?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (саундтек до покемонів)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Хочу бути, най^хвойд^ливі-шо-ю-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Як ніхто раніше-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Бедра й ^сідниці^, розкішні ^циці^-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ зі спітнілим ^членом^ і яйцями між ніг!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ ЗБОЧЕН-ЦІ! Я ЇХ ЗБЕР-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Суть в тому, що ми маніпулятивне мудло.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Вони спіймають тебе і примусово нагодують хлібом, щоб ти розжиріли і вони могли носити твою шкіру замість костюма!
{{/if}}

{{if _.parasite}}
b: Вони бичуватимуть тебе помодоро таймером і казатимуть "ТИ ПОВИННІ БУТИ ПРОДУКТИВНІШИМИ, ПАРАЗИТЕ"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Вони зроблять з тебе криваві конфеті, твої нутрощі стануть стрічками, а кров - чашею з пуншем!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Якщо щодо ТАКОГО запрошення?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: я такі замахані від цієї гри.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"loneliness will kill us"... {{/if}}
{{if _.parasite}}"we're a society-parasite"... {{/if}}
{{if _.whitebread}}"don't eat that, it'll kill us"... {{/if}}
{{if _.subtweet}}"they're talking behind our back"... {{/if}}
{{if _.badnews}}"the world is burning"... {{/if}}
{{if _.hookuphole}}"we'll die alone"... {{/if}}
{{if _.serialkiller}}"they're a serial killer"... {{/if}}
{{if _.catmilk}}"cats can't digest milk"... {{/if}}
{{if _.pokemon}}a ^crappy^ parody song... {{/if}}

h: я просто хочу жити своє життя.

h: я просто хочу бути вільними від всього цього... болю.

`bb({eyes:"look_sad"});`

b: Хей... людино...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Все буде гаразд.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Як твій вірний вовк-охоронець, я завжди на сторожі від небезпек і зроблю все, щоб вберегти тебе.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Обіцяю.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Останнє. Інстаграм. Що тут?

`hong({eyes:"sad"});`

h: Тут... більше фоток з вечірки.

`hong({mouth:"sad"});`

h: Всі такі щасоиві. Не турбуються. Не тривожаться.

`hong({mouth:"anger"});`

h: Господи, чому я не можу бути як вони? Чому я не можу бути *нормальними*?

`bb({eyes:"normal_right"});`

b: До речі, про вечірки. Ось моє фінальне рішення:

`bb({eyes:"normal"});`

[Ми мусимо піти.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Ми не йдемо туди.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Ми му--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^БЛЯТЬ^.*

`hong({body:"2_you"});`

h: ТИ.

(...500)

b: щ

(...1500)

`bb({eyes:"wat_2"});`

b: що?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Я збираюсь ПОГОДИТИСЬ на вечірку,

{{if _.act1g=="go"}}
h: НЕ тому що ти так хочеш, а бо *Я* так хочу.
{{/if}}

{{if _.act1g=="dont"}}
h: Точніше, САМЕ ТОМУ, що ти не хочеш.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Ти НЕ контролюєш мене.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Тепеп дай мені поїсти цю канапку у ^йобаній^ тиші.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[ААААА МИ ПОМРЕМО](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[ААААА ВСІ НЕНАВИДЯТЬ НАС](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[ААААА МИ ЖАХЛИВІІІ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА МИ ПОМРЕМО АААААААААААААААА

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА НАС УСІ НЕНАВИДЯТЬ АААААААААААААААА
```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ААААА МИ ЖАХЛИВІІІ АААААААААААААААА

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: ВІТАЮ

(...500)

n: ВИ УСПІШНО ЗАХИСТИЛИ ФІЗИЧНІ + СОЦІАЛЬНІ + ПСИХІЧНІ ПОТРЕБИ ВАШОЇ ЛЮДИНИ

n: ЩО Ж, ГЛЯНЬТЕ, ЯКІ ВОНИ ВДЯЧНІ!

(...500)

n: ОСКІЛЬКИ ЇХ ЕНЕРГІЯ ТЕПЕР НА НУЛІ, ВИ МОЖЕТЕ КОНТРОЛЮВАТИ ДІЇ НАПРЯМУ

`bb({mouth:"smile", eyes:"normal"});`

n: ОБЕРІТЬ ЗАКЛЮЧНУ ДІЮ

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ДОБИВАЙ*

[{БИЙ: Покарай свій тупий телефон!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{ТІКАЙ: Згорнися клубочком і плач!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Твій телефон ледь не спричинив панічну атаку!

`bb({eyes:"anger"})`

b: Цукерберг і ко захоплюють твій розум задля капіталістичного підняття своїх статків!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Покарай свій телефон! Зниш його! Розбий!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО ЗНИЩ ЙОГО--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Весь світ сповнений небезпек!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Будь як броненосець! Скрутись калачиком для самозахисту!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ СКРУТИСЬ І ПЛАЧ-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
