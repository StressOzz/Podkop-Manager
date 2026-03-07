<h1 align="center">Podkop Manager</h1>

<p align="center">
  <b>Многофункциональный установщик, менеджер и интегратор для OpenWRT.</b><br>
    <b>Обеспечивает обход DPI на уровне роутера, интеграцию прокси с фильтрацией трафика,</b><br>
     <b> стабильную маршрутизацию YouTube, Cloudflare, Госуслуг и др.</b><br>


> [!IMPORTANT]
> Рекомендуется устанавливать на "чистый" роутер !

> [!WARNING]
> Все настройки Podkop будут сброшены !

---

## Запуск менеджера
Скрипт который запускает менеджер
```
sh <(wget -O - https://raw.githubusercontent.com/StressOzz/Podkop-Manager/main/Podkop-Manager.sh)
```

## Основные функции

### 1) Установить Podkop
Устанавливает последнию версию Podkop
### 2) Удалить Podkop
Удаляеет Podkop
### 3) Установить ByeDPI
Устанавливает последнию версию ByeDPI
### 4) Удалить ByeDPI
Удаляеет ByeDPI
### 5) Интегрировать ByeDPI в Podkop
Настривает Podkop для работы с ByeDPI (все настройки Podkop будут сброшены)
### 6) Изменить текущую стратегию ByeDPI
Позволяет изменить стратегию ByeDPI
### 7) Установить AWG и интерфейс AWG
Устанавливает AmneziaWG и интерфейс AWG
### 8) Удалить AWG и интерфейс AWG
Удаляеет AmneziaWG и интерфейс AWG
### 9) Интегрировать AWG в Podkop
Настривает Podkop для работы с AWG (все настройки Podkop будут сброшены)
### 0) Перезагрузить устройство
Reboot

## Советы по использованию

- После первой интеграции ByeDPI обязательно перезагрузите роутер

- Необходимо загрузить конфиг Amnezia в **Network → Interfaces → AWG → Edit → Load configuration…**

- В конфиге Amnezia, обязательно должна быть строчка `PersistentKeepalive = 25`

- Рекомендовано подождать 30 секунд после перезагрузки устройства, чтобы все службы (ByeDPI, Podkop, sing-box, DNS и маршрутизация) полностью запустились и вступили в силу

- Если **GitHub** выдаёт ошибку лимита запросов — подождите 30–60 минут

- При смене стратегии **ByeDPI** (пункт 4) можно не перезагружать устройство

- Всё что связанно с **Podkop** можно прочитать в [Документация](https://podkop.net/)

---
[<img width="190" height="175" alt="donate-button-click-donation-charity-600nw-2339825981" src="https://github.com/user-attachments/assets/2999757b-fbf3-4149-bf6c-48bf3e241529" />](https://github.com/StressOzz#-поддержать-проект)

---

[![Star History Chart](https://api.star-history.com/svg?repos=StressOzz/Podkop-ByeDPI-OpenWRT&type=date&legend=top-left)](https://www.star-history.com/#StressOzz/Podkop-ByeDPI-OpenWRT&type=date&legend=top-left)

---
## Большое спасибо

- **[itdoginfo](https://github.com/itdoginfo)** за [podkop](https://github.com/itdoginfo/podkop)
- **[hufrea](https://github.com/hufrea)** за [byedpi](https://github.com/hufrea/byedpi)
- **[spvkgn](https://github.com/spvkgn)** за GitHub Actions
- **[romanvht](https://github.com/romanvht)** за возможность тестировать стратегии
- **[DPITrickster](https://github.com/DPITrickster)** за версию ByeDPI для OpenWRT и за написание гайда по ручной установке
