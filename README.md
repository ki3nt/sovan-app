# Dự án Android App cho Sovan.vn

Bộ mã nguồn hoàn chỉnh đóng gói trang web **https://sovan.vn** thành ứng dụng Android (.apk), đã tích hợp sẵn:
- **Tự động build file `.apk` trên GitHub Actions** (không cần cài Android Studio).
- **Hỗ trợ đầy đủ tính năng**: Tải file (PDF, Excel, báo giá, chứng từ...), tải ảnh/file từ điện thoại lên web, lưu phiên đăng nhập (Cookie/DOM Storage), thanh tiến trình tải trang, vuốt để làm mới (Pull-to-Refresh) và mở ứng dụng ngoài (Zalo, Gọi điện, Email).

---

## Cách 1: Lấy file APK tự động qua GitHub (Không cần cài phần mềm vào máy)

1. Giải nén file `SoVan_Android_App.zip` này ra một thư mục.
2. Đăng nhập vào **GitHub.com** -> Bấm nút **New** để tạo một Repository mới (đặt tên tuỳ ý, ví dụ: `sovan-android`).
3. Chọn **uploading an existing file** và kéo toàn bộ các file/thư mục bên trong (bao gồm cả thư mục `.github`, `app`, `build.gradle.kts`, `settings.gradle.kts`, `gradle.properties`) lên GitHub, sau đó bấm **Commit changes**.
4. Chuyển sang tab **Actions** trên thanh công cụ của Repository.
5. Bạn sẽ thấy tiến trình **Build SoVan APK** đang tự động chạy (mất khoảng 2 - 3 phút).
6. Khi hiện dấu tích xanh hoàn tất, bấm vào tiến trình đó -> Kéo xuống mục **Artifacts** -> Bấm vào **SoVan-Android-APK** để tải file `.apk` về và cài lên điện thoại Android.

---

## Cách 2: Mở bằng Android Studio trên máy tính

1. Giải nén file `SoVan_Android_App.zip`.
2. Mở **Android Studio** -> Chọn **Open** -> Trỏ tới thư mục vừa giải nén.
3. Đợi Android Studio tải Gradle hoàn tất -> Vào menu **Build** -> **Build Bundle(s) / APK(s)** -> **Build APK(s)** để xuất file `.apk`.
