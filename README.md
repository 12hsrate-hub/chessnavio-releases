# ChessNavio

Официальные выпуски расширения ChessNavio для Chrome, Edge и Яндекс Браузера.

ChessNavio помогает понять позицию, увидеть сильные продолжения и разобрать
ошибки прямо рядом с шахматной доской. Анализ выполняется на компьютере
пользователя: во время партии позиции и подсказки не отправляются на сервер.

Публичная регистрация открыта. Начать можно бесплатно; разбор завершённой
партии или позиции доступен на
[chessnavio.ru/analyze](https://chessnavio.ru/analyze).

## Скачать

Откройте раздел [Releases](https://github.com/12hsrate-hub/chessnavio-releases/releases)
и выберите один архив:

- `chessnavio-*-chrome-standard.zip` — обычная версия, подходит большинству
  компьютеров;
- `chessnavio-*-chrome-max.zip` — версия для мощных компьютеров.

Рядом с архивами публикуется `SHA256SUMS.txt`. Он позволяет убедиться, что
скачанный файл не был изменён. Подробная установка описана на
[chessnavio.ru/install](https://chessnavio.ru/install).

Текущая версия — [ChessNavio 1.0.4](https://github.com/12hsrate-hub/chessnavio-releases/releases/tag/v1.0.4).
VirusTotal не обнаружил вредоносного или подозрительного содержимого:
[обычная версия](https://www.virustotal.com/gui/file/ae82564d58faeac54b50c7b96c44638af848fa76992643bc132ed08de59370f8),
[версия для мощных компьютеров](https://www.virustotal.com/gui/file/ec2be756adaee695a81aabe20431bf65a0bb2f56b00d58a22bdbf0e0aa7efd43).

## Безопасность и прозрачность

- Основной код и внутренняя инфраструктура проекта хранятся в закрытом
  репозитории. Здесь находятся только готовые файлы выпуска и документация.
- Для каждого выпуска публикуются контрольные суммы и отчёт выполненных тестов.
- Стабильные выпуски публикуются как неизменяемые: после публикации GitHub не
  позволяет заменить их файлы или перенести тег на другой коммит.
- Встроенный Stockfish распространяется по GPLv3. Точные соответствующие
  исходники Stockfish опубликованы вместе со стабильной веткой выпусков.
- Перед использованием проверьте правила выбранной шахматной площадки.

Если у вас установлен GitHub CLI, неизменяемость выпуска и точное соответствие
скачанного файла можно проверить командами:

```bash
gh release verify v1.0.4 --repo 12hsrate-hub/chessnavio-releases
gh release verify-asset v1.0.4 \
  ./chessnavio-1.0.4-chrome-standard.zip \
  --repo 12hsrate-hub/chessnavio-releases
```

Сайт проекта: [chessnavio.ru](https://chessnavio.ru)  
Поддержка: [12hsrate@gmail.com](mailto:12hsrate@gmail.com)
