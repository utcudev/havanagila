# Hava Nagila — Arduino Buzzer

Pasif buzzer ile "Hava Nagila" ezgisini çalan tek dosyalık Arduino sketch'i.
`tone()` / `noTone()` ve `delay()` kullanır, ek kütüphane gerektirmez.

## Donanım

| Parça | Bağlantı |
|---|---|
| Pasif buzzer (+) | D11 |
| Pasif buzzer (−) | GND |

Arduino Uno/Nano/Mega ve `tone()` destekleyen diğer AVR kartlarında çalışır.

## Kullanım

1. `havanagila.ino` dosyasını Arduino IDE'de aç.
2. Kartını ve portunu seç, yükle.
3. Melodi `setup()` içinde bir kez çalar; `loop()` boştur.

Farklı bir pin kullanmak için dosyanın sonundaki sabiti değiştir:

```cpp
const int BUZZER_PIN = 11;
```

Sürekli tekrar için `song()` çağrısını `loop()` içine taşı.

## Lisans

MIT
