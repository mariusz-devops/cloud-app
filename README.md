# Cloud Task Manager (2026)

Projekt natywnej aplikacji chmurowej realizowany w architekturze 3-warstwowej. 

## Deklaracja Architektury (Mapowanie Azure)
Ten projekt został zaplanowany z myślą o usługach PaaS (Platform as a Service) w regionie **Poland Central**.

| Warstwa | Komponent Lokalny | Usługa Azure |
| :--- | :--- | :--- |
| **Presentation** | React 19 (Vite) | Azure Static Web Apps |
| **Application** | API (.NET 9 / Node 24) | Azure App Service |
| **Data** | SQL Server (Dev) | Azure SQL Database (Serverless) |

## 🚦 Status Projektu
* [x] **Artefakt 1:** Architektura i struktura folderów (Diagram C4).
* [x] **Artefakt 2:** Środowisko wielokontenerowe uruchomione lokalnie (Docker Compose).
* [x] **Artefakt 3:** Działająca warstwa prezentacji (React + Vite w Dockerze).

### 📝 Podsumowanie etapu
Trzeci artefakt został osiągnięty. Nasza architektura przestała być jedynie statycznym schematem – stała się funkcjonalnym, odizolowanym systemem. Front-end jest gotowy, skonteneryzowany i poprawnie serwowany przez Nginx na porcie 8080.

> **Informacja:** Ten plik będzie ewoluował. W kolejnych etapach dodamy tutaj sekcje 'Quick Start', opis zmiennych środowiskowych oraz instrukcję wdrożenia (CI/CD).