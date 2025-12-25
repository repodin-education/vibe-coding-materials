# Vibe Coding 2026 - Testimääreet ja Testausohjeet

## 📊 Testimääreet Kurssille

### 1. **Submission-Testauksen Kriteerit**

#### Beginner Level
- ✅ Yksinkertainen ratkaisu perusvaatimuksille
- ✅ Lähdekoodi toimii ongelmitta
- ✅ Selkeä ja luettava koodi
- ✅ Dokumentaatio on olemassa
- ⏱️ Completion time: 30-45 minuuttia

#### Intermediate Level
- ✅ Normaalitason ratkaisu kaikille vaatimuksille
- ✅ Hyvä koodin laatu ja rakenne
- ✅ Perusvirheenkäsittely
- ✅ Selkeä README ja kommentit
- ⏱️ Completion time: 1-2 tuntia

#### Advanced Level
- ✅ Monipuolinen ratkaisu + ekstravaiheet
- ✅ Korkealaatuinen koodi (DRY, SOLID periaatteet)
- ✅ Kattava virheenkäsittely
- ✅ Yksityiskohtainen dokumentaatio
- ✅ Testit (unit/integration)
- ⏱️ Completion time: 2-3 tuntia

### 2. **Koodin Laadun Mittarit**

| Kriteeri | Tarkistus |
|----------|-----------|
| **Readability** | Koodi on helppolukuista ja hyvin nimetty |
| **DRY (Don't Repeat Yourself)** | Ei toistuvia koodilohkoja |
| **Error Handling** | Virheet käsitellään asianmukaisesti |
| **Testing** | Unit-testit tai integration-testit mukana |
| **Documentation** | README ja inline-kommentit |

### 3. **Performance Benchmarks**

```javascript
// Testidata koko
- Small: 10 items
- Medium: 100 items
- Large: 1000+ items

// Hyväksyttävät suoritusajat
- Small: < 100ms
- Medium: < 500ms
- Large: < 2000ms
```

### 4. **Opiskelijapalaute-Mittarit**

Kerää palautetta näistä:
- 📚 Kurssin sisällön selkeys (1-5)
- 💡 Assignment-vaikeusaste (1-5)
- ⏰ Arvioitu aika vs todellinen aika
- 🆘 Tarvitaanko enemmän resursseja/vihjeitä
- ✨ Mitä oli hyödyllistä
- 🐛 Mitkä asiat olivat epäselviä

### 5. **Kurssin Kehitysmetriikka**

Seuraa näitä numeroita:
- % Opiskelijoista jotka palauttavat ajoissa
- Keskimääräinen submission-pisteet
- Palaute-palautusprosentti
- Assignment-epäonnistumisprosentti
- Yhteydenottojen määrä tukipyyntöjen kanssa

## 🧪 Testausstrategia

### Paikallinen Testaus

```bash
# 1. Kloonaa assignment-template
git clone https://github.com/artomatilainen/vibe-coding-2026-assignment-1 test-submission

# 2. Testaa beginner-versio
npm install
npm test  # Tai npm run check

# 3. Testaa intermediate-versio
# (korvaa ratkaisun)
npm test

# 4. Testaa advanced-versio
npm test

# 5. Testaa feedback-mekanismi
git push # Triggeroida GitHub Actions
```

### Automaattinen Testaus

Käytä GitHub Actions:
```yaml
- npm ci
- npm run lint
- npm test
- npm run type-check
```

## 📈 Seurannan Dashboard

Luodaan GitHub Projects board:
- **Backlog**: Uudet assignment-ideat
- **In Progress**: Nykyiset assignment-viikot
- **Testing**: Testataan uusia assignmentteja
- **Done**: Valmistuneet viikot
- **Feedback**: Opiskelijapalauteet

## 🎯 Tavoitteet Jokaiselle Assignmentille

Jokaiselle assignmentille aseta:
- 🎓 Learning outcomes
- ⏱️ Expected completion time
- 📊 Difficulty level (1-5)
- 🔗 Prerequisites
- 📚 Recommended resources

---

**Päivitetty**: 2025-12-24
**Versio**: 1.0
