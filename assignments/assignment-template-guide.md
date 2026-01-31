# Vibe Coding Assignment-Template Rakenne ja Dokumentaatio

## 📁 Assignment-Template Hakemistorakenne

```
vibe-coding-assignment-[N]/
├── README.md                 # Assignment kuvaus ja ohjeet
├── GETTING_STARTED.md        # Pika-opas
├── HINTS.md                  # Vinkit (valinnainen)
├── package.json              # Riippuvuudet ja skriptit
├── package-lock.json
├── .eslintrc.json            # Koodin standardit
├── .gitignore
├── tsconfig.json             # TypeScript config (jos käytössä)
│
├── src/                       # Lähdekoodi
│   ├── index.ts              # Main entry point
│   ├── types/                # TypeScript types
│   │   └── index.ts
│   └── utils/                # Helper functions
│       └── index.ts
│
├── tests/                     # Testit
│   ├── unit/                 # Unit tests
│   │   └── solution.test.ts
│   └── integration/          # Integration tests
│       └── e2e.test.ts
│
├── examples/                  # Esimerkit
│   ├── basic.ts              # Perusesimerkki
│   ├── intermediate.ts       # Välimerkkiesimerkki
│   └── advanced.ts           # Edistynyt esimerkki
│
├── .github/
│   └── workflows/
│       ├── test.yml          # Automaattinen testaus
│       └── lint.yml          # Koodin tarkistus
│
└── docs/                      # Dokumentaatio
    ├── API.md                # API dokumentaatio
    ├── TESTING.md            # Ohjeet testaukseen
    └── TROUBLESHOOTING.md    # Yleisiä ongelmia
```

## 📋 README.md Rakenne

```markdown
# Assignment [N]: [Nimi]

## 📚 Kuvaus
[1-3 lauseen kuvaus assignmentista]

## 🎯 Learning Outcomes
- [ ] Outcome 1
- [ ] Outcome 2
- [ ] Outcome 3

## ⏱️ Aikataulu
- Expected: 1-2 hours
- Difficulty: ★★★☆☆ (3/5)

## 📋 Vaatimukset

### Perusvaatimukset (75%)
- [ ] Requirement 1
- [ ] Requirement 2
- [ ] Requirement 3

### Bonusvaatimukset (25%)
- [ ] Extra feature 1
- [ ] Extra feature 2

## 🚀 Aloittaminen
[Step-by-step instructions]

## ✅ Testaus
[How to run tests]

## 📚 Resurssit
- [Link 1](url)
- [Link 2](url)

## 💬 Apua?
[Contact information]

## ✨ Hyväksymisperusteet
[Clear acceptance criteria]
```

## 🔍 package.json Rakenne

```json
{
  "name": "vibe-coding-assignment-1",
  "version": "1.0.0",
  "description": "Assignment 1 - Vibe Coding 2026",
  "main": "src/index.ts",
  "scripts": {
    "start": "node src/index.js",
    "dev": "ts-node src/index.ts",
    "test": "jest",
    "test:watch": "jest --watch",
    "test:coverage": "jest --coverage",
    "lint": "eslint src --fix",
    "type-check": "tsc --noEmit",
    "check": "npm run lint && npm run type-check && npm test"
  },
  "dependencies": {},
  "devDependencies": {
    "@types/jest": "^29.0.0",
    "@types/node": "^20.0.0",
    "eslint": "^8.0.0",
    "jest": "^29.0.0",
    "ts-node": "^10.0.0",
    "typescript": "^5.0.0"
  },
  "keywords": ["vibe-coding", "learning"],
  "author": "Vibe Coding Team",
  "license": "MIT"
}
```

## 🧪 Testien Rakenne

### Unit Tests (src/tests/unit/solution.test.ts)

```typescript
describe('Assignment 1 - Solution', () => {
  describe('Basic Requirements', () => {
    test('should handle basic input', () => {
      // Arrange
      const input = 'test';

      // Act
      const result = myFunction(input);

      // Assert
      expect(result).toBeDefined();
    });
  });

  describe('Edge Cases', () => {
    test('should handle empty input', () => {
      expect(myFunction('')).toBeDefined();
    });

    test('should handle null/undefined', () => {
      expect(myFunction(null)).toThrow();
    });
  });

  describe('Performance', () => {
    test('should complete within time limit', () => {
      const start = performance.now();
      myFunction(largeData);
      const end = performance.now();

      expect(end - start).toBeLessThan(500); // ms
    });
  });
});
```

## 📊 Grading Rubric Esimerkki

| Kriteeri | 1 Piste | 2 Pistettä | 3 Pistettä |
|----------|---------|-----------|-----------|
| **Functionality** | Ei toimi | Osittain toimii | Täydellisesti toimii |
| **Code Quality** | Sekava | Hyvä | Erinomainen |
| **Testing** | Ei testejä | Perintestejä | Kattavat testit |
| **Documentation** | Puuttuu | Osittainen | Kattava |

## 🔄 GitHub Actions Workflow Esimerkki

```yaml
name: Test Assignment

on: [push, pull_request]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Lint
        run: npm run lint

      - name: Type check
        run: npm run type-check

      - name: Run tests
        run: npm test -- --coverage

      - name: Upload coverage
        uses: codecov/codecov-action@v3
```

## 📝 GETTING_STARTED.md Esimerkki

```markdown
# Getting Started

## Vaatimukset
- Node.js 20+
- npm 10+

## Asennus

1. Kloonaa repository:
   \`\`\`bash
   git clone <url>
   cd assignment-folder
   \`\`\`

2. Asenna riippuvuudet:
   \`\`\`bash
   npm install
   \`\`\`

3. Käynnistä kehitysympäristö:
   \`\`\`bash
   npm run dev
   \`\`\`

4. Testaa:
   \`\`\`bash
   npm test
   \`\`\`

## Kansioiden Käyttötarkoitus

- **src/**: Sinun koodisi menee tähän
- **tests/**: Testit tarkistavat ratkaisusi
- **examples/**: Referenssiratkaisuja ja ideoita
- **docs/**: Apumateriaaleja ja ohjeita
```

## 💡 HINTS.md Rakenne

```markdown
# Vinkit Assignment 1

## Idea puuttuu?
Katso nämä ensin:
- [Konsepti 1](linkki)
- [Konsepti 2](linkki)

## Jumittunut kohdassa X?
Yritä:
1. Lue virheilmoitus huolellisesti
2. Tarkista Types-dokumentaatio
3. Katso examples/-kansion koodia
4. Testit antavat vihjeitä

## Yleiset ongelmat

### "Module not found"
```bash
npm install  # Asenna puuttuvat paketit
```

### "Test fails"
```bash
npm test -- --verbose  # Yksityiskohtaisempi tulostus
```

## Resursseista apua
[Linkit perusmateriaaleihin]

## Edelleen apua?
[Kontaktitiedot]
```

## 🎯 Assignment Progression Esimerkki

```
Viikko 1-2: Assignment 1 (Perus JavaScript)
├── Opitaan: Variables, functions, loops
├── Palaute: Code review + tests
└── Mittatikki: 80% opiskelijoista palauttaa

Viikko 3-4: Assignment 2 (Objects & Arrays)
├── Opitaan: Data structures, methods
├── Palaute: Peer review + automated tests
└── Mittatikki: 85% palauttaa, avg score 80/100

Viikko 5-6: Assignment 3 (Async & APIs)
├── Opitaan: Promises, async/await, fetch
├── Palaute: Code review + integration tests
└── Mittatikki: 90% palauttaa, avg score 85/100

Viikko 7-8: Pro Assignment (Koko projekti)
├── Opitaan: Kaikki yhdessä
├── Palaute: Detailed feedback + reflection
└── Mittatikki: 95% palauttaa, showcase best work
```

---

**Versio**: 1.0
**Päivitetty**: 2025-12-24
**Author**: Vibe Coding Team
