# 1 VISION DOCUMENT - HỆ THỐNG E-OFFICE HÒA PHÁT

## 1.1 Giới thiệu

### Mục đích
Tài liệu Vision được xây dựng nhằm mô tả tổng quan hệ thống Quản lý Văn phòng – Hành chính cho Tập đoàn Hòa Phát, xác định phạm vi dự án, mục tiêu nghiệp vụ, nhu cầu của các bên liên quan và các chức năng chính. Đây là cơ sở để xây dựng các tài liệu:
* Đặc tả Use Case
* Supplementary Requirements
* Glossary & Test Case
* Kế hoạch phát triển hệ thống

### Phạm vi
Dự án hướng đến số hóa công tác văn phòng cho Tập đoàn Hòa Phát với các nghiệp vụ:
* Quản lý công văn đến / đi.
* Phê duyệt đề xuất nội bộ & Quy trình phê duyệt nhiều cấp.
* Quản lý lịch họp, đặt phòng họp & Lưu trữ tài liệu số tập trung.
* Ứng dụng AI phân loại hồ sơ và gợi ý tài liệu liên quan.

### Tài liệu tham khảo
1. Dean Leffingwell, Don Widrig, *Managing Software Requirements*, Addison Wesley, 1999.
2. Axel van Lamsweerde, *Requirements Engineering*, Wiley, 2009.
3. Brian Berenbach, *Software & Systems Requirements Engineering*, McGraw Hill, 2009.

---

## 1.2 Định vị sản phẩm

### Cơ hội nghiệp vụ
Số hóa quy trình tại Hòa Phát giúp khắc phục tình trạng chậm phê duyệt, dễ thất lạc tài liệu và thiếu minh bạch, từ đó nâng cao hiệu quả vận hành doanh nghiệp.

### Phát biểu vấn đề (Bảng 1.1)
| Nội dung | Mô tả |
| :--- | :--- |
| **Vấn đề** | Quy trình xử lý công văn và hồ sơ nội bộ còn thủ công |
| **Đối tượng ảnh hưởng** | Nhân viên, quản lý, văn thư, ban lãnh đạo |
| **Tác động** | Chậm xử lý, khó kiểm soát, tăng chi phí vận hành |
| **Giải pháp mong muốn** | Hệ thống số hóa tập trung, xử lý nhanh, minh bạch |

### Phát biểu vị trí sản phẩm
Hệ thống là nền tảng quản lý quy trình hành chính giúp tự động hóa xử lý hồ sơ, quản lý tập trung và tích hợp AI hỗ trợ, khác biệt hoàn toàn với cách làm truyền thống qua giấy tờ/email rời rạc.

---

## 1.3 Mô tả Stakeholder và người dùng

### Tổng hợp Stakeholder (Bảng 1.2)
* **Ban lãnh đạo:** Phê duyệt hồ sơ quan trọng, xem báo cáo tổng hợp.
* **Trưởng phòng:** Quản lý đơn vị, phê duyệt cấp trung.
* **Nhân viên:** Tạo đề xuất, gửi hồ sơ, tra cứu tài liệu.
* **Văn thư:** Tiếp nhận, quản lý công văn đến/đi.
* **Admin:** Quản trị tài khoản, phân quyền, vận hành hệ thống.

### Nhu cầu chính của Stakeholder (Bảng 1.3)
| Nhu cầu | Mức ưu tiên |
| :--- | :--- |
| Phê duyệt hồ sơ nhanh | Cao |
| Theo dõi trạng thái xử lý | Cao |
| Lưu trữ tài liệu tập trung | Cao |
| Tìm kiếm hồ sơ nhanh | Cao |
| AI hỗ trợ xử lý | Trung bình |

---

## 1.4 Tổng quan về sản phẩm

### Tóm tắt khả năng (Bảng 1.4)
* **Giảm thời gian xử lý:** Quy trình phê duyệt điện tử.
* **Giảm thất lạc giấy tờ:** Kho tài liệu số.
* **Minh bạch quy trình:** Nhật ký xử lý.
* **Hỗ trợ thông minh:** AI phân loại và gợi ý tài liệu.

---

## 1.5 Các đặc trưng sản phẩm (Bảng 1.5)
| Mã | Chức năng | Mã | Chức năng |
| :--- | :--- | :--- | :--- |
| **FEAT01** | Tạo công văn / đề xuất | **FEAT06** | Tìm kiếm và tra cứu |
| **FEAT02** | Phê duyệt nhiều cấp | **FEAT07** | Quản lý lịch họp |
| **FEAT03** | Từ chối / Yêu cầu sửa | **FEAT08** | Thông báo tự động |
| **FEAT04** | Theo dõi trạng thái | **FEAT09** | AI phân loại công văn |
| **FEAT05** | Lưu trữ tài liệu số | **FEAT10** | AI gợi ý tài liệu |

---

## 1.6 Các ràng buộc & 1.7 Chỉ tiêu chất lượng

### Chỉ tiêu chất lượng (Bảng 1.7)
* **Thời gian phản hồi:** < 3 giây.
* **Tỷ lệ sẵn sàng:** ≥ 99%.
* **Bảo mật:** HTTPS + Phân quyền RBAC.
* **Khả năng mở rộng:** > 10.000 người dùng.

### Yêu cầu hệ thống & Môi trường
* **Nền tảng:** Web-based (Chrome, Edge, Firefox).
* **Cơ sở dữ liệu:** SQL Server / PostgreSQL.
* **Hiệu năng:** 500 người dùng đồng thời, tìm kiếm tài liệu < 5 giây.
