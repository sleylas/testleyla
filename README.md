Oтличия команды git pull и git fetch.

При использовании pull, git пытается сделать всё за вас. Он сливает любые внесённые коммиты в ветку, в которой вы сейчас работаете. Команда pull автоматически сливает коммиты, не давая вам сначала просмотреть их. Если вы не пристально следите за ветками, выполнение этой команды может привести к частым конфликтам.  

При использовании fetch, git собирает все коммиты из целевой ветки, которых нет в текущей ветке, и сохраняет их в локальном репозитории. Однако он не сливает их в текущую ветку. Это особенно полезно, если вам нужно постоянно обновлять свой репозиторий, но вы работаете над функциональностью, неправильная реализация которой может негативно сказаться на проекте в целом. Чтобы слить коммиты в основную ветвь, нужно использовать merge.  

Грубо говоря, по дефолту git pull — это шоткод для последовательности двух команд: git fetch (получение изменений с сервера) и git merge (сливание в локальную копию).
