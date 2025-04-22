# 🏠 Smart Home System – Aplikacja Webowa Django z MQTT

## 📌 Opis projektu

**Smart Home System** to aplikacja webowa służąca do zarządzania inteligentnym domem, oparta na frameworku **Django** oraz protokole **MQTT**. Umożliwia zdalne sterowanie urządzeniami IoT (takimi jak światła, gniazdka, czujniki temperatury i ruchu), wizualizację danych pomiarowych oraz tworzenie automatycznych scenariuszy (reguł).

Projekt integruje się z urządzeniami typu **ESP32/ESP8266** lub dowolnym innym klientem MQTT, obsługuje wielu użytkowników, gromadzi historię zdarzeń oraz pozwala na dynamiczną rozbudowę o nowe moduły.

---

## 🌟 Kluczowe funkcjonalności

### 1. 🔐 System użytkowników
- Rejestracja i logowanie użytkowników.
- Panel użytkownika z przeglądem urządzeń, danych i aktywności.
- Obsługa sesji, zabezpieczeń i ról użytkowników (np. administrator).

### 2. 💡 Zdalne sterowanie urządzeniami (MQTT)
- Włączanie/wyłączanie urządzeń w czasie rzeczywistym za pomocą tematów MQTT.
- Obsługa czujników (odczyt danych) i aktuatorów (wydawanie poleceń).
- Powiązanie tematów MQTT z urządzeniami przypisanymi do użytkowników.

### 3. 🧠 Automatyzacja i reguły
- Tworzenie reguł automatycznych, np. „włącz światło o 20:00” lub „gdy temperatura < 18°C, uruchom grzejnik”.
- Harmonogramy oraz warunki logiczne.
- Przechowywanie i edycja reguł przez GUI.

### 4. 📋 Lista i zarządzanie urządzeniami
- Dodawanie, edytowanie i usuwanie urządzeń.
- Przypisywanie nazw, ikon, pokoi oraz tematów MQTT.
- Podgląd statusu (online/offline) oraz ostatniej aktywności.

### 5. 📈 Wizualizacja danych
- Wykresy danych historycznych z czujników (temperatura, wilgotność, ruch itd.).
- Integracja z bibliotekami **Plotly** lub **Matplotlib**.
- Możliwość filtrowania danych według daty, urządzenia, zakresu czasu.

### 6. 📜 Historia zdarzeń
- Rejestrowanie wszystkich interakcji użytkownika i urządzeń.
- Logi dostępne z panelu użytkownika (kto, kiedy, co zrobił).
- Eksport historii do pliku CSV.

### 7. ⚙️ Panel administracyjny i ustawienia
- Konfiguracja globalnych ustawień aplikacji:
  - Adres i port brokera MQTT.
  - Domyślne reguły automatyzacji.
  - Personalizacja nazw urządzeń.
- Zarządzanie kontami użytkowników i urządzeniami.

---

## 🛠️ Technologie

- **Backend:** Python 3.10, Django 4.x
- **MQTT:** `paho-mqtt`, broker Mosquitto lub ESP32 jako klient
- **Frontend:** HTML, CSS (Bootstrap), JavaScript
- **Baza danych:** SQLite (domyślnie), PostgreSQL (opcjonalnie)
- **Wizualizacja danych:** Matplotlib, Plotly
- **Protokół komunikacji:** MQTT

---

## 🚀 Jak uruchomić projekt (dla początkujących z Django)

### 🔧 Czym jest Django?

**Django** to wysokopoziomowy framework webowy dla Pythona, który umożliwia szybkie tworzenie aplikacji internetowych w architekturze MVC (Model-View-Controller). Django automatycznie generuje panele administracyjne, obsługuje formularze, routing, bazę danych, logowanie, i wiele więcej.

---

## ▶️ Szybki start – krok po kroku

### 1. 📦 Klonowanie repozytorium

```bash
git clone https://github.com/twoje_repo/smart-home-system.git
cd smart-home-system
```
