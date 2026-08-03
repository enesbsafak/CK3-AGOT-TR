# AGOT Türkçe Çeviri — Terim Sözlüğü ve Çeviri Kuralları

> Bu dosya çevirinin anayasasıdır. Çevrilen her anahtar bu kurallara uyar.
> Değişiklik yalnızca ortak kararla ve bu dosyaya işlenerek yapılır.

---

## 1. DOKUNULMAYACAKLAR (Kesin Kurallar)

Aşağıdaki kategoriler **asla çevrilmez**, olduğu gibi korunur:

| Kategori | Örnekler |
|---|---|
| Kişi adları | Ned, Jon, Daenerys, Tyrion, Ramsay |
| Soyadları/Haneleri | Stark, Lannister, Targaryen, Bolton |
| Ejderha adları | Drogon, Balerion, Meraxes |
| Gemi adları | Sea Breeze, The Iron Vengeance |
| Şehir/Kale adları | Winterfell, King's Landing, Highgarden, The Wall |
| Bölge adları | Westeros, Essos, The North, The Reach |
| Hanelerin unvan/ünvan ekleri | House Stark, Lord of Winterfell (kalıp içinde isim kısmı) |
| Unvan ön adları | Ser, Maester (isimle birlikte), King/Queen (isimle birlikte) |
| Kitap/şarkı/yemin alıntıları | "Winter is Coming", "Hear Me Roar!" (yeminlerin tamamı kalıp olarak korunur veya ortak kararla çevrilir — bkz. §3) |
| Karakter selamındaki isimler | [CHARACTER.GetFirstName] gibi değişkenlerle gelenler |

**Kural:** Bir şeyin çevrilip çevrilmeyeceğine şüphe varsa **çevrilmez**. Karar defterine (§7) yazılır.

---

## 2. SABİT ÇEVİRİLER (Evren Terminolojisi)

Bunlar her durumda aynı karşılıkla çevrilir. (Kaynak: Epsilon Yayınları resmi Türkçe çevirisi — çevirmen Sibel Alaş.)

| İngilizce | Türkçe | Not |
|---|---|---|
| dragon | ejderha | her zaman tekil/çoğul uyumlu |
| dragonrider | ejderha binicisi | |
| The Hand of the King | Kralın Eli | |
| Kingsguard | Kral Muhafızları | |
| Lord Commander | Lord Kumandan | |
| Small Council | Küçük Konsey | |
| Maester | Üstat | |
| Archmaester | Baş Üstat | |
| The Citadel | Kale | |
| Warden of the North | Kuzey'in Koruyucusu | |
| Night's Watch | Gece Nöbetçileri | resmi çeviride "Yeminli Gece Nöbetçileri Kardeşliği" |
| The Wall | Sur | |
| Beyond the Wall | Sur'un Ötesi | |
| Wildling / Free Folk | Yabanıl / Özgür Halk | |
| The Others | Ak Gezenler | |
| Ironborn | Demirdoğanlar | |
| First Men | İlk İnsanlar | |
| Andals | Andallar | |
| Valyrian Steel | Valyria Çeliği | |
| Faith of the Seven | Yedilerin İnancı | |
| The Seven | Yediler | |
| Iron Throne | Demir Taht | |
| Seven Kingdoms | Yedi Krallık | |
| King in the North | Kuzey Kralı | |
| King's Landing | Kralın Şehri | resmi çeviride çevrilmiş |
| Iron Islands | Demir Adalar | |
| direwolf | ulukurt | resmi çeviri karşılığı |
| Children of the Forest | Ormanın Çocukları | |
| Night King | Gece Kralı | |
| Winter is Coming | Kış Geliyor | |
| Hear Me Roar | Kükrememi Duysunlar | |
| First Sword of Braavos | Braavos'un Birinci Kılıcı | |
| Faceless Men | Yüzsüz Adamlar | |
| Doom of Valyria | Valyria'nın Çöküşü | |
| Long Night | Uzun Gece | |
| Age of Heroes | Kahramanlar Çağı | |
| Master of Coin / Laws / Whisperers | Hazine / Adalet / Fısıltı Sorumlusu | tek tablo kararı |
| Lord | Lord (korunur) | resmi çeviride "Lord Eddard Stark" |
| Ser | Ser (korunur) | |

---

## 3. ÜSLUP KURALLARI (Makine Çevirisi Hissi Karşıtı)

1. **Cümle doğallığı:** İngilizce cümle yapısı birebir kopyalanmaz. Türkçe cümle dizilişi (özne-nesne-yüklem, devrik serbest) kullanılır. Örn. "You have proven yourself worthy" → "Kendini kanıtladın" değil, bağlama göre "Kendini kanıtlamış oldun" gibi doğal karşılık.
2. **Resmiyet/İçtenlik:** Orta Çağ saray dili. "Sen" yerine resmi hitaplarda "siz" (Strategyturk ile tutarlı). Modern deyim, argo, çağ dışı kavram **yasak** ("okey", "cool", "mükemmel ötesi" gibi).
3. **Duygusal yoğunluk:** Olay metinlerinde karakterin ruh hali korunur (hüzün, öfke, gizem). Kelimesi kelimesine değil, **duygu** çevrilir.
4. **Tekrarlar:** Aynı kavram her yerde aynı kelimeyle çevrilir (tutarlılık). §2'deki tablo buna güvence sağlar.
5. **Büyük/küçük harf:** Unvanlar ve özel adlar büyük harfle (Kralın Eli, Kuzey), cins isimler küçük (ejderha, kale).
6. **Türkçe imla:** Kesme işareti doğru (Stark'ın, Kuzey'in, Demir Taht'ın). Kuralsız İngilizce apostrof kullanılmaz.
7. **Strategyturk uyumu:** Aynı kavramın Strategyturk'te yerleşik çevirisi varsa (trait, konsept, GUI) **o kullanılır** — oyunda iki farklı karşılık çıkmaz.

---

## 4. TEKNİK KURALLAR (Asla Bozulmaz)

- **Anahtarlar** değişmez: `agot_scenario_ats.1000.t` aynen kalır.
- **Değişkenler** değişmez: `$VAR$`, `[CHARACTER.GetName]`, `[GetXxx]` — hem adı hem söz dizimi.
- **Konsept bağları** değişmez: `[Concept('war','Savaş')|E]` → içindeki `'war'` anahtarı AYNEN kalır, görünen ad Türkçe olur.
- **Format kodları** korunur: `#V ... #!`, `#high ... #!`, `\n`, `\t`, `$EFFECT_LIST_BULLET$`.
- **Tırnak/versiyon soneki** korunur: `:0 "..."` biçimi değişmez.
- **Çoğul/tekil uyumu** korunur: `$COUNT|V$` gibi değişkenlerle Türkçe uyum kontrol edilir.

---

## 5. İSİM DOSYALARI İÇİN ÖZEL KURALLAR

- `character_names`, `dynasty_names`, `house_names`: **çevrilmez, korunur.** (TODO etiketi "dokunulmaz" kararıyla düşer.)
- Takma adlar (nickname): anlamlıysa çevrilir (The Fat → Şişman), isimle bütünleşmişse korunur (Jon the Wandering — karar defteri).
- Mottolar (sözler): çevrilir — ama üslup kuralı 1-7'ye tabi, kalıp bozulmaz.
- Tarihi isimlerin Türkçe yazımı varsa ortak kararla deftere işlenir (ör. Viserys → Viserys).

---

## 6. ÇEVİRİ İŞ AKIŞI

1. **Kısa metinler önce** (GUI, unvan, modifier) → sonra uzun anlatılar (olaylar).
2. Her kategori için: ben önce karar defterine uygun **taslak** üretirim → sen gözden geçirirsin → onaylanan commit olur.
3. Şüpheli her karar §7'ye işlenir — çeviri bir daha geri dönüp düzeltilmez.
4. `### TODO` etiketi ancak **insan onayından** geçen anahtarda kalkar. (Dokunulmaz kategorisi hariç — orada etiket "DOKUNULMAZ" kararıyla kalkar.)

---

## 7. KARAR DEFTERİ

| Tarih | Anahtar/Dosya | Karar | Gerekçe | Onaylayan |
|---|---|---|---|---|
| 2026-08-03 | Yer adları (Winterfell vb.) | Korunur | Resmi Türkçe çeviride Winterfell aynen | enesbsafak |
| 2026-08-03 | King's Landing | Kralın Şehri | Resmi Türkçe çeviri | enesbsafak |
| 2026-08-03 | Lord / Ser | Korunur | Resmi Türkçe çeviri | enesbsafak |
| 2026-08-03 | Yeminler (Winter is Coming) | Çevrilir: "Kış Geliyor" | Resmi Türkçe çeviri | enesbsafak |
| 2026-08-03 | The Others / direwolf / Night's Watch | Ak Gezenler / ulukurt / Gece Nöbetçileri | Resmi Türkçe çeviri | enesbsafak |

---

## 8. ONAYLANAN AÇIK SORULAR (Resmi Türkçe çeviri — Epsilon/Sibel Alaş esas alındı)

1. **Yer adları:** Resmi çeviri karışık kullanıyor → aynısını yapacağız:
   - **Winterfell, Highgarden, Casterly Rock gibi kaleler: korunur** (resmi çeviride Winterfell aynen)
   - **King's Landing → Kralın Şehri** (resmi çeviride çevrilmiş)
   - **Iron Islands → Demir Adalar**, **The North → Kuzey**, **The Reach → Erişim değil, korunur/bölge adı olarak "Reach"→ karar defteri**
2. **Yeminler:** Çevrilir ("Winter is Coming" → "Kış Geliyor").
3. **Lord:** Korunur ("Lord Eddard Stark" — resmi çeviri).
4. **Ser:** Aynen korunur.
5. **Dini terimler:** §2 tablosundaki gibi onaylandı.

> Bu kararlar resmi kitap çevirisinden alınmıştır; oyundaki isimlerle çelişirse
> (ör. modda "The Reach" bölgesi) karar defterine işlenir, çeviri buna göre yürür.
