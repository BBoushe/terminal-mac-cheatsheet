# Кратенки за терминалот на Mac (основни команди)

## Македонска верзија

Преводот е изработен од [BBoushe](https://github.com/BBoushe)
_Големите букви служат за визуелна репрезентација._  _КАПСЛОК треабa да е изгаснат._

_На некои места во овој документ наизменично се користи терминот датотека и фајл. Правилниот превод е **датодека** меѓутоа во некои ситуации поедноставно и поразбирливо е да се преведе како **фајл**_

------------

### КРАТЕНКИ

| Команда | Опис |
| ----------- | ----------- |
| Ctrl + A   | Оди на почетокот на линијата на која моментално пишуваш. Оваа команда работи и за повеќето полиња за пишување на системско ниво.  Netbeans е еден исклучок. |
| Ctrl + E   | Оди на крајот на линијата на која моментално пишуваш. Оваа команда работи и за повеќето полиња за пишување на системско ниво.  Netbeans е еден исклучок.  |
| Ctrl + L   | Го брише/чисти екранот |
| Cmd + K    | Го брише/чисти екранот (алтернативна верзија) |
| Ctrl + U   | Исечи сѐ наназад до почеток на линијата |
| Ctrl + K   | Исечи сѐ нанапред до крајот на линијата |
| Ctrl + W   | Исечи еден збор наназад до првото празно место |
| Esc + Backspace | Исечи еден збор наназад до првиот знак т.е. првиот знак што не е буква |
| Ctrl + Y   | Додаи/пејстирај тоа што било исечено од последната „исечи“ (cut) команда |
| Ctrl + H   | Исто како `backspace` т.е. избриши буква/знак |
| Ctrl + C   | Уби (прекини го) го процесот што моментално работи.  Исто така бриште/чисти се на моменталната линија |
| Ctrl + D   | Излези од моменталната `shell` околина кога нема процес што работи, или испрати EOF (крај на датотека) до процесот кој моментално работи |
| Ctrl + Z   | Го поместува моменталниот процес во позадина и го става во мирување т.е. го суспендира. Командата `fg` го враќа во фокус  |
| Ctrl + _   | Поништи (undo) ја предходната команда (командата се изведува со комбинација на  `Ctrl + Shift + minus`) |
| Ctrl + T   | Замени им го местото на последните две букви/знака пред курсорот |
| Ctrl + F   | Помести го курсорот една буква/знак нанапред |
| Ctrl + B   | Помести го курсорот една буква/знак наназад |
| Option + →  | Помести го курсорот еден збор нанапред |
| Option + ←  | Помести го курсорот еден збор наназад |
| Esc + T  | Замени им го местото на последните два збора пред курсорот |
| Tab  | Автоматски ги пополнива имињата на датотеки и папки |


### ГЛАВНИ КОМАНДИ

| Команда | Опис |
| ----------- | ----------- |
| cd [папка] | Менување на директориум, на пр. `cd Documents` |
| cd | Почетен директориум |
| cd ~ | Почетен директориум |
| cd /  | Корен на дискот |
| cd -  | Претходен директориум |
| ls | Прикажи ги датотеките во моменталниот директориум |
| ls -l | `ls` со опција за детална листа |
| ls -a | `ls` со опција за прикажување и на скриени датотеки |
| ls -lh| `ls` со опција за прикажување на човечки читливи големини на датотеки |
| ls -R | `ls` со опција за со опција за прикажување на целата содржина на директориумот рекурзивно прикажувајќи ги сите папки и нивните содржини |
| sudo [команда] | Извршување команда со привилегии на суперкорисник (Super User DO) |
| open [фајл] | Го отвара фајлот (како да е двокликнат) |
| top | Прикажува активни процеси. Притиснете `q` за излез |
| nano [фајл] | Отвора фајл со уредникот nano |
| vim [фајл] | Отвора фајл со уредникот vim |
| clear | Го брише/чисти екранот |
| reset | Го ресетира приказот на терминалот |

### ПОВРЗУВАЊЕ КОМАНДИ

| Команда | Опис |
| ----------- | ----------- |
| [команда-А]; [команда-Б] | Извршување команда А, а потоа Б, без оглед на успехот на А |
| [команда-А] && [команда-Б] | Извршување команда Б, ако А е успешна |
| [команда-А] \|\| [команда-Б] | Извршување команда Б, ако А не успее |
| [команда-А] & | Извршување команда А во позадина |

### ПОВРЗУВАЊЕ СО ЦЕВКА (ПАЈП)
<small>Пајпирање или piping е термин во `shell` и `unix` скрипти што претставува процес на извршување на команда, потоа зимање на излезот или резултатот на таа команда и користење како влез на наредната команда во цевката. Овој процес може да се продолжи се додека има команди во цевката.</small>
<br>

| Копче/Команда | Опис |
| ----------- | ----------- |
| [команда-а] \| [команда-б] | Извршување команда А и проследување на резултатот на команда Б, на пр. `ls -l | awk '{print $9}'` |

### КРАТЕНКИ ЗА ИСТОРИЈА НА КОМАНДИ

| Команда | Опис |
| ----------- | ----------- |
| history n | Прикажува историја на внесени команди – додајте број за да ограничите на последни n команди |
| Ctrl + R  | Интерактивно пребарување низ претходно внесени команди |
| ![вредност] | Извршување на последната команда што започнува со ‘вредност’. На пр. `ls -l` па потоа `!l` ја извршува последната команда која почнува на `l` |
| ![вредност]:p | Прикажување во терминалот на последната команда што започнува со ‘вредност’ |
| !! | Извршување на последната внесена команда |
| !!:p | Прикажување во конзолата на последната внесена команда |

### УПРАВУВАЊЕ СО ФАЈЛОВИ

| Команда | Опис |
| ----------- | ----------- |
| touch [фајл] | Креира нов фајл |
| pwd | Целосна патека до работниот директориум |
| . | Тековна папка, на пр. `ls .` |
| \.\. | Родителски/обвивачки директориум, на пр. `ls ..`. Може да го сфатиме и како едно ниво погоре во контектс на моменталниот директориумот |
| ls -l \.\. | Детална листа на родителскиот директориум |
| cd \.\./\.\./ | Преместување две нивоа погоре |
| cat [фајл] | Испринтај содржина на фајл на екран |
| rm [фајл] | Бришење фајл, на пр. `rm data.tmp` |
| rm -i [фајл] | Бришење со потврда |
| rm -r [директориум] | Бришење директориум и содржина т.е. рекурзивно бришење |
| rm -f [фајл] | Присилно бришење без потврда |
| cp [фајл] [новфајл] | Копира фајл во нов фајл |
| cp [фајл] [директориум] | Копира фајл во директориум |
| mv [фајл] [ново име] | Преместување/Преименување, на пр. `mv file1.ad /tmp`. Ако е во рамки на иста папка е преименување ако е во рамку на друга папка е преместување |
| pbcopy < [фајл] | Копирање на содржината на фајлот спремен за залепување/пејстирање т.е. во `clipboard` |
| pbpaste | Залепување/пејстирање на содржината од `clipboard` |
| pbpaste > [фајл] | Залепување на содржината од `clipboard` во фајл, `pbpaste > paste-test.txt` |

### УПРАВУВАЊЕ СО ДИРЕКТОРИУМИ/ПАПКИ

ДИРЕКТОРИУМ = ПАПКА

| Команда | Опис |
| ----------- | ----------- |
| mkdir [папка] | Креира нов директориум |
| mkdir -p [папка]/[папка] | Креира вгнездени директориуми |
| rmdir [папка] | Брише директориум (само празни директориуми) |
| rm -R [папка] | Брише директориум и содржина |
| less [фајл]| Прикажување на содржината на фајлот во делови според големината на екранот |
| [команда] > [фајл] | Испраќа излез во фајл, имајќи предвид дека ќе се препише |
| [команда] >> [фајл] | Додава излез во постоечки фајл |
| [команда] < [фајл] | Наложува командата да ја прочита содржината од фајл. Со други зборови змеи влез на команда од фајл |

### ПРЕБАРУВАЊЕ

| Команда | Опис |
| ----------- | ----------- |
| find [папка] -name [шаблон_за_пребарување] | Пребарување фајлови, на пр. `find /Users -name "file.txt"` |
| grep [шаблон_за_пребарување] [фајл] | Пребарување на сите линии што го содржат шаблонот, на пр. `grep "Tom" file.txt` |
| grep -r [шаблон_за_пребарување] [папка] | Рекурзивно пребарување во сите фајлови во одреден директориум за сите линии што го содржат шаблонот |
| grep -v [шаблон_за_пребарување] [фајл] | Пребарување на сите линии што НЕ го содржат шаблонот |
| grep -i [шаблон_за_пребарување] [фајл] | Пребарување на сите линии што го содржат шаблонот без разлика на големината на буквите |
| mdfind [шаблон_за_пребарување] | Spotlight пребарување на фајлови (име, содржина, други метаподатоци), на пр. `mdfind skateboard` |
| mdfind -onlyin [папка] -name [шаблон] | Spotlight пребарување на фајлови чии имиња одговараат на шаблонот во дадениот директориум |

### ПОМОШ

| Команда | Опис |
| ----------- | ----------- |
| [команда] -h | Прикажува помош за командата, т.е. прикажува упатство за користење на командата |
| [команда] --help | Слично како и опција `-h` |
| info [команда] | Нуди детални информации за командата. Во најновата верзија на `zsh` терминалот не доаѓа инсталирана, треба да се инсталира мануелно |
| man [команда] | Прикажување на упатството за [команда]. Исто како и претходната команда, нуди детално упатство за командата |
| apropos [шаблон_за_пребарување] | Пребарува команди со клучни зборови во описот пр. `apropos details` ќе ги пребара сите команди кои во описот го имаат шаблонот|
| whatis [шаблон_за_пребарување] | Печати опис од еден ред за команди кои во името или нивниот опис го содржат тој шаблон|
