# Báo cáo Prompt Logic & Tư duy UX - Trang Web Du lịch (Smart Interface)

## 1. Danh sách Prompt AI đã sử dụng (Vibe Coding)

Nhóm đã sử dụng các câu lệnh Prompt AI sau để hỗ trợ viết mã, tinh chỉnh chuyển động và xử lý lỗi hiệu ứng:

* **Prompt tối ưu thông số cubic-bezier cho chuyển động Hero Section:**
  > *"Hãy đóng vai là một chuyên gia Frontend Animation. Hãy giúp tôi viết đoạn mã CSS sử dụng thuộc tính `transition` với hàm `cubic-bezier()` để tạo hiệu ứng trượt lên (Slide-up) và mờ dần (Fade-in) cho phần Banner trang web du lịch. Yêu cầu thông số phải tạo ra cảm giác chuyển động mượt mà, tăng tốc nhẹ nhàng ở đầu và giảm tốc mượt ở cuối, tuyệt đối không bị giật cục."*

* **Prompt xử lý lỗi xung đột hiệu ứng cuộn trang (AOS Library):**
  > *"Tôi đang tích hợp thư viện AOS (Animate On Scroll) cho các Section danh mục tour du lịch và blog, nhưng khi người dùng cuộn chuột nhanh, các hiệu ứng bị chồng lấn và gây giật lag (đặc biệt khi dùng thuộc tính top/left). Hãy đề xuất giải pháp tối ưu bằng cách dùng `transform: translate3d()` và cấu hình lại data-aos attributes cho các thẻ Card."*

* **Prompt tối ưu Micro-interactions cho nút Đặt Tour (Call-to-Action):**
  > *"Hãy tạo hiệu ứng Micro-interactions bằng CSS cho nút 'Đặt tour ngay' (CTA button): khi rê chuột vào (hover) thì nút nổi lên nhẹ nhàng kèm hiệu ứng bóng đổ (box-shadow), và khi click (active state) thì có hiệu ứng lún xuống phản hồi tức thì cho người dùng."*

---

## 2. Giải thích tư duy UX cho từng Section trên Website Du lịch

Lý do nhóm lựa chọn và phân bổ các hiệu ứng chuyển động nhằm tối ưu hóa trải nghiệm người dùng (UX):

* **Header & Hero Section (Intro Animation):** 
  * *Hiệu ứng áp dụng:* Fade-in kết hợp Slide-up.
  * *Tư duy UX:* Ngay khi người dùng mở trang web du lịch, hình ảnh banner hoành tráng của điểm đến nổi bật cùng thanh menu sẽ xuất hiện mượt mà. Điều này thu hút ngay thị giác, tạo cảm giác chuyên nghiệp, cao cấp và kích thích người dùng khám phá tiếp mà không gây cảm giác ngợp thông tin.

* **Interactive Portfolio / Menu (Các Thẻ Card Tour Du Lịch):**
  * *Hiệu ứng áp dụng:* Hover effect chuyển động phóng to nhẹ hoặc lật thẻ (Flip)[cite: 1].
  * *Tư duy UX:* Thay vì hiển thị toàn bộ thông tin chi tiết (giá cả, lịch trình, số ngày) làm rối mắt giao diện, nhóm sử dụng hiệu ứng tương tác khi rê chuột. Người dùng chủ động tương tác với địa điểm nào thì thông tin chi tiết của điểm đến đó mới hiển thị, giúp giao diện gọn gàng và tăng tính khám phá.

* **Scroll Revelation (Các Section Danh Mục Tour, Đánh Giá, Blog):**
  * *Hiệu ứng áp dụng:* Thư viện AOS (Animate On Scroll)[cite: 1].
  * *Tư duy UX:* Khi người dùng cuộn chuột xuống dưới để tìm hiểu về các dịch vụ du lịch, các khối nội dung sẽ lần lượt trượt ra nhịp nhàng theo chiều cuộn. Hiệu ứng này dẫn dắt dòng đọc của mắt người dùng một cách tự nhiên, giảm tải áp lực thị giác khi phải nhìn một lượng thông tin lớn cùng lúc.

* **Micro-interactions (Các Nút Bấm / Call-to-Action):**
  * *Hiệu ứng áp dụng:* Thay đổi màu sắc, scale và active state[cite: 1].
  * *Tư duy UX:* Giúp cung cấp phản hồi trực quan (Visual Feedback) ngay lập tức cho người dùng biết thao tác chạm/click của họ đã được hệ thống ghi nhận, tạo cảm giác trang web có "linh hồn" và độ nhạy cao.