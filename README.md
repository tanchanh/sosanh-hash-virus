# 🛡️ Trình So Sánh File / Hash / Kiểm Virus

Ứng dụng web công cụ gọn nhẹ chạy hoàn toàn độc lập, giúp tính toán mã băm SHA256, so sánh tính toàn vẹn giữa hai tệp tin và hỗ trợ liên kết kiểm tra mã độc trực tuyến nhanh chóng.

---

## ✨ Tính Năng Nổi Bật

* **Hoạt động Offline an toàn:** Quá trình tính toán mã băm SHA256 diễn ra hoàn toàn cục bộ trên trình duyệt thông qua thư viện Web Crypto API, tuyệt đối không tải tệp tin lên máy chủ, bảo mật dữ liệu cá nhân.
* **So sánh tệp song song:** Hỗ trợ chọn đồng thời hai tệp tin để đối chiếu trực tiếp xem nội dung dữ liệu có hoàn toàn trùng khớp hay không.
* **Đối sánh chuỗi Hash linh hoạt:** Cho phép dán hoặc nhập trực tiếp một chuỗi SHA256 từ bên ngoài để kiểm tra chéo với các tệp tin hiện tại, tự động chuyển đổi màu nền cảnh báo trực quan.
* **Đa phương thức nạp file:** Tích hợp tính năng kéo và thả tệp tin trực tiếp vào vùng nút bấm (Drop zone tích hợp) hoặc nhấp chọn truyền thống từ bộ nhớ máy tính.
* **Tích hợp kiểm virus nhanh:** Cơ chế tự động trích xuất chuỗi băm để chuyển hướng tra cứu trực tiếp trên hệ thống quét mã độc toàn cầu VirusTotal chỉ với một cú nhấp chuột.

---

## 📐 Quy Trình Hoạt Động & Định Dạng Chuẩn

Để công cụ đối sánh chính xác, chuỗi băm nhập vào thủ công cần tuân thủ tiêu chuẩn kỹ thuật sau:

* **Định dạng mã băm hỗ trợ:** Chuỗi ký tự độ dài cố định **64 ký tự** thuộc hệ thập lục phân (Hexadecimal bao gồm các ký tự từ `0-9` và `a-f`).
* **Cơ chế so sánh:** Hệ thống tự động chuyển đổi chuỗi về dạng chữ thường (Lowercase) trước khi so sánh, loại bỏ sự sai lệch do định dạng chữ hoa/chữ thường từ các nguồn cấp khác nhau.

---

## 🛠️ Hướng Dẫn Sử Dụng

* **Tải và Tính mã băm:** Nhấp nút **Chọn File 1** / **Chọn File 2** (hoặc kéo thả tệp trực tiếp vào nút) để nạp dữ liệu. Hệ thống sẽ tự động hiển thị tên tệp kèm dung lượng chuẩn hoá (`B`, `KB`, `MB`, `GB`) và tính mã SHA256 theo thời gian thực.
* **Đối chiếu tự động:** Khi cả hai tệp được nạp thành công, bảng kết quả sẽ tự động đưa ra kết luận trùng khớp (màu xanh lá) hoặc không trùng khớp (màu đỏ).
* Nhấp nút **Sao Chép** ngay cạnh chuỗi SHA256 vừa tính để lưu mã băm vào bộ nhớ đệm (Clipboard).

* **Kiểm tra chéo và Quét Virus:**
* Sử dụng nút **Dán** hoặc tự nhập mã SHA256 vào ô trống để so sánh nhanh với hai tệp tin phía trên. Nhấp nút **Xoá** để dọn sạch ô nhập liệu và đặt lại trạng thái.
* Nhấp nút **Kiểm Virus Online** để chuyển hướng tra cứu. Nếu ô nhập liệu có sẵn mã băm, hệ thống sẽ mở thẳng trang kết quả quét mã độc của tệp đó trên VirusTotal.

---

## 📝 Thông Tin Phát Triển

* **Tác giả:** Dương Tấn Chánh
* **Công nghệ tích hợp:** HTML5 (Drag and Drop API), CSS3 (Variables Custom Properties & Responsive Layout), JavaScript Thuần (Vanilla JS - Ứng dụng Web Crypto API thuần tuý để xử lý bất đồng bộ mã hoá, tối ưu dung lượng và tốc độ).
