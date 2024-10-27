1.	Создать новый Remote Repository (удаленный репозиторий) на GitHub. Указать описание репозитория. Произвести клонирование репозитория на локальную машину в Local Repository и создать LocalWorkingDirectory.
2.	В папке LocalWorkingDirectory (назвать «person1») создать приложение с 3-мя файлами на любом языке программирования (возможно работа с текстовыми файлами). Добавить Commit (коммит) в Local Repository (локальный репозиторий), перенести Commit в Remote Repository. 
3.	Произвести клонирование Remote Repository еще в одну LocalWorkingDirectory (назвать «person2»). В текущей LocalWorkingDirectory добавить в один из файлов новую информацию, добавить Commit в Local Repository. Проверить изменения в LocalWorkingDirectory «person1». Загрузить изменения из LocalWorkingDirectory «person2» в Remote Repository, скачать изменения в LocalWorkingDirectory «person1», проверить изменения в LocalWorkingDirectory «person1». Добавить изменения в другой файл, создать новый Commit, и повторить работу с Remote Repository.
4.	Создание новых веток. Для разработки новой функциональности необходимо создать новую ветку в Local Repository «person1» с названием «dev». Переключиться на нее. Создать новый файл в LocalWorkingDirectory «person1» в новой ветке. Сделать новый Commit в ветке и провести обновление в Remote Repository. В LocalWorkingDirectory «person2» получить последние обновления из Remote Repository, создать новую ветку «dev2» в которой создать новый файл и выполнить Commit и загрузить его в Remote Repository. Сделать небольшие изменения в новом файле и добавить эти изменения в предыдущий Commit. 
5.	Слияние веток.
1.	Изучить слияние веток с помощью Squash Commits, Merge, Rebase. Привести примеры слияния и полученные результаты. Слияние веток проводить повторно, выполняя пункт 4. 
2.	Разрешение конфликтов слияния. Создать третью LocalWorkingDirectory «person3» и загрузить туда копию из Remote Repository. Для третьей LocalWorkingDirectory создать свою ветку «dev3» и изменить в ней один из первых файлов с последующим созданием Commit и выгрузкой Commit на Remote Repository. Также необходимо изменить другой файл в LocalWorkingDirectory «person2» в ветке «dev2», создать и выгрузить новый Commit на Remote Repository. В LocalWorkingDirectory «person1» необходимо изменить тот же файл, что и в третьей LocalWorkingDirectory, но в другом месте и добавить Commit в ветку «dev1». Данные действия имитирую работу трех программистов над разными задачами и одинаковыми или различными файлами проекта. Поочередно проведите слияние веток «dev» с веткой «master» и опишите результаты. Рассмотрите методы исправления конфликтов слияния.
6.	Использовать git log для нахождения хэша Commit. Откатить изменения до выбранного Commit а с помощью git reset --hard <commit_hash>. Для просмотра изменений в каждом Commit можно использовать git log –p
7.	Используйте команду git cherry-pick <commit_hash> для перемещения Commit из ветки «dev2» на текущую ветку. Используйте git rebase для перебазирования Commit ветки «dev1» на другую ветку. Для перемещения нескольких Commit можно использовать git rebase -i <commit_hash>.  Создайте серию коммитов в ветке «dev3», создайте патчи для этих коммитов с помощью git format-patch и примените их к ветке main с помощью git apply
8.	Установите Git LFS на ваш компьютер, если он еще не установлен, с помощью инструкций на официальном сайте Git LFS.
9.	Добавьте поддержку Git LFS к существующему репозиторию с помощью команды git lfs install.
10.	Добавьте несколько больших файлов в репозиторий с помощью команды git lfs track "*.extension", где extension - расширение файлов, которые вы хотите отслеживать.
11.	Сделайте Commit с добавленными большими файлами с помощью команды git add . и git commit -m "Added large files".
12.	Проверьте статус больших файлов с помощью команды git lfs ls-files, чтобы убедиться, что они правильно отслеживаются Git LFS.
13.	Отправьте изменения на удаленный репозиторий.
14.	Скачайте репозиторий на другой компьютер и убедитесь, что большие файлы успешно загружены с помощью Git LFS.
15.	Попробуйте изменить настройки отслеживания файлов в Git LFS, например, добавить новые типы файлов для отслеживания.
16.	Удалите один из больших файлов из репозитория с помощью команды git rm --cached filename и проверьте, что он больше не отслеживается Git LFS.
17.	После успешного использования Git LFS для управления большими файлами завершите работу, убедитесь, что все изменения сохранены и продолжайте разработку проекта с использованием Git LFS для эффективного управления большими файлами.
