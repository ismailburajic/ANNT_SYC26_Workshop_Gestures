# 🤖 Radionica: Prepoznavanje gesti ruke pomoću umjetne inteligencije

Dobrodošli na radionicu!

Tokom ove radionice napravit ćemo vlastiti sistem koji može **prepoznati geste ruke pomoću web kamere**. Naučit ćemo kako računar "vidi" šaku, kako se prikupljaju podaci za treniranje modela i kako umjetna inteligencija uči razlikovati različite geste.

Na kraju radionice imat ćete aplikaciju koja u stvarnom vremenu prepoznaje geste koje ste sami naučili model.

---

# 🎯 Šta ćemo napraviti?

Na kraju radionice naš program će moći:

- 📷 prepoznati vašu šaku pomoću kamere,
- ✋ prepoznati različite geste,
- 🧠 koristiti istrenirani AI model za donošenje odluke,
- ⚡ raditi u stvarnom vremenu.

---

# 📚 Šta ćemo naučiti?

Kroz radionicu ćemo proći kroz nekoliko koraka:

## 1. Detekcija šake

Prvo ćemo koristiti **MediaPipe**, biblioteku koja može pronaći šaku na slici i označiti njene karakteristične tačke (landmarke).

Umjesto da AI posmatra cijelu sliku, koristit ćemo upravo te tačke.

---

## 2. Prikupljanje podataka

Zatim ćemo napraviti vlastiti skup podataka.

Za svaku gestu:

- kamera će prikazati odbrojavanje,
- napravit ćemo 30 uzoraka,
- podaci će se automatski sačuvati.

Na ovaj način sami kreiramo podatke na kojima će model učiti.

---

## 3. Treniranje modela

Nakon što prikupimo dovoljno uzoraka, pokrenut ćemo treniranje neuronske mreže.

Model će pokušati naučiti razliku između svih gesti koje smo prikupili.

---

## 4. Testiranje

Na kraju ćemo uključiti kameru i provjeriti koliko dobro model prepoznaje geste u stvarnom vremenu.

Ako pokažemo jednu od naučenih gesti, model će pokušati pogoditi o kojoj gesti se radi.

---

# 📁 Struktura projekta

```
Data_2/
    hello/
    thanks/
    iloveyou/

gestures.ipynb
gesture_model.h5
README.md
```

Najveći dio radionice odvijat će se u datoteci **gestures.ipynb**.

---

# ▶ Pokretanje projekta

Instalirajte potrebne biblioteke:

```bash
pip install tensorflow mediapipe opencv-python numpy matplotlib pandas scikit-learn
```

Nakon toga otvorite:

```
gestures.ipynb
```

i pokrećite ćelije redom od početka prema kraju.

---

# 💡 Kako izgleda cijeli proces?

```
Web kamera
      │
      ▼
Detekcija šake
      │
      ▼
Prikupljanje podataka
      │
      ▼
Treniranje AI modela
      │
      ▼
Prepoznavanje gesti
```

---

# 🚀 Izazov

Nakon što završite radionicu, pokušajte:

- dodati novu gestu,
- prikupiti vlastite podatke,
- ponovo istrenirati model,
- provjeriti može li AI prepoznati i novu gestu.

Na taj način ćete vidjeti kako se modeli umjetne inteligencije mogu prilagoditi različitim zadacima.

---

# 📖 Cilj radionice

Cilj ove radionice nije samo napraviti aplikaciju, nego razumjeti kako funkcioniše jedan jednostavan AI sistem.

Do kraja radionice znat ćete:

- kako računar prepoznaje šaku,
- šta su podaci za treniranje,
- kako funkcioniše neuronska mreža,
- kako AI donosi odluke na osnovu podataka koje smo prikupili.

Sretno i zabavite se istražujući svijet umjetne inteligencije! 🚀