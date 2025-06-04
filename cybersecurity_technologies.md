# 🛡️ 1. Endpoint Detection and Response (EDR)

### **Ta’rif:**

EDR — bu so‘nggi nuqtadagi qurilmalar (kompyuterlar, noutbuklar, serverlar, mobil qurilmalar)da tahdidlarni aniqlash, tahlil qilish va ularga javob berishni avtomatlashtiradigan xavfsizlik texnologiyasi.

### **Asosiy imkoniyatlar:**

- Qurilmada ro‘y berayotgan har bir jarayonni real vaqt rejimida kuzatib boradi.
- Zararli dastur yoki kutilmagan faoliyat aniqlansa, uni to‘xtatadi yoki karantinga oladi.
- Harakatlar jurnalini yaratadi: foydalanuvchi nima qildi, qaysi port ishlatilgan, qaysi IP manzilga bog‘landi va hokazo.
- Ilgari yuz bergan tahdidlarni tahlil qilish orqali tahdid modelini yaratadi (threat hunting).

### **Nega kerak?**

Ko‘pgina kiberhujumlar so‘nggi qurilmalar orqali amalga oshiriladi (masalan, foydalanuvchi phishing havolaga bosadi va zararli kod yuklab olinadi). Shu sababli bu qurilmalarni real vaqt rejimida nazorat qilish juda muhim.

### **Real hayotdagi misol:**

Xodim USB orqali zararli fayl ochadi. EDR bu faylni avtomatik tahlil qiladi, zararli kod borligini aniqlaydi va darhol izolyatsiya qiladi.

### **Foydalari:**

✅ Hujumlarga javob tezligi oshadi  
✅ Hujumlar tarqalishini oldini oladi  
✅ Xodimlar xatolari avtomatik to‘g‘rilanadi  
✅ Raqamli izlar orqali keyingi tahlil osonlashadi

---

# 🧠 2. Threat Intelligence (TI)

### **Ta’rif:**

Threat Intelligence — bu kiber tahdidlar haqidagi **strukturaviy va kontekstli ma’lumotlar** majmuasi bo‘lib, tashkilotga tahdidlarni oldindan aniqlash, tahlil qilish va oldini olishda yordam beradi.

### **TI manbalari:**

- Dark web forumlar
- Xaker guruhlari faoliyati
- Malware tahlili
- Tashqi ijtimoiy tarmoqlar
- Xalqaro xavfsizlik hamjamiyatlari

### **TI turlari:**

- **Strategik** – Boshqaruv darajasida qarorlar qabul qilish uchun (masalan, davlat miqyosidagi tahdidlar).
- **Taktik** – Hujumchilarning odatdagi usullari (TTP – tactics, techniques, and procedures).
- **Operativ** – Hodisa vaqtida darhol kerakli ma’lumot (masalan, IP, hash, domen).
- **Texnik** – Aniq xakerlik vositalari va zaifliklar haqida.

### **Nega kerak?**

Tahdidlar haqidagi razvedka vositalari tashkilotni **hujumdan oldin ogohlantirish** imkonini beradi. Reaktiv himoya emas, **proaktiv himoya**ni amalga oshirish mumkin.

### **Real hayotdagi misol:**

TI orqali tashkilot xakerlar ma'lum IP manzillardan skanerlash qilayotganini oldindan bilib oladi va ushbu IP’larni bloklaydi.

---

# 🌐 3. External Attack Surface Management (EASM)

### **Ta’rif:**

EASM — bu tashqi yuzadagi (ya’ni internet orqali ochiq bo‘lgan) IT aktivlarni aniqlash, monitoring qilish va zaifliklardan himoya qilish uchun xizmat qiladigan platforma yoki xizmat.

### **Nimalarni nazorat qiladi?**

- Domenlar va subdomenlar
- Ochiq portlar, API interfeyslar
- Veb serverlar, DNS yozuvlar
- Cloud xizmatlar (masalan: AWS, Azure’dagi ochiq resurslar)

### **Jarayon:**

1. **Aktivlarni aniqlash** – Tashkilot egasi bo‘lgan barcha IT resurslar ro‘yxatga olinadi.  
2. **Xavflarni aniqlash** – Noto‘g‘ri sozlangan, zaif yoki ochiq bo‘lganlar ajratiladi.  
3. **Reyting berish** – Qaysi aktiv eng xavfli ekanligi aniqlanadi.  
4. **Hisobot va monitoring** – Doimiy ravishda tahlil qilinadi.

### **Nega kerak?**

Ko‘pincha tashkilot o‘zining qaysi aktivlari internetga ochiq ekani haqida to‘liq bilmaydi. EASM buni avtomatik aniqlaydi.

### **Real misol:**

Tashkilotning eski subdomeni ishlamaydi, lekin hanuzgacha internetga ochiq. Hacker bu subdomen orqali _subdomain takeover_ qilishi mumkin.

---

# 📢 4. Awareness – Kiberxavfsizlik bo‘yicha xabardorlik

### **Ta’rif:**

Awareness — bu xodimlarning **kiberxavfsizlik xatarlarini tushunishi va ularga qanday munosabatda bo‘lishini** shakllantirishga qaratilgan ta’limiy va madaniy faoliyatlar majmuasi.

### **Asosiy yo‘nalishlar:**

- Phishing va social engineering haqida treninglar  
- Parol siyosati bo‘yicha ko‘rsatmalar  
- USB xavfsizligi va mobil qurilma gigiyenasi  
- Real hodisalarga asoslangan mashg‘ulotlar (gamification)

### **Nega kerak?**

80% dan ortiq muvaffaqiyatli kiberhujumlar **xodimlar xatolari** tufayli sodir bo‘ladi (havolaga bosish, zaif parol, maxfiy ma’lumotni oshkor qilish).

### **Foydalari:**

✅ Xodimlar hushyor va mas’uliyatli bo‘ladi  
✅ Oson tuzilgan hujumlar (phishing) muvaffaqiyatsiz bo‘ladi  
✅ Kiberxavfsizlik tashkilot madaniyatiga aylanadi

---

# ⚙️ 5. Security Orchestration, Automation and Response (SOAR)

### **Ta’rif:**

SOAR — bu turli xavfsizlik tizimlarini **birlashtiradigan (orchestration), avtomatlashtiradigan (automation)** va hodisalarga **tez javob beradigan (response)** kompleks tizimdir.

### **SOAR qanday ishlaydi:**

1. **Hodisa aniqlanadi** (masalan, SIEM dan signal keladi).  
2. **SOAR avtomatik tekshiradi** (IP qora ro‘yxatda bormi, bu xatti-harakat odatiymi).  
3. **Jarayon boshlanadi** (foydalanuvchini bloklash, karantin, alert yuborish).  
4. **Hodisa bo‘yicha hisobot tayyorlanadi.**

### **Imkoniyatlari:**

- SIEM, EDR, Firewall, TI kabi vositalarni yagona platformaga birlashtiradi  
- Reaksiyani inson aralashuvsiz avtomatlashtiradi  
- Xodimlarning ishini kamaytiradi, tezlikni oshiradi

### **Real hayotdagi misol:**

Firewall notanish IP'dan ko‘p urinish bo‘lganini aniqlaydi → SOAR bu IP’ni SIEM orqali tekshiradi → xavfli deb topiladi → avtomatik ravishda ushbu IP bloklanadi va administratorga xabar yuboriladi.

---

# 🔚 Xulosa

| Texnologiya | Maqsadi | Asosiy foydasi |
|------------|---------|----------------|
| **EDR** | Qurilmalarda tahdidlarni aniqlash va javob berish | Qurilma darajasidagi himoya |
| **TI** | Tahdidlar haqida razvedka | Proaktiv xavfsizlik |
| **EASM** | Tashqi aktivlarni boshqarish | Ochiq yuzalarni yopish |
| **Awareness** | Xodimlarni o‘qitish | Inson xatolarini kamaytirish |
| **SOAR** | Xavfsizlik jarayonlarini avtomatlashtirish | Tezlik va integratsiya |
