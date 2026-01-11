TaxCortex - Complete Technical Documentation & Architecture

📁 GitHub Repository Structure

![PHOTO-2026-01-11-13-32-21](https://github.com/user-attachments/assets/1f1315e6-b0f5-42e0-b493-394ac56042a6)


Detailed Repository Organization: The repository follows industry-standard monorepo architecture with clear separation of concerns. The docs/architecture/ directory contains all Data Flow Diagrams (DFDs) and system diagrams exported as PNG for hackathon submissions and technical reviews. src/backend/ houses the Flask Python API with business logic separated into tax_logic.py for testability. src/frontend/ contains production-optimized vanilla JavaScript with no framework dependencies. deployment/ provides Docker containerization and Nginx configuration for zero-downtime production deployments. The tests/ directory maintains 100% unit test coverage for tax calculation accuracy across all FY 2024-25 slabs and edge cases.


🏗️ System Architecture Diagram
<img width="844" height="475" alt="Screenshot 2026-01-11 at 1 11 27 PM" src="https://github.com/user-attachments/assets/bae7500e-a3ba-4460-b635-3cb8d6e84b1f" />



