# 🇺🇿 Git Buyruqlari - O‘zbek tilida

Git — bu fayllar ustida bajarilgan o‘zgarishlarni boshqarish tizimi. Quyida eng ko‘p ishlatiladigan Git buyruqlari va ularning nima qilishini sodda, tushunarli shaklda ko‘rishingiz mumkin.

---

## 🛠️ 1. Gitni sozlash (bir marta bajariladi)

### `git config --global user.name "Ismingiz"`
> Gitga foydalanuvchi ismini sozlaydi. Commitlarda ko‘rinadi.

### `git config --global user.email "email@misol.com"`
> Gitga foydalanuvchi emailini sozlaydi. Commitlarda ko‘rinadi.

---

## 📁 2. Yangi loyiha boshlash

### `git init`
> Yangi Git repository (loyiha) yaratadi. Bu katalogda `.git` papkasi hosil qiladi.

---

## 📦 3. Mavjud loyihani nusxalash

### `git clone <repository_url>`
> Uzoqdagi (masalan, GitHub'dagi) loyihani kompyuterga yuklab oladi.

---

## 🔍 4. Holatni tekshirish

### `git status`
> Hozirgi repository holatini ko‘rsatadi (qaysi fayllar o‘zgargan, sahnaga qo‘shilganmi yoki yo‘q).

---

## ➕ 5. O‘zgartirilgan fayllarni sahnaga qo‘shish

### `git add <fayl_nomi>`
> Belgilangan faylni sahnaga (stage) qo‘shadi.

### `git add .`
> Barcha o‘zgargan fayllarni sahnaga qo‘shadi.

---

## ✅ 6. O‘zgarishlarni saqlash

### `git commit -m "Xabar"`
> Sahnadagi fayllarni versiya sifatida saqlaydi. `"Xabar"` o‘zgarish haqida izoh bo‘ladi.

---

## 📜 7. Versiyalar tarixini ko‘rish

### `git log`
> Qilingan commitlar ro‘yxatini ko‘rsatadi.

---

## 🧾 8. O‘zgarishlar tafsilotlarini ko‘rish

### `git diff`
> Commit qilinmagan o‘zgarishlarni ko‘rsatadi.

---

## 🌿 9. Tarmoqlar bilan ishlash

### `git branch`
> Mavjud tarmoqlarni ko‘rsatadi.

### `git branch <yangi_tarmoq>`
> Yangi tarmoq yaratadi.

### `git checkout <tarmoq_nomi>`
> Belgilangan tarmoqqa o‘tadi.

### `git checkout -b <yangi_tarmoq>`
> Yangi tarmoq yaratadi va shu tarmoqqa o‘tadi.

### `git switch <tarmoq_nomi>`
> Zamonaviy tarmoqqa o‘tish buyrug‘i (checkout o‘rniga ishlatiladi).

---

## 🔀 10. Tarmoqlarni birlashtirish

### `git merge <tarmoq_nomi>`
> Belgilangan tarmoqdagi o‘zgarishlarni joriy tarmoqqa qo‘shadi.

---

## 🌐 11. Uzoqdagi repository bilan ishlash

### `git remote add origin <url>`
> Uzoqdagi Git repository'ni `origin` nomi bilan bog‘laydi.

### `git push origin <tarmoq_nomi>`
> Commitlarni uzoqdagi repository'ga (masalan GitHub) yuboradi.

### `git pull origin <tarmoq_nomi>`
> Uzoqdagi repository'dan o‘zgarishlarni yuklab olib joriy loyiha bilan birlashtiradi.

### `git fetch`
> Uzoqdagi o‘zgarishlarni yuklab oladi, lekin avtomatik birlashtirmaydi.

---

## 🗑️ 12. O‘chirish va bekor qilish

### `git rm <fayl>`
> Git'dan faylni o‘chiradi (va diskdan ham o‘chiradi).

### `git reset --hard <commit_id>`
> Loyihani ko‘rsatilgan commit holatiga qaytaradi. Barcha keyingi o‘zgarishlar o‘chadi.

### `git revert <commit_id>`
> Oldingi commit’ni bekor qiluvchi yangi commit yaratadi.

---

## 📥 13. Saqlash (stash)

### `git stash`
> Hozirgi o‘zgarishlarni vaqtincha yashiradi, lekin yo‘q qilmaydi.

### `git stash pop`
> Yashirilgan o‘zgarishlarni tiklaydi.

---

## 🏷️ 14. Versiyalash

### `git tag <yorliq_nomi>`
> Hozirgi commit'ga yorliq qo‘yadi (masalan, `v1.0.0`).

---

## 🔎 15. .gitignore

**`.gitignore` fayli** — Git e’tibor bermasligi kerak bo‘lgan fayllar ro‘yxatini saqlaydi (masalan: `*.log`, `venv/`, `node_modules/`).

---

## 📌 Maslahatlar

- Har doim `git status` bilan boshlang.
- Commit xabarlari tushunarli bo‘lsin (`git commit -m "login sahifasini tuzatildi"`).
- `git log --oneline` — qisqacha commitlar ro‘yxati.
- Xatolik bo‘lsa, `git reset`, `git stash`, `git checkout` yordam beradi.

---

## 📚 Qo‘shimcha havolalar

- [Rasmiy sayt](https://git-scm.com/)
- [Pro Git kitobi (inglizcha)](https://git-scm.com/book/en/v2)

