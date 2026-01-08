# 🧊 S-Cube (S³) Stack

**High-Performance. Fine-Grained. Type-Safe.**

The **S-Cube Stack** is a cutting-edge web architecture designed for 2026 enterprise applications that require extreme performance, memory safety, and reactive user experiences. It bridges the gap between the speed of **Rust** and the agility of **SolidJS**.

---

## 🛠 The Pillars of S³

- **[Salvo](salvo.rs) (Rust):** A lightning-fast, ergonomic web framework. It handles the heavy lifting with native **HTTP/3** support and automatic **OpenAPI** documentation.
- **[SolidStart](start.solidjs.com) (SolidJS):** The next generation of meta-frameworks. Utilizing fine-grained reactivity, it delivers the smallest possible JavaScript bundles and industry-leading runtime performance.
- **[SeaORM](www.sea-ql.org) (Rust):** An async, dynamic ORM for Rust. It allows you to build complex relational queries with type safety, ensuring your data layer is as robust as your backend.
- **[PostgreSQL](www.postgresql.org):** The world’s most advanced open-source relational database, serving as the reliable "Source of Truth" for your enterprise data.

---

## 🚀 Why S-Cube?

### 1. Unified Type Safety
By leveraging **SeaORM** on the backend and **TypeScript** on the frontend (powered by Salvo's generated OpenAPI specs), you achieve end-to-end type safety. Change a database column, and your frontend will know immediately.

### 2. Extreme Resource Efficiency
The Rust-based backend (**Salvo**) uses a fraction of the RAM and CPU compared to traditional Node.js or Python backends, significantly reducing your 2026 cloud infrastructure costs.

### 3. Sub-Millisecond Reactivity
**SolidStart** skips the Virtual DOM entirely. Combined with **Salvo’s** high-concurrency [Tokio](tokio.rs) runtime, the S-Cube stack provides a near-instantaneous user experience even under heavy load.

---

## 📂 Project Structure

```text
├── apps/
│   ├── web/                # SolidStart Frontend
│   └── api/                # Salvo.rs Backend
├── libs/
│   ├── migration/          # SeaORM Migrations
│   └── entity/             # SeaORM Database Entities (Shared)
├── docker-compose.yml      # Local Dev Environment (Postgres)
└── README.md
```

---

## 🚥 Getting Started
### Prerequisites
* Rust & Cargo (v1.85+)
* Node.js (v22+)
* SeaORM CLI
* Docker

### Quick Start
Clone the repository:
```bash
git clone github.com
```

Start the database:
```bash
docker-compose up -d
```

Run the backend:
```bash
cd apps/api && cargo run
```

Run the frontend:
```bash
cd apps/web && npm install && npm run dev
```

---

## 🛡 License
This stack is released under the MIT License.
Built for the future of the web in 2026.
