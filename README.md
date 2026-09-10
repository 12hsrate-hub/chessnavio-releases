# ChessNavio

Официальные выпуски расширения ChessNavio для Chrome, Edge и Яндекс Браузера.

ChessNavio показывает шахматные подсказки прямо рядом с доской: основной ход,
короткую идею и варианты под выбранный уровень. Завершённую партию можно
разобрать по PGN или FEN без установки — на
[chessnavio.ru/analyze](https://chessnavio.ru/analyze).

Анализ выполняется на вашем компьютере. Во время партии позиции и подсказки не
отправляются на сервер. Первые 3 партии или тренировки каждые 30 дней доступны
бесплатно.

Сайт: [chessnavio.ru](https://chessnavio.ru)

## Скачать

Актуальный выпуск:
[ChessNavio 1.2.3](https://github.com/12hsrate-hub/chessnavio-releases/releases/latest).

В каждом релизе два архива:

- `chessnavio-*-chrome-standard.zip` — обычная версия, подходит большинству
  компьютеров;
- `chessnavio-*-chrome-max.zip` — версия для мощных компьютеров.

Рядом публикуется `SHA256SUMS.txt` — сравните контрольную сумму перед
установкой.

**Пошаговая установка** (рекомендуется):
[chessnavio.ru/install](https://chessnavio.ru/install?utm_source=github&utm_medium=referral&utm_campaign=active_hints_launch&utm_content=release_notes)

VirusTotal для текущей версии 1.2.3:

- [обычная версия](https://www.virustotal.com/gui/file/c219cd83a5d44f9926b04e260d202c1c6a465a6f7b007aa74a8adcb4d16a749a)
- [версия для мощных компьютеров](https://www.virustotal.com/gui/file/e87e5981ba5f84e13b7d25f75614c5187e91ef7b429c0dc8dfe134776f88e52b)

## Что умеет расширение

- подсказка сразу, по шагам или после собственного хода;
- уровень хода от клубного до максимального;
- оценка позиции и до трёх продолжений;
- разбор ошибок после партии;
- Lichess, Chess.com, World Chess и Chess King — с предупреждением о правилах
  площадки.

Подробнее о режимах: [chessnavio.ru/chess-helper](https://chessnavio.ru/chess-helper).

## Безопасность и прозрачность

- Исходный код продукта и инфраструктура — в закрытом репозитории. Здесь только
  готовые файлы выпуска и пользовательская документация.
- Стабильные выпуски публикуются как **неизменяемые**: после публикации GitHub
  не позволяет заменить файлы или перенести тег.
- Встроенный Stockfish распространяется по GPLv3; соответствующие исходники
  приложены к релизу.
- Перед использованием подсказок проверьте правила выбранной шахматной
  площадки.

Проверка неизменяемости выпуска (GitHub CLI):

```bash
gh release verify v1.2.3 --repo 12hsrate-hub/chessnavio-releases
gh release verify-asset v1.2.3 \
  ./chessnavio-1.2.3-chrome-standard.zip \
  --repo 12hsrate-hub/chessnavio-releases
```

Поддержка: [support@chessnavio.ru](mailto:support@chessnavio.ru)
