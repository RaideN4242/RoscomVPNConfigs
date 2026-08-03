# 🔥 RoscomVPNConfig

> Исправленная версия конфигов маршрутизации от [RoscomVPN Routing](https://github.com/hydraponique/roscomvpn-routing)

---

## 📌 О проекте

Этот репозиторий содержит **исправленные конфиги маршрутизации** для приложений **Happ** и **Incy**, основанные на оригинальных конфигах от [hydraponique/roscomvpn-routing](https://github.com/hydraponique/roscomvpn-routing).

Особенности оригинального конфига:
- 🚀 **GlobalProxy** — весь трафик идёт через VPN
- 🇷🇺 **Российские сайты** — напрямую (`geosite:category-ru`)
- 🎮 **Игровые сервисы** — напрямую (Steam, Epic Games, Riot, и др.)
- 🌐 **Зарубежные сервисы** — через прокси (YouTube, Telegram, GitHub)
- 🛑 **Блокировка рекламы и трекеров** (`geosite:category-ads`)
- 🔐 **DNS-over-HTTPS** — Google DNS (8.8.8.8) для зарубежного трафика, Яндекс DNS (77.88.8.8) — для российского
- 🏛️ **DNS-привязка сайтов налоговой** — для корректной работы с ФНС

---

## 🔧 Что исправлено

Оригинальный конфиг использовал `google.com` для проверки пинга, что вызывало ошибку TLS-рукопожатия при использовании на серверах в РФ.

**Что изменил:**  
В раздел `DirectSites` добавлен домен `gstatic.com`

---

⚙️ Настройка сервера

В панели **3x-ui** в разделе настроек XRAY, в поле **"URL для теста исходящего"** укажите:
https://www.gstatic.com/generate_204

![3x-ui settings](https://img.shields.io/badge/%D0%9D%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-3x--ui-blue)
