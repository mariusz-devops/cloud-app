# ☁️ Cloud Task Manager - Książka "Azure w Praktyce"
**Autor: Mariusz Dworniczak**

Projekt nowoczesnej, natywnej aplikacji chmurowej (Cloud-Native) zrealizowany w pełnej architekturze 3-warstwowej z wykorzystaniem najlepszych praktyk DevOps oraz bezpieczeństwa chmurowego.

---

## 🏗️ Architektura Systemu (Azure Mapping)

Aplikacja została w pełni zmigrowana z kontenerów lokalnych do usług klasy PaaS (Platform as a Service) w chmurze Azure, co zapewnia wysoką dostępność, skalowalność i bezpieczeństwo klasy korporacyjnej.

| Warstwa | Technologia | Usługa Azure |
| :--- | :--- | :--- |
| **Presentation** | React 19 + Vite | Azure App Service (Static Host) |
| **Application** | .NET 9 Web API | Azure App Service |
| **Data** | Entity Framework Core | Azure SQL Database (Serverless) |
| **Security** | Managed Identity | Azure Key Vault |
| **Automation** | GitHub Actions | CI/CD Pipelines |

---

## 🚦 Status Projektu i Artefakty

* [x] **Artefakt 1:** Architektura i struktura folderów (Diagram C4).
* [x] **Artefakt 2:** Środowisko wielokontenerowe uruchomione lokalnie (Docker Compose).
* [x] **Artefakt 3:** Działająca warstwa prezentacji (React + Vite).
* [x] **Artefakt 4:** Działająca warstwa logiki backendu (.NET 9).
* [x] **Artefakt 5:** Trwałość danych i profesjonalny kontrakt API (EF Migrations + DTO).
* [x] **Artefakt 6:** Aplikacja przemigrowana do Azure (App Services).
* [x] **Artefakt 7:** Pełna integracja z chmurą: Tożsamość Zarządzana (Managed Identity) i Magazyn Kluczy (Key Vault).
* [x] **Artefakt 8:** Dokumentacja techniczna API (Swagger UI) dostępna publicznie.

---

## 🚀 Adresy Projektu (Live Demo)

Aplikacja została wdrożona w regionie **Germany West Central**. Możesz przetestować jej działanie pod poniższymi linkami:

* **🌐 Interfejs Użytkownika (Frontend):** [Uruchom Aplikację](https://www.cloud-task-manager-frontend-dtdme9ekavhpfegg.germanywestcentral-01.azurewebsites.net)

* **📖 Dokumentacja API (Swagger):** [Przeglądaj API](https://cloud-task-manager-api-h9fsfpd4gnaeaddz.germanywestcentral-01.azurewebsites.net/swagger)

---

## 🛡️ Bezpieczeństwo i DevOps

Projekt implementuje model **Zero Trust** poprzez:
1.  **Azure Key Vault**: Brak haseł i connection stringów w kodzie źródłowym.
2.  **Managed Identity**: Backend komunikuje się z bazą danych i magazynem kluczy bez użycia poświadczeń tekstowych.
3.  **CI/CD**: Każdy `git push` wyzwala automatyczne testy i wdrożenie na środowisko produkcyjne Azure.

> **Informacja:** Ten plik stanowi integralną część materiałów edukacyjnych książki "Azure w Praktyce". Jest dowodem na poprawną implementację pełnego cyklu życia aplikacji chmurowej.