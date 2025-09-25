# Sprint4
Machine Learning Trainning - Sprint 4. In this project, you will be performing a multimodal classification task for e-Commerce product categorization.  Learning about computer vision and NLP: CNNs, image embeddings, tokenization, vectorization, word embeddings.


 `mermaid
  graph TD
      subgraph "Clientes"
          Browser["🌐 Navegador Web"]
          Scheduler["⏰ Programador de Tareas"]
      end

      subgraph "Capa de Presentación (UI)"
          WebApp["UMM.AutoEd.UI.Web"]
          WinService["UMM.AutoEd.UI.WinService"]
      end

      subgraph "Capa de Negocio (Business)"
          BusinessAnticipos["Módulo de Anticipos"]
          BusinessLiquidaciones["Módulo de Liquidaciones"]
          BusinessCatalogos["Módulo de Catálogos"]
          BusinessOtros["... otros módulos"]
      end

      subgraph "Capa Central (Core)"
          Core["Binaries/MPM.Core"]
          DataAccess["- DataAccess (SQL/MySQL)"]
          Logging["- Logging"]
          Encrypt["- Encrypt"]
          Core --> DataAccess & Logging & Encrypt
      end

      subgraph "Capa de Datos"
          Model["Model (Entidades, DTOs)"]
          Database["🗄️ Base de Datos (SQL)"]
      end

      %% Conexiones
      Browser --> WebApp
      Scheduler --> WinService

      WebApp --> BusinessAnticipos & BusinessLiquidaciones & BusinessCatalogos & BusinessOtros
      WinService --> BusinessAnticipos & BusinessLiquidaciones & BusinessCatalogos & BusinessOtros

      BusinessAnticipos & BusinessLiquidaciones & BusinessCatalogos & BusinessOtros --> Core

      Core --> Model
      DataAccess --> Database
  `
