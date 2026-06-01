# 🐧 Linux Cheatsheet

## Dosya İşlemleri

```bash
ls -la                      # Detaylı listeleme
cd <dizin>                  # Dizin değiştir
mkdir <dizin>               # Dizin oluştur
rm -rf <dizin>              # Dizin ve içeriğini sil
cp -r <kaynak> <hedef>      # Kopyala
mv <kaynak> <hedef>         # Taşı veya yeniden adlandır
find . -name "*.txt"        # Dosya bul
```

## Dosya Okuma/Yazma

```bash
cat <dosya>                 # Dosyayı göster
less <dosya>                # Sayfalı göster
head -n 20 <dosya>          # İlk 20 satırı göster
tail -f <log-dosyasi>       # Canlı log takip
grep "arama" <dosya>        # Dosyada ara
```

## Sistem

```bash
top                         # Süreçleri göster
htop                        # Gelişmiş süreç gösterici
df -h                       # Disk kullanımı
free -h                     # Bellek kullanımı
uname -a                    # Sistem bilgisi
uptime                      # Çalışma süresi
```

## Ağ

```bash
ping <host>                 # Ağ bağlantısı test
curl <url>                  # HTTP isteği
wget <url>                  # Dosya indir
netstat -tuln               # Açık portları göster
ss -tuln                    # Modern port görüntüleme
```

## İpuçları

```bash
history | grep "komut"      # Komut geçmişinde ara
!!                          # Son komutu tekrar çalıştır
sudo !!                     # Son komutu sudo ile çalıştır
alias ll="ls -la"           # Kısayol oluştur
chmod +x <dosya>            # Çalıştırma izni ver
```
