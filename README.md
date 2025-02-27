# Semantic Release Configuration

Det här projektet använder **Semantic Release** för att automatisera versionshantering, changelog-generering och releaser baserat på commit-meddelanden som följer **Conventional Commits**-standarden.

---

## 📋 Commit-meddelanden och Versionering

Semantic Release analyserar commit-meddelanden för att avgöra vilken typ av versionbump som ska göras (major, minor, eller patch). Nedan visas vilka commit-typer som påverkar versioneringen:

### **Commit-typer och deras effekter**
| Commit Typ    | Versionbump      | Beskrivning                                      |
|---------------|------------------|--------------------------------------------------|
| `feat`        | **Minor**        | Nya funktioner som inte bryter bakåtkompatibilitet. |
| `fix`         | **Patch**        | Bugfixar som inte bryter bakåtkompatibilitet.   |
| `docs`        | **Patch**        | Uppdateringar av dokumentation.                |
| `style`       | **Patch**        | Kodstil, formatförändringar utan påverkan på funktion. |
| `refactor`    | **Patch**        | Kodförbättringar utan påverkan på funktionalitet. |
| `perf`        | **Patch**        | Förbättringar som påverkar prestanda.          |
| `test`        | **Patch**        | Lägga till eller uppdatera tester.             |
| `chore`       | _Ingen bump_     | Ändringar i byggprocess eller verktyg som inte påverkar kod. |
| `build`       | _Ingen bump_     | Förändringar i byggprocessen.                  |
| `ci`          | _Ingen bump_     | Ändringar i CI/CD pipelines.                   |

feat och fix är det centrala.

### **Breaking Changes**
Breaking changes kan anges genom
"BREAKING CHANGE" i footern på commit meddelandet d v s 

"feat: En feature som utvecklats

BREAKING CHANGE: Förändringen som bryter bakåtkompabiliteten"

