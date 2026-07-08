CAVE DUEL
=========
Kose widget'i olarak tasarlanan mini dovus oyunu.
Oyun tamamen HTML'e gomulu (base64); assets/ klasoru kaynak dosyalardir.

DOSYALAR
  1.html  -> UI 1: yakin plan (seffaf arka plan: duvar kagidi gorunur,
             sadece yildizlar + zemin; golgesiz sprite)
  2.html  -> UI 2: genis dunya - gokyuzu/dag manzarasi acilir (golgesiz)
  3.html  -> UI 3: ana oyun - can bari, bolum adi, envanter, skiller;
             golgeli sprite'lar
  index.html -> eski tek dosya prototip (arsiv)

KARAKTERLER (CC0 - projenin kendi "Pixel Hero Maker" ureteciyle olusturuldu)
  Kahraman: Soldier
  Dusmanlar: ORK (yesil) / KIZIL ORK / GOLGE ORK (hizli) / ALTIN ORK (tank, 2x coin)
  Kizil-golge-altin varyantlari palet kaydirmayla uretildi
  (assets/karakterler/orc-varyantlar/).
  Karakterler ayak satirina gore zemine basar (golge referans degildir).

OYUN AKISI
  Dusmani oldur -> kahraman kosar, arazi + dag paralaks akar ->
  ileride sabit bekleyen dusmana ulasinca savas baslar.

KAYIT
  localStorage "caveDuelSave": coin, bolum, esyalar. 3 dosya ortak.

ASSETS/
  arkaplan/     arazi.png (zemin, loop) + arka plan araazi.png (dag, paralaks)
  karakterler/  soldier/, orc/, orc-varyantlar/
  ikonlar/      silah ikonlari + coin (0x72, sadece menu ikonu)

KONTROLLER (masaustu test)
  Bosluk/Sag ok = saldiri, Sol ok/Shift = kalkan. Telefonda otomatik.
