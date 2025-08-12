# CodeArtifact CI Sample (Node + Snyk)

## 1) Chuẩn bị
- Tạo GitHub repo mới, sau đó tải thư mục này lên.
- Tạo GitHub Secrets trong **Settings → Secrets and variables → Actions**:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_REGION` (ví dụ: `ap-southeast-1`)
  - `SNYK_TOKEN` (lấy từ https://snyk.io)

## 2) Chỉnh sửa tham số CI nếu cần
Mặc định:
- Domain CodeArtifact: `secure-domain`
- Repository: `dev-repo`

Đổi trong file `.github/workflows/ci.yml` nếu bạn dùng tên khác.

## 3) Chạy
- Commit & push lên nhánh `main`.
- Xem tab **Actions** để theo dõi pipeline.
