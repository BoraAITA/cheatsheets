# 🐳 Docker Cheatsheet

## Temel Komutlar

```bash
docker run <image>          # Container başlat
docker run -d <image>       # Arka planda başlat
docker run -p 8080:80 <image>  # Port yönlendirme
docker run -it <image> bash # Etkileşimli shell
docker ps                   # Çalışan container'ları göster
docker ps -a                # Tüm container'ları göster
```

## Yönetim

```bash
docker stop <container>     # Container'ı durdur
docker start <container>    # Container'ı başlat
docker rm <container>       # Container'ı sil
docker rmi <image>          # Image'ı sil
docker logs <container>     # Logları göster
docker exec -it <container> bash  # Container'a gir
```

## Image İşlemleri

```bash
docker images               # Image'ları listele
docker pull <image>         # Image indir
docker build -t <name> .    # Image oluştur
docker tag <image> <tag>    # Image'ı etiketle
docker push <image>         # Image'ı paylaş
```

## Docker Compose

```bash
docker-compose up           # Başlat
docker-compose up -d        # Arka planda başlat
docker-compose down         # Durdur ve sil
docker-compose ps           # Durum göster
docker-compose logs         # Logları göster
docker-compose build        # Yeniden oluştur
```

## Temizlik

```bash
docker system prune         # Kullanılmayan her şeyi temizle
docker system prune -a      # Tüm kullanılmayan image'ları sil
docker volume prune         # Kullanılmayan volume'ları temizle
```
