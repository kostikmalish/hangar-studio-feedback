<div align="center">

# Hangar Studio

**Ошибки, предложения и вопросы**

[![Открытые ошибки](https://img.shields.io/github/issues-search/kostikmalish/hangar-studio-feedback?query=is%3Aissue%20is%3Aopen%20label%3A%D0%B1%D0%B0%D0%B3&label=%D0%BE%D1%82%D0%BA%D1%80%D1%8B%D1%82%D1%8B%D0%B5%20%D0%B1%D0%B0%D0%B3%D0%B8&color=e5534b&style=flat-square)](https://github.com/kostikmalish/hangar-studio-feedback/issues?q=is%3Aissue%20is%3Aopen%20label%3A%D0%B1%D0%B0%D0%B3)
[![Исправлено](https://img.shields.io/github/issues-search/kostikmalish/hangar-studio-feedback?query=is%3Aissue%20is%3Aclosed%20label%3A%D0%B1%D0%B0%D0%B3&label=%D0%B8%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%BE&color=2da44e&style=flat-square)](https://github.com/kostikmalish/hangar-studio-feedback/issues?q=is%3Aissue%20is%3Aclosed%20label%3A%D0%B1%D0%B0%D0%B3)
[![Обсуждения](https://img.shields.io/github/discussions/kostikmalish/hangar-studio-feedback?label=%D0%BE%D0%B1%D1%81%D1%83%D0%B6%D0%B4%D0%B5%D0%BD%D0%B8%D1%8F&color=8250df&style=flat-square)](https://github.com/kostikmalish/hangar-studio-feedback/discussions)

[Сообщить об ошибке](https://github.com/kostikmalish/hangar-studio-feedback/issues/new?template=bug.yml) &nbsp;·&nbsp; [Предложить идею](https://github.com/kostikmalish/hangar-studio-feedback/discussions/new?category=ideas) &nbsp;·&nbsp; [Задать вопрос](https://github.com/kostikmalish/hangar-studio-feedback/discussions/new?category=q-a)

</div>

---

Hangar Studio — модификация для «Мира Танков» и World of Tanks, которая позволяет сменить ангар или сделать ангаром любую игровую карту. Здесь собираются отчёты об ошибках, предложения и вопросы пользователей. Все обращения публичны: можно найти уже известную проблему, поддержать чужое предложение или подписаться на обновления.

## Куда писать

| Раздел | Назначение | |
|---|---|---|
| **Ошибки** | Мод работает неправильно, вызывает вылет игры или отображается некорректно. | [Сообщить](https://github.com/kostikmalish/hangar-studio-feedback/issues/new?template=bug.yml) · [Список](https://github.com/kostikmalish/hangar-studio-feedback/issues?q=is%3Aissue%20label%3A%D0%B1%D0%B0%D0%B3) |
| **Предложения** | Новые возможности и улучшения. Предложения с наибольшим числом голосов рассматриваются в первую очередь. | [Предложить](https://github.com/kostikmalish/hangar-studio-feedback/discussions/new?category=ideas) · [Список](https://github.com/kostikmalish/hangar-studio-feedback/discussions/categories/ideas) |
| **Вопросы** | Установка, настройка и работа с модом. Ответ, отмеченный как решение, закрепляется в обсуждении. | [Спросить](https://github.com/kostikmalish/hangar-studio-feedback/discussions/new?category=q-a) · [Список](https://github.com/kostikmalish/hangar-studio-feedback/discussions/categories/q-a) |

## Как сообщить об ошибке

1. Убедитесь, что установлена последняя версия мода.
2. Проверьте [список ошибок](https://github.com/kostikmalish/hangar-studio-feedback/issues?q=is%3Aissue%20label%3A%D0%B1%D0%B0%D0%B3). Если проблема уже известна, поддержите её реакцией и нажмите **Subscribe**, чтобы получить уведомление об исправлении.
3. Заполните форму и приложите `python.log`.

> [!NOTE]
> `python.log` находится в корне папки с игрой: рядом с `Tanki.exe` в «Мире Танков» или с `WorldOfTanks.exe` в World of Tanks. Приложите его сразу после ошибки, не запуская игру повторно. Без лога большинство ошибок найти невозможно.

## Поддерживаемые версии

| Клиент | Статус |
|---|---|
| Мир Танков (Lesta Games) | Поддерживается |
| World of Tanks (Wargaming) | Поддерживается |

## Статусы обращений

```mermaid
flowchart LR
    new([новый]) --> confirmed([подтверждён]) --> progress([в работе]) --> fixed([исправлено])
    new --> needlog([нужен лог]) --> new
    new --> norepro([не воспроизводится])
    new --> duplicate([дубликат])
    new --> intended([так задумано])
```

| Метка | Значение |
|---|---|
| `статус: новый` | Обращение получено и ещё не рассмотрено |
| `статус: нужен лог` | Недостаточно данных, чаще всего не хватает `python.log` |
| `статус: подтверждён` | Ошибка воспроизведена |
| `статус: в работе` | Исправление в процессе |
| `статус: исправлено` | Исправлено, войдёт в следующую версию |
| `статус: не воспроизводится` | Повторить ошибку не удалось, нужны подробности |
| `статус: дубликат` | Ошибка уже описана, ссылка приведена в комментарии |
| `статус: так задумано` | Описанное поведение не является ошибкой |

## Частые вопросы

<details>
<summary><b>После установки игра перезапустилась сама</b></summary>

Это ожидаемое поведение. При первом запуске `openwg_gameface` обновляет список ресурсов игры и один раз перезапускает клиент.

</details>

<details>
<summary><b>Мод не появился в игре</b></summary>

Проверьте, что установлен [openwg_gameface](https://gitlab.com/openwg/wot.gameface/-/releases/) — без него мод не запускается. Файл мода должен находиться в папке `mods/<номер_патча>`.

</details>

<details>
<summary><b>Где находится кнопка мода</b></summary>

В ангаре, рядом с кнопкой уведомлений, появляется кнопка со списком модификаций — Hangar Studio открывается из неё. Если у вас уже установлен другой мод со списком модификаций, Hangar Studio добавится в него, отдельная кнопка не появится.

</details>

<details>
<summary><b>Можно ли писать на английском</b></summary>

Да. English is welcome.

</details>

## Ссылки

- [Тема мода на форуме](https://forum.tanki.su/topic/2225940-14500-hangarstudio-%E2%80%94-%D0%B2%D1%8B%D0%B1%D0%B8%D1%80%D0%B0%D0%B9-%D1%81%D0%BE%D0%B7%D0%B4%D0%B0%D0%B2%D0%B0%D0%B9-%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%B0%D0%B8%D0%B2%D0%B0%D0%B9/) — описание и загрузка
- [openwg_gameface](https://gitlab.com/openwg/wot.gameface/-/releases/) — обязательная зависимость

---

<sub>Hangar Studio — неофициальная модификация, не связанная с Lesta Games и Wargaming.</sub>
