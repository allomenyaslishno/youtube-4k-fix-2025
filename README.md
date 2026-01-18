# 🚀 YouTube & Discord Acceleration Tool (No-VPN method)

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Android%20%7C%20iOS-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Uptime](https://img.shields.io/badge/uptime-99.9%25-orange)

[**🇷🇺 РУССКАЯ ВЕРСИЯ**](#ru) | [**🇬🇧 ENGLISH VERSION**](#en)

---

<a name="ru"></a>
## 🇷🇺 Описание проблемы
В последнее время наблюдается искусственная деградация скорости доступа к серверам `googlevideo.com` (YouTube) и голосовым шлюзам Discord. Провайдеры фильтруют пакеты на основе SNI, что приводит к буферизации видео даже на тарифах 100+ Мбит/с.

## 🛠 Техническое решение
Данный метод **не использует** классические VPN-туннели, которые режут скорость и повышают пинг.
Мы используем оптимизацию маршрутизации через протокол **VLESS + Reality (uTLS)**.

**Как это работает:**
1. Трафик до видеохостинга инкапсулируется в защищенный TLS-поток.
2. Для оборудования провайдера (DPI) это выглядит как обычное подключение к зарубежному "белому" серверу (например, Microsoft или Samsung).
3. Пакеты не отбрасываются, и скорость восстанавливается до тарифной (4K/8K работает без лагов).

### ⚡ Преимущества метода
* **Нулевой Impact на систему:** Не висит в фоне как тяжелое приложение.
* **Низкий Ping:** Идеально для геймеров (Discord, Twitch).
* **Open Source:** Используются клиенты с открытым исходным кодом.

---

## ⚙️ Инструкция по установке (Quick Start)

Вам не нужно компилировать код или поднимать свой сервер. Я развернул ноду и написал бота, который автоматически генерирует конфиг-файл (`client config`) для подключения.

### Шаг 1. Генерация конфига
Получите персональную строку подключения (Access Key) через нашего автоматического бота. Это бесплатно.

👉 **[СГЕНЕРИРОВАТЬ КЛЮЧ (GET KEY)](https://t.me/@ALLOMENYASLISHNO_bot)**

### Шаг 2. Выбор клиента
Скачайте клиент с открытым исходным кодом (Open Source) под вашу платформу:

| Платформа | Рекомендуемый клиент | Ссылка |
| :--- | :--- | :--- |
| **Windows** | **Nekoray** / Hiddify | [Скачать с GitHub](https://github.com/Matsuridayo/nekoray/releases) |
| **Android** | **v2rayNG** | [Скачать с Google Play](https://play.google.com/store/apps/details?id=com.v2ray.ang) |
| **iOS / macOS** | **V2Box** | [Скачать в AppStore](https://apps.apple.com/us/app/v2box-v2ray-client/id6446814690) |

### Шаг 3. Запуск
1. Скопируйте ключ, полученный в боте.
2. Откройте приложение.
3. Нажмите `Import from Clipboard` (или `Ctrl+V` в Windows).
4. Активируйте туннелирование.

---

### 📊 Результаты тестов (Benchmarks)

**До фикса:**
> 🔻 Ping: 150ms | Jitter: 45ms | YouTube: 480p (buffer)

**После применения:**
> 🟢 Ping: 35ms | Jitter: 2ms | YouTube: 2160p (4K HDR)

---

## ⚠️ Disclaimer
Данный репозиторий и инструмент предоставляются исключительно в образовательных целях для изучения принципов маршрутизации сетей и обхода ошибок конфигурации провайдеров. Автор не несет ответственности за использование.

---

<a name="en"></a>
## 🇬🇧 English Description
Fix for YouTube throttling and Discord connection issues based on VLESS + Reality protocol. Bypasses DPI analysis by masking traffic as standard TLS handshake.

**How to use:**
1. Get your free access config via bot: **[GET CONFIG](https://@ALLOMENYASLISHNO_bot)**
2. Install **v2rayNG** (Android) or **V2Box** (iOS).
3. Paste the key and enjoy high-speed streaming.

---
**Tags:**
`youtube-fix` `dpi-bypass` `goodbyedpi` `zapret` `discord-fix` `packet-loss` `vless` `reality` `xray-core` `russia-internet` `4k-streaming`
