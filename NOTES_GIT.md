<h3 align="center">НОТАТКИ по Git/</h3>
## Operations on Files**************

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git add <filename> | Adds a file to Staging area |          
| $ git add * | Adds all files to Staging area | 
| $ git commit -a | Stages files automatically | ******
| $ git log -p | Produces patch text |***************
| $ git show | Shows various objects |**********
| $ git diff | Can show the differences in various commits |************
| $ git diff --staged | Show all staged files compared to the named commit |
| $ git add -p | Allows a user to interactively review patches to add to the current commit |
| $ git mv | Moves a file |
| $ git rm | Removes a file |
	


 ## Branches*************

| Syntax | Description |                        
| :--- | :--- |                                                                                
| $ git branch | Used to manage branches |       
| $ git branch <name> | Creates the branch | 
| $ git branch -d <name> | Deletes the branch |
| $ git branch -D <name> | Forcibly deletes the branch |
| $ git checkout <branch> | Switches to a branch |
| $ git checkout -b <branch> | Creates a new branch and switches to it |
| $ git merge <branch> | Merge joins branches together |
| $ git merge --abort | abort the merge action (In case of merge conflict) |
| $ git log --graph --oneline | This shows a summarized view of the commit history for a repo |
	

<b>Система контроля версий (от англ. Version Control System, VCS</b>) — это место хранения кода  для разработчиков!

Она заточена именно на разработку продуктов. То есть на хранение кода, синхронизацию работы нескольких человек, создание релизов (бранчей)...

Имеет решающее значение для поддержания здоровой кодовой базы для всех видов ИТ-ресурсов,и для того, чтобы несколько людей сотрудничали в одних и тех же проектах кодирования вместе./
можем использовать инструмент командной строки diff, чтобы взять два файла или даже в каталоги, и показать различия между ними в нескольких форматах. 

Diff является самым популярным , но не единственным доступным. Например, wdiff выделяет слова, которые изменили в файле вместо рабочей строки за строкой, как diff.

Шпаргалка по различиям и исправлениям
разница
diff используется для поиска различий между двумя файлами. Само по себе это немного сложно использовать; вместо этого используйте его с diff -u, чтобы найти строки, которые различаются в двух файлах:

разница -у
diff -u используется для сравнения двух файлов, строка за строкой, и сравнения различных строк в одном и том же выводе
Пластырь
Патч полезен для применения различий между файлами. См. приведенный ниже пример, в котором сравниваются два файла. Сравнение сохраняется в виде файла .diff, который затем исправляется до исходного файла!
В нашем примере возможно, что код , который использовал наш коллега для подготовки исправление, не был последней версией. Используя diff вместо всего файла, мы можем четко видеть, что они изменили, независимо от того, какую версию они использовали. Команда patch может обнаружить, что были внесены изменения в файл и сделает все возможное, чтобы применить diff в любом случае.
мы можем разобрать все структуры каталогов , и в этом случае файл diff может указать, где каждый файл изменений должен быть без необходимости делать любое ручное жонглирование.
#VCS хранит ваш код и конфигурацию. Он также хранит историю этого кода и конфигурации. Система управления версиями может функционировать как машина времени, давая вам представление о решениях прошлого. 

<b>Git</b> — это бесплатная система с открытым исходным кодом, доступная для установки на Unix платформах, Windows и macOS. 
Просмотр истории коммитов  -  для этого является команда git log
Основной инструмент, используемый для определения, какие файлы в каком состоянии находятся — это команда git status.Используйте команду git status, чтобы проверить текущее состояние репозитория.
Для того чтобы начать отслеживать (добавить под версионный контроль) новый файл, используется команда <b></b> git add/ Если вы изменили файл после выполнения git add, вам придётся снова выполнить git add, чтобы проиндексировать последнюю версию файла:
Простейший способ зафиксировать изменения — это набрать git commit




<b>Git commit -a </b> не работает с новыми файлами, потому что они не отслеживаются.Вместо этого git commit -a - это ярлык для выполнениялюбых изменений в отслеживаемых файлах и фиксации их за один шаг.
Если измененный файлникогда не был зафиксирован в репо,нам все равно нужно будет использовать git add, чтобы отслеживать его сначала. Эти ярлыки полезны при внесении небольших изменений, которые мы знаем, что мы хотим, чтобы зафиксировали непосредственно, не сохраняя их в промежуточной области и необходимости писать длинные и сложные описания. Имейте в виду, что когда вы используете ярлык -m, вы можете писать только короткие сообщения и не можете использовать лучшие практики в отношении описаний commit, о которых мы говорили ранее.

Команда <b>git log</b> имеет очень большое количество опций для поиска коммитов по разным критериям. Одним из самых полезных аргументов является -p или --patch, который показывает разницу (выводит патч), внесенную в каждый коммит. Еще одним интересным флагом для git log является флаг —stat. Это приведет к тому, что git log покажет  сокращенную статистику для каждого коммита.опция --stat печатает под каждым из коммитов список и количество измененных файлов, а также сколько строк в каждом из файлов было добавлено и удалено. В конце можно увидеть суммарную таблицу изменений.

git diff сама по себе не показывает все изменения сделанные с последнего коммита — только те, что ещё не проиндексированы.С помощью этой команды мы можем увидеть фактические изменения этапа.

удалить файлы из репозитория с помощью команды git rm, которая остановит отслеживание файла git и удалит его из каталога git./* сначала посмотрите содержимое каталога с помощью ls, затем удалите файл с git rm, затем проверьте содержимое с помощью ls еще раз, и , наконец, проверьте статус с git status.*/

команду git mv может использоваться как для перемещения, так и для переименования файлов в репозитории.

Файлы <b>.gitignore</b> используются, чтобы указать инструменту git намеренно игнорировать некоторые файлы в данном репозитории Git. 
К шаблонам в файле .gitignore применяются следующие правила:

Пустые строки, а также строки, начинающиеся с #, игнорируются.

Стандартные шаблоны являются глобальными и применяются рекурсивно для всего дерева каталогов.

Чтобы избежать рекурсии используйте символ слеш (/) в начале шаблона.

Чтобы исключить каталог добавьте слеш (/) в конец шаблона.

Можно инвертировать шаблон, использовав восклицательный знак (!) в качестве первого символа.

ПАМЯТКА

<b>git checkout</b> эффективно используется для переключения веток.

<b>git reset</b> в основном сбрасывает репо, отбрасывая некоторые изменения. Это несколько сложно понять, поэтому чтение примеров в документации может быть немного полезнее.

В Интернете есть несколько других полезных статей, в которых обсуждаются более агрессивные подходы к сбросу репозитория .

<b>git commit</b> --amend используется для внесения изменений в коммиты постфактум, что может быть полезно для создания заметок о данном коммите.

<b>git revert</b> делает новую фиксацию, которая фактически откатывает предыдущую фиксацию. Это немного похоже на команду отмены.


Слияние
Git использует два разных алгоритма для выполнения слияния,быстрого вперёд и трехстороннего слияния.Слияние, которое мы только что выполнили, является примером быстрого слияния вперед.Этот вид слияния происходит, когда все коммитыв извлеченной ветке также находятся в объединенной ветке.Если это так,мы можем сказать, что история фиксации обеих ветвей не расходятся.В этих случаях все, что нужно сделать Git, это обновить указатели ветвей дотой же фиксации, и фактическое слияние не должно происходить.С другой стороны, трехстороннее слияние выполняется, когда история слиянияветвей в некотором роде расходится, инет хорошего линейного пути, чтобы объединить их с помощью быстрой пересылки.Это происходит, когда фиксация производится на одной веткепосле точки, когда обе ветви разделяются.


