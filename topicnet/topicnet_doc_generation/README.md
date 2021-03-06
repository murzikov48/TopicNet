### Документация


Документация создана при помощи модуля ```pdoc3```:  

```
pip install pdoc3
```

Для пересоздания документации без исходного кода предпочтительно использовать данную команду  
```
pdoc --html -o topicnet_documentation/ -c show_source_code=False --force ../topicnet
```
внутри папки ```topicnet```.

Обычно достаточно команды
```
pdoc --html -o topicnet_doc_generation/ --force ../topicnet
```

### Readme

При необходимости все Markdown-файлы могут быть добавлены в 
текстовом виде в документацию. 

Для добавления *md* в документацию запустите скрипт ```insert_md.sh``` из папки ```topicnet_documentation```. Скрипт использует модуль ```pandoc``` для ковертации *md* в *html*.

### Проблемы

#### ```pdoc``` не распознает команду.

Проверьте, что установлена версия ```pdoc 0.6.3```.
