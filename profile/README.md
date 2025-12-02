# ☕ POS Coffee — Microservice Architecture  
**Kubernetes • Kong API Gateway • RabbitMQ • Java (Wallet & Account) • Go (Transaction, Master Data, SSE) • Node.js (Notification)**

POS Coffee adalah sistem Point of Sale modular untuk kedai kopi, dibangun dengan arsitektur **microservices** dan komunikasi event-driven menggunakan **RabbitMQ**.  
Seluruh service berjalan di atas **Kubernetes**, memakai **Kong** sebagai API Gateway, dan memanfaatkan **SSE Gateway** untuk realtime update ke frontend.

---

# 🚀 Tech Stack Overview

### Backend Services
| Service | Language | Responsibilities |
|---------|----------|------------------|
| **wallet-service** | Java Spring Boot | Saldo, topup, debit, ledger |
| **account-service** | Java Spring Boot | Registrasi user, auth, OTP, profile |
| **transaction-service** | Go Fiber | Order, POS transaction, internal payment |
| **master-data-service** | Go Fiber | Produk, kategori, toko, meja |
| **sse-gateway** | Go Fiber | Realtime event → SSE stream |
| **notification-service** | Node.js + Resend | Email notif, receipt, OTP |

### Infrastructure
- **Kubernetes**
- **Kong API Gateway**
- **RabbitMQ**
- **Redis** (cache & idempotency)
- **PostgreSQL per service**
