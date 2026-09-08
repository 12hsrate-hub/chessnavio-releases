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
[ChessNavio 1.2.2](https://github.com/12hsrate-hub/chessnavio-releases/releases/latest).

В каждом релизе два архива:

- `chessnavio-*-chrome-standard.zip` — обычная версия, подходит большинству
  компьютеров;
- `chessnavio-*-chrome-max.zip` — версия для мощных компьютеров.

Рядом публикуется `SHA256SUMS.txt` — сравните контрольную сумму перед
установкой.

**Пошаговая установка** (рекомендуется):
[chessnavio.ru/install](https://chessnavio.ru/install?utm_source=github&utm_medium=referral&utm_campaign=active_hints_launch&utm_content=release_notes)

VirusTotal для текущей версии 1.2.2:

- [обычная версия](https://www.virustotal.com/gui/file/769d16ac7b8254dfcc972c2a40e4f87891c68e92bd96396f0f61de517a87ad0f)
- [версия для мощных компьютеров](https://www.virustotal.com/gui/file/2aaf79b68b77e765ac6f0f664b2a1df81dfa45047182283fbe04afcaf5a7c9cd)

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
gh release verify v1.2.2 --repo 12hsrate-hub/chessnavio-releases
gh release verify-asset v1.2.2 \
  ./chessnavio-1.2.2-chrome-standard.zip \
  --repo 12hsrate-hub/chessnavio-releases
```

Поддержка: [support@chessnavio.ru](mailto:support@chessnavio.ru)
