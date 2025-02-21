# Pico-Ducky

Bu proje, Raspberry Pi Pico'yu bir USB Rubber Ducky'ye dönüştürmenizi sağlar.

## 🛠️ Gereksinimler

### Donanım
- Raspberry Pi Pico
- Micro USB kablo
- Bilgisayar (Windows, Linux veya MacOS)

### Yazılım
- [CircuitPython](https://circuitpython.org/board/raspberry_pi_pico/) (En son sürüm)
- [Adafruit HID Kütüphanesi](https://github.com/adafruit/Adafruit_CircuitPython_HID)
- Metin editörü (örn. VS Code, Notepad++, vb.)

## 📥 Kurulum Adımları

1. **CircuitPython Kurulumu**
   - BOOTSEL düğmesine basılı tutarak Pico'yu bilgisayarınıza bağlayın
   - CircuitPython .uf2 dosyasını Pico'ya sürükleyip bırakın
   - Pico otomatik olarak yeniden başlayacaktır

2. **Gerekli Kütüphanelerin Kurulumu**
   - [CircuitPython kütüphane paketi](https://circuitpython.org/libraries)ni indirin
   - Aşağıdaki dosyaları Pico'nun `lib` klasörüne kopyalayın:
     - `adafruit_hid`
     - `asyncio`
     - `adafruit_debouncer.mpy`

3. **Pico-Ducky Dosyalarının Yüklenmesi**
   - `code.py` dosyasını Pico'nun ana dizinine kopyalayın
   - `payload.dd` dosyasını oluşturun ve Ducky Script kodunuzu buraya yazın

## 💻 Kullanım

1. Payload hazırlama:
   - `payload.dd` dosyasını metin editörü ile açın
   - [Ducky Script sözdizimini](https://docs.hak5.org/hak5-usb-rubber-ducky/ducky-script-basics/ducky-script-basics) kullanarak kodunuzu yazın
   - Dosyayı kaydedin

2. Çalıştırma:
   - Pico'yu hedef bilgisayara bağlayın
   - Payload otomatik olarak çalışacaktır


## ⚠️ Güvenlik Uyarısı

Bu tool sadece eğitim ve test amaçlı kullanılmalıdır. Kötü amaçlı kullanımından doğacak sonuçlardan kullanıcı sorumludur.

## 📜 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.
