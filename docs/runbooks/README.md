# 🛠 docs/runbooks — Hướng dẫn vận hành

## Mục đích

Chứa các **runbook** — hướng dẫn từng bước để xử lý các tình huống vận hành, troubleshooting, và setup.

## Nội dung hiện tại

```
runbooks/
├── local-dev.md                              ← Hướng dẫn troubleshooting local development
├── devsecops-cloud-iac-manual-operations.md ← Vận hành thủ công Cloud/IaC DevSecOps
└── cloudnativepg-foundation-manual-operations.md ← Chạy thủ công CloudNativePG foundation
```

### `local-dev.md`

Hướng dẫn khắc phục các lỗi thường gặp khi chạy local:
- Lỗi kết nối PostgreSQL
- Port bị chiếm
- Flyway migration conflict
- Docker Compose issues
- Vite dev server errors

### `devsecops-cloud-iac-manual-operations.md`

Hướng dẫn vận hành phần Cloud/IaC DevSecOps:
- Chạy bootstrap và environment bằng OpenTofu
- Kiểm tra GKE, CloudNativePG backup foundation, Redis, Secret Manager, ESO
- Tạm dừng để tiết kiệm chi phí
- Xóa và tạo lại tài nguyên đúng thứ tự

### `cloudnativepg-foundation-manual-operations.md`

Ghi lại lệnh đã chạy khi chuyển từ Cloud SQL sang CloudNativePG foundation, và hướng dẫn bật lại node pool, apply namespace/KSA/ExternalSecret cho CloudNativePG.

## Dự kiến bổ sung

```
runbooks/
├── local-dev.md           ← ✅ Hiện có
├── devsecops-cloud-iac-manual-operations.md ← ✅ Hiện có
├── db-migration.md        ← Hướng dẫn tạo/chạy database migration
├── deploy-staging.md      ← Deploy lên staging (K8s)
└── incident-response.md   ← Quy trình xử lý sự cố
```
