
# Phần mềm Quản lý Thu phí Chung cư BlueMoon

## Mô tả Dự án

Phần mềm quản lý thu phí ở chung cư BlueMoon được phát triển với mục tiêu giúp Ban quản trị chung cư quản lý các khoản phí dịch vụ, phí quản lý và các khoản đóng góp từ cư dân trong chung cư. Phần mềm hỗ trợ tự động hóa việc thu phí, thống kê các khoản thu và quản lý thông tin về hộ gia đình, nhân khẩu trong chung cư.

Dự án được xây dựng dưới dạng ứng dụng desktop với công nghệ Java và cơ sở dữ liệu MySQL. Phần mềm sẽ hỗ trợ các chức năng cơ bản như tạo khoản thu, thu phí, thống kê các khoản đóng góp và quản lý thông tin hộ gia đình, nhân khẩu.

### Các chức năng chính của phần mềm:
1. **Quản lý thông tin hộ gia đình**: Quản lý các thông tin liên quan đến hộ khẩu và nhân khẩu của cư dân trong chung cư.
2. **Quản lý thu phí**: Quản lý các khoản thu phí dịch vụ, phí quản lý, phí gửi xe và các khoản đóng góp khác.
3. **Thống kê và báo cáo**: Cung cấp các báo cáo về tình trạng thu phí và các khoản đóng góp.
4. **Quản lý người dùng**: Phân quyền truy cập và bảo mật thông tin cho các thành viên trong Ban quản trị chung cư.

## Cấu trúc Dự án

Dưới đây là mô tả về cấu trúc thư mục của dự án:

```
/BlueMoon-Project
│
├── /docs                # Tài liệu dự án
│   ├── /SRS             # Tài liệu yêu cầu phần mềm
│   ├── /User_Guide      # Hướng dẫn người dùng
│   ├── /Tech_Specs      # Tài liệu kỹ thuật
│   ├── /WBS             # Phân chia công việc (Work Breakdown Structure)
│   │   └── WBS.xlsx     # Tệp phân chia công việc của dự án
│   └── /Timeline        # Lịch trình dự án
│       └── Timeline.xlsx # Tệp timeline dự án (Gantt Chart)
│
├── /src                 # Mã nguồn phần mềm
│   ├── /main
│   │   ├── /java        # Mã nguồn Java
│   │   ├── /resources   # Tài nguyên (config, hình ảnh, v.v.)
│   │   └── /sql         # Tập lệnh SQL cho cơ sở dữ liệu
│   └── /test            # Các tệp kiểm thử
│       ├── /unit_tests  # Kiểm thử đơn vị
│       └── /integration_tests  # Kiểm thử tích hợp
│
├── /build               # Các tệp xây dựng dự án (ví dụ: JAR, WAR, v.v.)
│
├── /config              # Các tệp cấu hình hệ thống (configurations)
│   ├── /database        # Cấu hình cơ sở dữ liệu
│   ├── /server          # Cấu hình máy chủ
│   └── /application     # Cấu hình ứng dụng
│
├── /scripts             # Các script tiện ích
│   ├── /setup           # Các script thiết lập ban đầu
│   └── /deploy          # Các script triển khai
│
├── /resources           # Các tài nguyên như hình ảnh, giao diện người dùng, v.v.
│   ├── /images          # Ảnh và biểu tượng
│   ├── /css             # Tệp CSS cho giao diện người dùng
│   └── /js              # Tệp JavaScript
│
├── /logs                # Các tệp log hệ thống
│
├── /tests               # Các bài kiểm tra tự động và thủ công
│
└── README.md            # Tài liệu giới thiệu và hướng dẫn sử dụng
```

### Mô tả các thư mục:

1. **/docs**: Lưu trữ tất cả tài liệu liên quan đến dự án, bao gồm tài liệu yêu cầu phần mềm (SRS), hướng dẫn người dùng, tài liệu kỹ thuật, phân chia công việc (WBS), và lịch trình dự án (Timeline).
   
2. **/src**: Chứa mã nguồn của phần mềm. Thư mục con `/main` chứa mã nguồn Java chính, tài nguyên cần thiết cho ứng dụng, và các tập lệnh SQL cho cơ sở dữ liệu. Thư mục `/test` chứa các tệp kiểm thử phần mềm.

3. **/build**: Lưu trữ các tệp xây dựng của dự án (chẳng hạn như các tệp JAR hoặc WAR) sau khi biên dịch mã nguồn.

4. **/config**: Các tệp cấu hình của hệ thống như cấu hình cơ sở dữ liệu, máy chủ, và ứng dụng.

5. **/scripts**: Lưu trữ các script tiện ích giúp thiết lập môi trường ban đầu và triển khai phần mềm.

6. **/resources**: Chứa các tài nguyên như hình ảnh, tệp CSS, và JavaScript dùng trong giao diện người dùng.

7. **/logs**: Các tệp log hệ thống để theo dõi hoạt động của phần mềm.

8. **/tests**: Các tệp kiểm tra tự động và thủ công giúp đảm bảo chất lượng phần mềm.

---

### Cài đặt và Sử dụng

1. **Yêu cầu hệ thống**:
   - Java JDK (phiên bản 11 hoặc mới hơn)
   - MySQL (hoặc hệ quản trị cơ sở dữ liệu tương thích)
   - Công cụ quản lý mã nguồn Git
   - IDE (Eclipse, IntelliJ, v.v.)

2. **Hướng dẫn cài đặt**:
   - Cloning repository:
     ```bash
     git clone https://github.com/thanhsonnee/KTPM-nhom24.git
     ```
   - Cài đặt các phụ thuộc (nếu có) và cấu hình cơ sở dữ liệu.
   - Chạy phần mềm trên môi trường phát triển Java.

---

### Liên hệ

- **Email**: vudo22555@gmail.com
