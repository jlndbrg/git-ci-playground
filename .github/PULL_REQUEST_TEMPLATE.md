## PR-titel
*OBS! PR-titeln används för automatgenererade releasenotes.* 

Följ **Conventional Commits**-formatet för PR-titeln:

```
<type>: <kort beskrivning>
```

### Där:
- **type**: Välj en av följande:
  - `feat`: Ny funktion
  - `fix`: Buggfix
  - `docs`: Dokumentationsändring
  - `style`: Kodstil/formatering
  - `refactor`: Omstrukturering utan att ändra funktionalitet
  - `perf`: Prestandaförbättring
  - `test`: Lägga till/uppdatera tester
  - `chore`: Bygg- eller verktygsändringar
  - `revert`: Återställer en tidigare commit

### Exempel:
- `feat: Lägg till OAuth2-autentisering`
- `fix: Justera felaktig CSS i header`
- `refactor!: Uppdatera autentiseringslogik` (Breaking Change)
- `perf!: Ändra databasstruktur för optimering` (Breaking Change)

---

## Beskrivning

### Sammanfattning
Förklara varför ändringen behövs och sammanfatta vad som ändrats.

---

### Hur ska ändringen testas?

---

## Relaterade ärenden
Länka eventuella relaterade ärenden (t.ex. `Fixar #123`).
