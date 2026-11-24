## 🏗️ Travel & Transport Platform — Architecture Highlights

**Repo:** `vhvanhtuan/sgvt2` (private) · **Demo:** [vexedemo.dulichreal.com](https://vexedemo.dulichreal.com)

### One codebase, multiple business types
Single PHP codebase supports tour operators, bus ticket companies, cargo carriers, car rental, hotel, and visa agencies — each tenant enables only the modules it needs.

### Unified modular API
- Entry point: `api/app.php?m=<module>&a=<action>`
- Module manifest declares auth/permission per action — the router enforces access control automatically before any handler runs
- File-per-action design: only the relevant handler file is loaded per request (vs. a monolithic 4,000-line file)
- Backward-compatible: legacy URL files become thin wrappers; frontend migrates gradually

### Metadata-driven CMS & auto-generated API
- Declaring a table in `table_names` + `table_definitions` auto-generates full CRUD screens and REST endpoints — **no code required**
- Dashboard widgets configured entirely in DB rows: bar/line/pie charts, KPI tiles, combo aggregations — with per-user pinning and tenant-scoped data

### Modules
| Status | Modules |
|--------|---------|
| ✅ Live | system, content, tour, visa, crm, tools |
| 🔄 In progress | vexe (bus tickets, seat map), cargo (shipments, delivery), hotel, rental, pms, fleet |

### Tech stack
PHP 8.3 · MariaDB · React (public site, multi-domain via `config/sites.js`) · Vanilla JS (CMS) · Claude API (AI chatbot, streaming)
