# ESPHome & Home Assistant IoT Cihaz Konfigürasyonları

Bu depo, Home Assistant ile entegre çalışan ESP-12F (ESP8266) ve ESP32-S3 geliştirme kartlarına ait ESPHome konfigürasyon dosyalarını içerir.

## Donanım Özellikleri
* **ESP-12F (NodeMCU v2):** GPIO üzerinden röle anahtarlama ve kontrolü.
* **ESP32-S3:** Dahili sıcaklık, sistem çalışma süresi (uptime), boş RAM, Wi-Fi sinyal gücü izleme ve WS2812 adreslenebilir durum LED kontrolü.

## Güvenlik ve Kurulum
Projede hassas ağ verileri (Wi-Fi SSID, şifreler, statik IP adresleri ve API anahtarları) `!secret` etiketleriyle ayrıştırılmıştır.

1. Depoda bulunan `secrets.yaml.example` dosyasını referans alarak kendi ortamınızda bir `secrets.yaml` dosyası oluşturun.
2. Ağ ve cihaz bilgilerinizi bu dosyaya tanımlayın.
3. ESPHome arayüzü üzerinden ilgili kartlara derleyip yükleyin.



ESPHome & Home Assistant IoT Device Configurations

This repository contains ESPHome configuration files for ESP-12F (ESP8266) and ESP32-S3 development boards that work with Home Assistant.

Hardware Specifications
ESP-12F (NodeMCU v2): Relay switching and control via GPIO.
ESP32-S3: Monitoring of internal temperature, system uptime, free RAM, Wi-Fi signal strength, and WS2812 addressable status LED control.
Security and Setup

Sensitive network information (Wi-Fi SSIDs, passwords, static IP addresses, and API keys) has been separated using !secret tags.

Create a secrets.yaml file in your environment by using the secrets.yaml.example file in the repository as a reference.
Define your network and device information in this file.
Compile and upload the configuration to the corresponding boards through the ESPHome interface.
