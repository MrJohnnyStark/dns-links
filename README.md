# DNS Links / Ссылки на публичные DNS-сервера

[![GitHub](https://img.shields.io/badge/GitHub-AristarhUcolov-blue?logo=github)](https://github.com/AristarhUcolov)

A curated collection of public DNS servers with configuration details for various platforms.

Коллекция публичных DNS-серверов с инструкциями по настройке для различных платформ.

---

## 📋 Table of Contents / Содержание

- [About](#about--о-проекте)
- [Available DNS Servers](#available-dns-servers--доступные-dns-сервера)
- [How to Use](#how-to-use--как-использовать)
  - [Android](#android)
  - [iOS/iPhone](#iosiphone)
  - [Windows](#windows)
  - [macOS](#macos)
  - [Linux](#linux)
- [Contributing](#contributing--участие)
- [Author](#author--автор)

---

## About / О проекте

This repository contains links and configuration details for popular public DNS servers including Google DNS, Cloudflare DNS, and AdGuard DNS. These DNS servers can improve your internet speed, security, and privacy.

Этот репозиторий содержит ссылки и детали настройки популярных публичных DNS-серверов, включая Google DNS, Cloudflare DNS и AdGuard DNS. Эти DNS-серверы могут улучшить скорость интернета, безопасность и приватность.

---

## Available DNS Servers / Доступные DNS-сервера

### 🔵 Google DNS

**IPv4 Addresses:**
- Primary: `8.8.8.8`
- Secondary: `8.8.4.4`

**Features:**
- Fast and reliable
- No HTTPS/DNS-over-HTTPS URL available
- Compatible with all devices

**Особенности:**
- Быстрый и надёжный
- URL для HTTPS не предоставлен
- Совместим со всеми устройствами

---

### 🟠 Cloudflare DNS

**IPv4 Addresses:**
- Primary: `1.1.1.1`
- Secondary: `1.0.0.1`

**DNS-over-HTTPS URL:**
- `security.cloudflare-dns.com`

**Features:**
- Focus on privacy and security
- One of the fastest DNS resolvers
- DNS-over-HTTPS support for Android

**Особенности:**
- Фокус на приватности и безопасности
- Один из самых быстрых DNS-резолверов
- Поддержка DNS-over-HTTPS для Android

---

### 🟢 AdGuard DNS

**DNS-over-HTTPS URL:**
- `dns.adguard-dns.com`

**iOS/iPhone Configuration:**
- Profile-based setup: [https://adguard-dns.io/ru/public-dns.html](https://adguard-dns.io/ru/public-dns.html)

**Features:**
- Blocks ads and tracking
- Family protection options available
- DNS-over-HTTPS support
- Easy profile installation for iOS

**Особенности:**
- Блокировка рекламы и трекеров
- Доступна семейная защита
- Поддержка DNS-over-HTTPS
- Простая установка профиля для iOS

---

## How to Use / Как использовать

### Android

#### Method 1: Using DNS-over-HTTPS (Рекомендуется / Recommended)

1. Open Settings / Откройте Настройки
2. Go to Network & Internet / Перейдите в Сеть и Интернет
3. Select Private DNS / Выберите Частный DNS
4. Choose "Private DNS provider hostname" / Выберите "Имя хоста провайдера частного DNS"
5. Enter one of the following / Введите один из следующих:
   - Cloudflare: `security.cloudflare-dns.com`
   - AdGuard: `dns.adguard-dns.com`

#### Method 2: Manual IP Configuration

1. Open WiFi settings / Откройте настройки WiFi
2. Long press on your network / Долго нажмите на вашу сеть
3. Select "Modify network" / Выберите "Изменить сеть"
4. Show advanced options / Показать дополнительные параметры
5. Change IP settings to "Static" / Измените настройки IP на "Статические"
6. Enter DNS servers / Введите DNS-серверы:
   - Google: `8.8.8.8` and `8.8.4.4`
   - Cloudflare: `1.1.1.1` and `1.0.0.1`

---

### iOS/iPhone

#### For AdGuard DNS (Profile-based):

1. Visit / Посетите: [https://adguard-dns.io/ru/public-dns.html](https://adguard-dns.io/ru/public-dns.html)
2. Download the configuration profile / Скачайте конфигурационный профиль
3. Install the profile in Settings / Установите профиль в Настройках
4. Follow the on-screen instructions / Следуйте инструкциям на экране

#### For Google DNS or Cloudflare DNS:

1. Open Settings / Откройте Настройки
2. Select WiFi / Выберите WiFi
3. Tap the (i) icon next to your network / Нажмите на значок (i) рядом с вашей сетью
4. Tap "Configure DNS" / Нажмите "Настроить DNS"
5. Select "Manual" / Выберите "Вручную"
6. Add DNS servers / Добавьте DNS-серверы:
   - Google: `8.8.8.8` and `8.8.4.4`
   - Cloudflare: `1.1.1.1` and `1.0.0.1`

---

### Windows

1. Open Control Panel / Откройте Панель управления
2. Go to Network and Internet > Network and Sharing Center / Перейдите в Сеть и Интернет > Центр управления сетями
3. Click on your active connection / Нажмите на активное подключение
4. Click "Properties" / Нажмите "Свойства"
5. Select "Internet Protocol Version 4 (TCP/IPv4)" / Выберите "Протокол Интернета версии 4 (TCP/IPv4)"
6. Click "Properties" / Нажмите "Свойства"
7. Select "Use the following DNS server addresses" / Выберите "Использовать следующие адреса DNS-серверов"
8. Enter DNS servers / Введите DNS-серверы:
   - Google: Primary `8.8.8.8`, Secondary `8.8.4.4`
   - Cloudflare: Primary `1.1.1.1`, Secondary `1.0.0.1`

---

### macOS

1. Open System Preferences / Откройте Системные настройки
2. Click on Network / Нажмите Сеть
3. Select your active connection / Выберите активное подключение
4. Click "Advanced" / Нажмите "Дополнительно"
5. Go to the DNS tab / Перейдите на вкладку DNS
6. Click the "+" button to add DNS servers / Нажмите кнопку "+" чтобы добавить DNS-серверы:
   - Google: `8.8.8.8` and `8.8.4.4`
   - Cloudflare: `1.1.1.1` and `1.0.0.1`
7. Click "OK" and "Apply" / Нажмите "OK" и "Применить"

---

### Linux

Edit `/etc/resolv.conf` or use NetworkManager:

```bash
# Using command line
sudo nano /etc/resolv.conf

# Add these lines (choose one provider):
nameserver 8.8.8.8
nameserver 8.8.4.4

# Or for Cloudflare:
nameserver 1.1.1.1
nameserver 1.0.0.1
```

For permanent changes, use NetworkManager or your distribution's network configuration tool.

---

## Contributing / Участие

Feel free to contribute by:
- Adding new DNS providers / Добавление новых DNS-провайдеров
- Updating existing information / Обновление существующей информации
- Improving documentation / Улучшение документации
- Reporting issues / Сообщение о проблемах

---

## Author / Автор

**Aristarh Ucolov (Аристарх Уколов)**

---

## License / Лицензия

This project is open source and available for public use.

Этот проект с открытым исходным кодом и доступен для публичного использования.

---

*Last updated: 2025*
