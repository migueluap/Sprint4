# Sprint4
Machine Learning Trainning - Sprint 4. In this project, you will be performing a multimodal classification task for e-Commerce product categorization.  Learning about computer vision and NLP: CNNs, image embeddings, tokenization, vectorization, word embeddings.



## Diagrama de System Design: Arquitectura Monolítica

  Una arquitectura monolítica es un modelo de desarrollo de software tradicional en el que una aplicación se construye como una única unidad autónoma y unificada. Todos los componentes de
  la aplicación, como la interfaz de usuario, la lógica de negocio y las capas de acceso a datos, están estrechamente integrados en una única base de código y se implementan como un único
  archivo o servicio ejecutable.

  ### Componentes

     Cliente (Client):* Representa a los usuarios que interactúan con la aplicación a través de un navegador web, una aplicación móvil u otro dispositivo.
     Aplicación Monolítica (Monolithic Application):* Es el núcleo del sistema, un único bloque que contiene toda la funcionalidad. Se divide internamente en las siguientes capas:
         Interfaz de Usuario (User Interface):* Es la capa de presentación que maneja las interacciones del usuario y muestra la información.
         Lógica de Negocio (Business Logic):* Contiene las reglas y la lógica central de la aplicación.
         Capa de Acceso a Datos (Data Access Layer):* Gestiona la comunicación con la base de datos.
     Base de Datos (Database):* Es el único almacén de datos que comparte toda la aplicación.

  ### Diagrama (Mermaid)

  `mermaid
  graph TD
      subgraph "Cliente"
          A[Navegador Web]
          B[Aplicación Móvil]
      end


      subgraph "Aplicación Monolítica"
          C[Interfaz de Usuario]
          D[Lógica de Negocio]
          E[Capa de Acceso a Datos]
      end

      F[Base de Datos]


      A --> C
      B --> C
      C --> D
      D --> E
      E --> F
  `

  ### Cómo visualizarlo

  Puedes copiar y pegar este código en cualquier editor de Markdown o visor en línea que admita diagramas de Mermaid (como los visores de GitHub, GitLab o editores como Typora) para ver el
  gráfico renderizado.
