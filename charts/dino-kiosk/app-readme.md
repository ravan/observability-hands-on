## Introduction


This application is a fully integrated, Kubernetes-based system designed to bring custom dinosaur models to life through a seamless digital-to-physical workflow. By leveraging microservices across two clusters—**Prod** and **Kiosk**—the system allows users to design, order, and produce 3D-printed dinosaur models.

Users interact with the system through a **Frontend** interface that communicates with a specialized **Build-a-Dino** service, where custom designs are generated using an **AI Model** service. Once a design is finalized, the **Printing Service** manages the printing workflow, utilizing a **Printing Queue** to handle print job organization. Finally, the **3D Printer** service brings these designs to life, completing the process.

This modular architecture enables flexibility, scalability, and observability, allowing for real-time monitoring and management of each stage in the design-to-production pipeline. With integrated OpenTelemetry and stress simulation features, the application also provides valuable insights into service performance and reliability.

