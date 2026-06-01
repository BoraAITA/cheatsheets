# 🔄 Git Cheatsheet

## Temel Komutlar

```bash
git init                    # Yeni repo başlat
git clone <url>             # Repo kopyala
git status                  # Durum göster
git add .                   # Tüm değişiklikleri ekle
git commit -m "mesaj"       # Commit et
git push                    # Uzak sunucuya gönder
git pull                    # Değişiklikleri çek
```

## Branch İşlemleri

```bash
git branch                  # Branch'leri listele
git checkout -b <branch>    # Yeni branch oluştur ve geç
git switch <branch>         # Branch değiştir
git merge <branch>          # Branch birleştir
git branch -d <branch>      # Branch sil
```

## Undo İşlemleri

```bash
git reset --soft HEAD~1     # Son commit'i geri al (değişiklikleri koru)
git reset --hard HEAD~1     # Son commit'i geri al (değişiklikleri sil)
git stash                   # Değişiklikleri sakla
git stash pop               # Saklanan değişiklikleri geri al
```

## Log ve Diff

```bash
git log --oneline           # Kısa log göster
git log --graph             # Grafik log
git diff                    # Değişiklikleri göster
git diff --staged           # Stage edilmiş değişiklikleri göster
```

## İpuçları

```bash
git commit -m "fix: hata düzeltme"  # Conventional commit
git rebase -i HEAD~3                # Son 3 commit'i düzenle
git cherry-pick <commit>            # Belirli bir commit'i al
```
