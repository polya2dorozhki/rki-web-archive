# Коллекция веб-архивов сайтов по изучению русского языка как иностранного

Этот репозиторий содержит коллекцию веб-архивов (WARC) образовательных сайтов, посвящённых изучению русского языка.

Данные собраны с помощью инструмента **wpull**, проанализированы с помощью **metawarc**, а показатели архивируемости — через сервис **ArchiveReady**.

## Автор проекта
**Поля Дорожкина**

## Лицензия
**CC0 1.0 Universal (Public Domain)**  
Материалы можно использовать, копировать и перерабатывать без ограничений.

---

# Структура коллекции

| Сайт | URL | Markdown-файлы |  
|------|-----|----------------|  
| **learnrussian.rt.com** | https://learnrussian.rt.com | см. в папке `md_files/` |  
| **russianforfree.com** | https://russianforfree.com | см. в папке `md_files/` |  
| **russianstepbystep.com** | https://russianstepbystep.com | см. в папке `md_files/` |  

---

# WARC-архивы

Все WARC-файлы коллекции доступны по ссылке:

**Google Drive:**  
https://drive.google.com/drive/folders/11iYaL5_yL3B7DSRAJ3iOvaIJ_n9usd2S?usp=sharing

---

# ArchiveReady — Показатели архивируемости

## learnrussian.rt.com
![ArchiveReady Summary LR](lr_archiveready.png.png)

- **Overall:** 76%  
- **Accessibility:** 47%  
- **Cohesion:** 90%  
- **Metadata:** 100%  
- **Standards Compliance:** 69%  

---

# MIME-тип анализ (metawarc)

## learnrussian.rt.com

| MIME                           | Файлов | Доля |
|-------------------------------|--------|------|
| application/pdf               | 91     | 58.25% |
| image/png                     | 1445   | 27.50% |
| image/jpeg                    | 86     | 6.80% |
| text/html                     | 472    | 6.47% |
| image/gif                     | 85     | 0.47% |
| application/javascript        | 3      | 0.28% |
| text/css                      | 9      | 0.13% |
| application/octet-stream      | 6      | 0.08% |
| application/json              | 1      | 0.0004% |
| **Итого:**                    | **2198** | **100%** |

---

# russianforfree.com
![ArchiveReady Summary RF](rf_archiveready.png.png)

- **Overall:** 72%  
- **Accessibility:** 47%  
- **Cohesion:** 69%  
- **Metadata:** 100%  
- **Standards Compliance:** 72%  

### MIME-анализ

| MIME                               | Файлов | Доля |
|-----------------------------------|--------|------|
| audio/mpeg                        | 1045   | 66.81% |
| text/html                         | 666    | 25.08% |
| image/jpeg                        | 512    | 2.80% |
| image/png                         | 293    | 2.05% |
| application/pdf                   | 19     | 1.70% |
| image/gif                         | 104    | 1.00% |
| application/javascript            | 11     | 0.23% |
| application/x-shockwave-flash     | 6      | 0.16% |
| text/xml                          | 2      | 0.12% |
| text/css                          | 8      | 0.03% |
| text/plain                        | 1      | 0.0003% |
| **Итого:**                        | **2667** | **100%** |

---

# russianstepbystep.com
![ArchiveReady Summary RSBS](rsbs_archiveready.png.png)

- **Overall:** 84%  
- **Accessibility:** 41%  
- **Cohesion:** 100%  
- **Metadata:** 100%  
- **Standards Compliance:** 93%  

### MIME-анализ

| MIME                           | Файлов | Доля |
|-------------------------------|--------|------|
| text/html                     | 6212   | 43.27% |
| image/jpeg                    | 1832   | 22.07% |
| audio/mpeg                    | 68     | 11.06% |
| application/javascript        | 476    | 10.78% |
| image/png                     | 465    | 7.82% |
| text/css                      | 186    | 1.47% |
| application/json              | 1472   | 1.22% |
| image/svg+xml                 | 19     | 0.59% |
| text/xml                      | 372    | 0.45% |
| application/vnd.ms-fontobject | 11     | 0.26% |
| font/ttf                      | 9      | 0.20% |
| application/msword            | 2      | 0.20% |
| x-font/woff                   | 8      | 0.14% |
| application/rss+xml           | 82     | 0.13% |
| application/pdf               | 2      | 0.09% |
| font/woff2                    | 4      | 0.05% |
| image/gif                     | 46     | 0.04% |
| text/plain                    | 12     | 0.03% |
| **Итого:**                    | **11280** | **100%** |

---

# Папка Markdown-файлов

Все Markdown-файлы с контентом каждого сайта находятся в папке `md_files`.

# Дополнительные данные

В корне проекта находятся два файла:

- **export.jsonl** — содержит извлечённый текстовый контент страниц и сопутствующую информацию из WARC-архивов.
- **metadata.jsonl** — включает технические метаданные страниц (MIME-типы, размеры, структура ресурсов), полученные из WARC-файлов.

