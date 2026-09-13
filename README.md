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
[ChessNavio 1.3.0](https://github.com/12hsrate-hub/chessnavio-releases/releases/latest).

В каждом релизе два архива:

- `chessnavio-*-chrome-standard.zip` — обычная версия, подходит большинству
  компьютеров;
- `chessnavio-*-chrome-max.zip` — версия для мощных компьютеров.

Рядом публикуется `SHA256SUMS.txt` — сравните контрольную сумму перед
установкой.

**Пошаговая установка** (рекомендуется):
[chessnavio.ru/install](https://chessnavio.ru/install?utm_source=github&utm_medium=referral&utm_campaign=active_hints_launch&utm_content=release_notes)

VirusTotal для текущей версии 1.3.0:

- [обычная версия](https://www.virustotal.com/gui/file/5d7c79e78eb5bed314fd42159cf920858f02db130ef5c46c3bd0eb28e0111950)
- [версия для мощных компьютеров](https://www.virustotal.com/gui/file/79c4b788b994486342d24eda5001f5c9b1807e2ead4bf1be1972753c8dadaf32)

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
gh release verify v1.3.0 --repo 12hsrate-hub/chessnavio-releases
gh release verify-asset v1.3.0 \
  ./chessnavio-1.3.0-chrome-standard.zip \
  --repo 12hsrate-hub/chessnavio-releases
```

Поддержка: [support@chessnavio.ru](mailto:support@chessnavio.ru)
