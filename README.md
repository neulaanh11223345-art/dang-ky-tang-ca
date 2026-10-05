# 📝 Đăng ký Tăng ca — Credible Việt Nam

Ứng dụng web cho phép nhân viên **đăng ký tăng ca bằng điện thoại**, tự động tính số giờ, xem trước đơn và **xuất file PDF/Excel để trình ký**.

> Chỉ cần 1 file `index.html`, chạy được ngay trên **GitHub Pages** không cần server.

## ✨ Tính năng

- 📱 Giao diện tối ưu cho điện thoại (mobile-first)
- ➕ Thêm nhiều ngày tăng ca, **tự tính số giờ** từ khung giờ (từ - đến)
- 🏷️ Chọn ca làm việc: Hành chính / Ca ngày / Ca đêm / Chủ nhật
- 💾 Lưu nháp tự động trên máy (localStorage) — không sợ mất dữ liệu
- 👁️ Xem trước đơn đúng khuôn mẫu công ty (song ngữ Việt - Trung)
- 🖨️ **In / Lưu PDF** để trình ký tên
- 📊 **Xuất file Excel** (`.xlsx`) gửi bộ phận HCNS
- ✍️ Đầy đủ 4 ô chữ ký: Người xin · Người xác nhận · Quản lý bộ phận · Hành chính nhân sự

## 🚀 Cách đưa lên GitHub (cho mọi người dùng)

### Bước 1: Tạo repository
1. Đăng nhập [github.com](https://github.com) → bấm **New repository**
2. Đặt tên ví dụ: `dang-ky-tang-ca`, để **Public**, tick **Add a README file** → **Create repository**

### Bước 2: Upload file `index.html`
1. Vào repository vừa tạo → bấm **Add file → Upload files**
2. Kéo thả file `index.html` (và `README.md` này) vào → bấm **Commit changes**

### Bước 3: Bật GitHub Pages
1. Vào tab **Settings** → menu **Pages** (bên trái)
2. Ở **Source** chọn **Deploy from a branch**
3. Ở **Branch** chọn `main` / `(root)` → bấm **Save**
4. Đợi ~1 phút, đường dẫn sẽ hiện ra dạng:  
   `https://<tên-tài-khoản>.github.io/dang-ky-tang-ca/`

### Bước 4: Chia sẻ
Gửi đường link trên cho đồng nghiệp — họ mở bằng điện thoại là dùng được ngay, không cần cài đặt gì.

## 📖 Hướng dẫn sử dụng (gửi kèm cho nhân viên)

1. Mở link bằng điện thoại
2. Tab **Điền thông tin**: nhập Họ tên, Mã thẻ, Bộ phận, Chức vụ
3. Bấm **Thêm ngày tăng ca** cho mỗi buổi tăng ca: chọn ngày, ca, giờ bắt đầu/kết thúc, lý do
   - Số giờ được **tự động tính** (có thể sửa tay nếu cần)
4. Bấm **Lưu nháp** nếu muốn làm tiếp sau
5. Sang tab **Xem trước & Xuất**:
   - **In / Lưu PDF** → chọn máy in "Lưu thành PDF" → có file đơn để in ra ký
   - **Xuất file Excel** → tải file `.xlsx` gửi HCNS
6. In đơn PDF ra, ký tên và trình cấp trên duyệt

## ⚙️ Tùy chỉnh nhanh

- **Tên công ty / tiêu đề**: sửa trong `index.html` tại khối `#printArea .co` và `.title`
- **Danh sách bộ phận / chức vụ gợi ý**: sửa các `<option>` trong `<datalist id="deptList">` và `posList`
- **Màu sắc**: sửa biến `--accent` trong `<style>`

---

*Dữ liệu chỉ lưu trên trình duyệt của người dùng (localStorage), không gửi lên server. Người dùng tự xuất file để nộp.*
