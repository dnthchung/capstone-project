# Giới Thiệu

Hệ thống quản lý vận chuyển và điểm danh học sinh tự động là một giải pháp toàn diện, kết hợp công nghệ AI, camera và thẻ từ/QR code để đảm bảo học sinh luôn có mặt trên xe trong suốt chuyến đi và luôn có mặt trong tiết/ca/buổi học của ngày hôm đó. Hệ thống hoạt động hoàn toàn tự động, giúp nâng cao hiệu quả quản lý và đảm bảo an toàn cho học sinh.

---

## Phần 1: Tổng Hợp Chi Tiết Về Cách Hệ Thống Hoạt Động

### 1. Trên Xe Bus (On Bus)

#### 1.1. Tự Động Nhận Diện Học Sinh

- **Camera quét tự động**:
    - Camera được lắp đặt ở cửa lên/xuống xe và các vị trí chiến lược trên xe.
    - Khi học sinh lên/xuống xe, camera tự động quét và nhận diện khuôn mặt.
    - Hệ thống AI so sánh khuôn mặt với cơ sở dữ liệu và cập nhật trạng thái "đã lên xe" hoặc "đã xuống xe".
- **Thông báo tự động (qua mobile app)**:
    - Hệ thống gửi thông báo (mobile app) đến phụ huynh và tài xế mỗi khi học sinh check-in/check-out.

#### 1.2. Đảm Bảo Học Sinh Luôn Có Mặt Trên Xe

- **Camera giám sát liên tục**:
    - Camera trên xe liên tục quét và nhận diện khuôn mặt học sinh trong suốt chuyến đi.
    - Hệ thống AI xác nhận sự hiện diện của học sinh.
    - Nếu học sinh không được phát hiện trong một khoảng thời gian nhất định, hệ thống sẽ gửi cảnh báo (qua mobile app) đến tài xế và quản trị viên (Admin).

### 2. Trong Lớp Học (In Class)

#### 2.1. Tự Động Điểm Danh

- **Camera quét tự động**:
    - Camera được lắp đặt ở cửa lớp và các góc lớp.
    - Khi học sinh vào/ra lớp, camera tự động quét và nhận diện khuôn mặt.
    - Hệ thống AI so sánh khuôn mặt với cơ sở dữ liệu và cập nhật trạng thái "đã vào lớp" hoặc "đã ra lớp".
- **Thông báo tự động (qua mobile app)**:
    - Hệ thống gửi thông báo đến giáo viên khi học sinh check-in/check-out.

#### 2.2. Đảm Bảo Học Sinh Luôn Có Mặt Trong Tiết/Ca/Buổi Học

- **Camera giám sát liên tục**:
    - Camera trong lớp liên tục quét và nhận diện khuôn mặt học sinh trong suốt buổi học.
    - Hệ thống AI xác nhận sự hiện diện của học sinh.
    - Nếu học sinh không được phát hiện trong một khoảng thời gian nhất định, hệ thống sẽ gửi cảnh báo đến giáo viên và quản trị viên (Admin).

---

## Phần 2: Các Actor Tham Gia Vào Hệ Thống

### 1. Học Sinh

- **Feature**:
    - Tự động check-in/check-out trên xe bus và trong lớp học bằng camera AI.
    - Sử dụng thẻ từ/QR code để check-in/check-out nếu camera gặp sự cố.
- **Quy trình thao tác**:
    - Học sinh lên/xuống xe hoặc vào/ra lớp, camera tự động quét và nhận diện khuôn mặt.
    - Nếu camera gặp sự cố, học sinh sử dụng thẻ từ/QR code để check-in/check-out.

### 2. Phụ Huynh

- **Feature**:
    - Nhận thông báo (qua mobile app) về trạng thái lên/xuống xe của con em.
    - Theo dõi lịch trình và thông tin chuyến đi trên mobile app.
- **Quy trình thao tác**:
    - Phụ huynh cài đặt mobile app trên điện thoại.
    - Nhận mọi thông báo về check-in/check-out và cập nhật lộ trình qua mobile app.

### 3. Tài Xế

- **Feature**:
    - Theo dõi lộ trình và danh sách học sinh trên xe (thông qua mobile app).
    - Nhận cảnh báo nếu học sinh không được phát hiện trên xe.
    - Sử dụng mobile app để quét thẻ từ/QR code của học sinh nếu camera gặp sự cố.
    - Xác nhận hoàn thành tuyến đường sau khi tất cả học sinh đã xuống xe.
- **Quy trình thao tác**:
    - Tài xế đăng nhập mobile app, xem danh sách học sinh và lộ trình (xem map in app).
    - Nhận thông báo về học sinh đã lên/xuống xe và cảnh báo nếu có bất thường.
    - Tài xế sử dụng mobile app để quét thẻ từ/QR code nếu camera gặp sự cố.
    - Tài xế nhấn nút xác nhận hoàn thành chuyến đi trên mobile app.

### 4. Giáo Viên

- **Feature**:
    - Theo dõi kết quả điểm danh trong lớp học (thông qua mobile app).
    - Nhận cảnh báo nếu học sinh không được phát hiện trong lớp.
    - Sử dụng mobile app để quét thẻ từ/QR code của học sinh nếu camera gặp sự cố.
- **Quy trình thao tác**:
    - Giáo viên đăng nhập mobile app để xem báo cáo điểm danh và nhận thông báo.
    - Giáo viên sử dụng mobile app để quét thẻ từ/QR code nếu camera gặp sự cố.

### 5. Quản Trị Viên (Admin)

- **Feature**:
    - **Là người dùng chính của giao diện web**.
    - Quản lý thông tin học sinh, lớp học, xe bus, tài xế.
    - Xem và quản lý báo cáo về hoạt động của hệ thống.
    - **Chỉ theo dõi** danh sách tuyến đường (được hệ thống thiết lập tự động) của ngày hôm đó theo thời gian. - (Có thể chỉnh sửa nếu có vấn đề)
    - Thiết lập tùy chọn **sign** học sinh vào lớp (bằng thuật toán tự động hoặc theo mã số/ngày sinh...) .
- **Quy trình thao tác**:
    - Admin **đăng nhập** vào **website** để thêm, sửa, xóa thông tin cần thiết (học sinh, xe bus, tài xế, lớp học...).
    - Theo dõi danh sách tuyến đường do hệ thống tự động tạo ra.
    - Xem báo cáo chi tiết quá trình vận hành (điểm danh, lộ trình, ...).

---

## Phần 3: Công Nghệ Sử Dụng

### 1. Camera AI

- Camera tích hợp AI để nhận diện khuôn mặt trong thời gian thực.

### 2. Thuật Toán Nhận Diện

- Sử dụng các thuật toán nhận diện khuôn mặt hiện đại như FaceNet hoặc DeepFace.

### 3. Thẻ Từ/QR Code

- Học sinh được cấp thẻ từ/QR code cá nhân để sử dụng khi camera gặp sự cố.

### 4. Mobile App

- **Ứng dụng di động** dành cho tài xế, giáo viên và phụ huynh:
    - Gửi/nhận thông báo (check-in, check-out, cảnh báo).
    - Theo dõi lộ trình (tài xế, phụ huynh).
    - Quét thẻ từ/QR code (tài xế, giáo viên).

### 5. Giao Diện Web

- **Chủ yếu dành cho Admin**:
    - Thêm, sửa, xóa thông tin học sinh, lớp học, xe bus, tài xế. ( có thể dùng import file nếu số lợnợng lớn )
    - Theo dõi danh sách tuyến đường tự động (không cần tạo tay).
    - Tùy chọn cấu hình tính năng sign học sinh vào lớp (tự động hoặc theo tiêu chí).
    - Tạo và xem báo cáo chi tiết.

### 6. Cơ Sở Dữ Liệu

- Lưu trữ hình ảnh và thông tin học sinh để so sánh và nhận diện.
- Lưu trữ lịch sử check-in/check-out, thông tin lộ trình, lớp học.
- Lưu trữ báo cáo, log hoạt động.

---

## Phần 4: Quy Trình Thao Tác Của Hệ Thống

### A. Quy Trình Trên Xe Bus

#### Bước 1: Admin Thiết Lập Thông Tin Ban Đầu (trên Web)

1. **Đăng nhập hệ thống**:
    - Admin đăng nhập vào website quản trị bằng tài khoản và mật khẩu.
2. **Quản lý học sinh**:
    - Admin thêm, sửa, xóa thông tin học sinh (tên, lớp, địa chỉ, phụ huynh, ...).
3. **Quản lý xe bus và tài xế**:
    - Admin thêm, sửa, xóa thông tin xe bus (biển số, loại xe, sức chứa) và tài xế (tên, số điện thoại, bằng lái).
4. **Tùy chọn cách sign học sinh vào lớp**:
    - Admin bật/tắt chế độ **auto sign** hoặc sign theo tiêu chí (mã học sinh, ngày sinh...).

#### Bước 2: Hệ Thống Tự Động Thiết Lập Tuyến Đường

1. **Thu thập dữ liệu**:
    - Hệ thống thu thập thông tin học sinh, xe bus, tài xế, vị trí đón/trả từ cơ sở dữ liệu.
2. **Sử dụng thuật toán**:
    - Hệ thống tự động chạy thuật toán tối ưu (ví dụ TSP - Travelling Salesman Problem) để **thiết lập tuyến đường** đón và trả học sinh theo khu vực, hoàn toàn không thao tác thủ công.
3. **Phân công tài xế và xe bus**:
    - Hệ thống tự động phân công tài xế và xe bus cho từng tuyến đường.
4. **Tạo lịch trình**:
    - Hệ thống tạo lịch trình chi tiết (thời gian đón/trả, điểm dừng...) và lưu vào cơ sở dữ liệu.

#### Bước 3: Thực Hiện Chuyến Đi (Tài xế dùng Mobile App)

1. **Check-in học sinh lên xe**:
    - Khi học sinh lên xe, camera ở cửa tự động quét và nhận diện khuôn mặt.
    - Nếu camera gặp sự cố, tài xế sử dụng mobile app để quét thẻ từ/QR code của học sinh.
    - Hệ thống cập nhật trạng thái "đã lên xe" và gửi thông báo đến phụ huynh (mobile app).
2. **Giám sát học sinh trên xe**:
    - Camera trên xe liên tục quét và nhận diện khuôn mặt học sinh trong suốt chuyến đi.
    - Nếu học sinh không được phát hiện, hệ thống gửi cảnh báo (mobile app) đến tài xế và Admin (web).
3. **Check-out học sinh xuống xe**:
    - Khi học sinh xuống xe, camera ở cửa tự động quét và nhận diện khuôn mặt.
    - Nếu camera gặp sự cố, tài xế sử dụng mobile app để quét thẻ từ/QR code.
    - Hệ thống cập nhật trạng thái "đã xuống xe" và gửi thông báo đến phụ huynh (mobile app).

#### Bước 4: Xác Nhận Hoàn Thành Route

1. **Tài xế xác nhận hoàn thành route (trên Mobile App)**:
    - Sau khi tất cả học sinh đã xuống xe và check-out thành công, tài xế nhấn nút xác nhận hoàn thành route.
2. **Cập nhật trạng thái route**:
    - Hệ thống cập nhật trạng thái route là "đã hoàn thành" và lưu trữ dữ liệu.
3. **Admin theo dõi**:
    - Admin chỉ **theo dõi** danh sách tuyến đường, trạng thái hoàn thành và báo cáo tổng hợp trên web.

---

### B. Quy Trình Trong Lớp Học

#### Bước 1: Admin Thiết Lập Thông Tin Ban Đầu (trên Web)

1. **Quản lý lớp học**:
    - Admin thêm, sửa, xóa thông tin lớp học (tên lớp, giáo viên chủ nhiệm, danh sách học sinh).
2. **Tùy chọn cách sign học sinh vào lớp**:
    - Admin cấu hình chế độ tự động hoặc theo tiêu chí mã số/ngày sinh...

#### Bước 2: Điểm Danh Trong Lớp Học (Giáo viên dùng Mobile App)

1. **Check-in học sinh vào lớp**:
    - Khi học sinh vào lớp, camera ở cửa tự động quét và nhận diện khuôn mặt.
    - Nếu camera gặp sự cố, giáo viên sử dụng mobile app để quét thẻ từ/QR code.
    - Hệ thống cập nhật trạng thái "đã vào lớp" và gửi thông báo cho giáo viên (mobile app).
2. **Giám sát học sinh trong lớp**:
    - Camera trong lớp liên tục quét và nhận diện khuôn mặt học sinh.
    - Hệ thống đảm bảo học sinh luôn có mặt trong lớp.
    - Nếu không, cảnh báo được gửi đến giáo viên (mobile app) và Admin (web).
3. **Check-out học sinh ra khỏi lớp**:
    - Khi học sinh ra lớp, camera tự động quét và nhận diện khuôn mặt.
    - Nếu camera gặp sự cố, giáo viên sử dụng mobile app để quét thẻ từ/QR code.
    - Hệ thống cập nhật trạng thái "đã ra lớp" và gửi thông báo cho giáo viên (mobile app).

---

## Phần 5: Ví Dụ Minh Họa Quy Trình

### 1. Trên Xe Bus

1. **Admin A** đăng nhập vào web, vào mục **Cài đặt lịch trình đưa đón**.
2. **Hệ thống tự động phân bổ tuyến đường** dựa trên các bước sau:
    - Admin chỉ cần chọn **thời gian hiệu lực**:
        - **Option 1**: Áp dụng cố định trong **một tháng**.
        - **Option 2**: Lịch trình thay đổi tự động theo tuần hoặc nhiều tháng.
    - Sau khi chọn thời gian, Admin nhấn nút **"Xác nhận"**.
3. **Hệ thống tự động thiết lập lộ trình và phân công tài xế/xe bus**:
    - Sử dụng thuật toán tối ưu (TSP) để phân bổ tuyến đường một cách công bằng và hiệu quả.
    - Ví dụ:
        - Tài xế A phụ trách khu vực phía Bắc với xe bus số 1.
        - Tài xế B phụ trách khu vực phía Nam với xe bus số 2.
    - Các tuyến đường sẽ tự động cập nhật và hiển thị trong hệ thống.
4. **Học sinh C** lên xe:
    - Camera AI tự động nhận diện khi học sinh bước lên xe -> Hệ thống cập nhật trạng thái “đã lên xe” và gửi thông báo đến phụ huynh qua mobile app.
5. **Học sinh C** xuống xe:
    - Camera AI tự động nhận diện khi học sinh bước xuống xe -> Hệ thống cập nhật trạng thái “đã xuống xe” và gửi thông báo đến phụ huynh qua mobile app.
6. Sau khi hoàn thành lộ trình:
    - Tài xế nhấn nút **“Hoàn thành”** trên mobile app để xác nhận kết thúc chuyến đi.
    - Admin có thể xem báo cáo chi tiết bao gồm:
        - Lịch trình đưa đón.
        - Danh sách học sinh đã check-in/check-out.
        - Thời gian hoàn thành lộ trình.

---

### 2. Trong Lớp Học

1. **Admin A** cấu hình 3 lớp học, thêm giáo viên chủ nhiệm, chọn cách “sign” học sinh **tự động** vào lớp dựa trên dữ liệu hệ thống.
2. **Học sinh C** bước vào lớp: Camera AI tự động nhận diện, cập nhật trạng thái “đã vào lớp” -> Giáo viên nhận thông báo qua mobile app.
3. Trong giờ học: Camera AI tiếp tục theo dõi liên tục. Nếu **học sinh C** rời khỏi lớp hoặc không xuất hiện trong thời gian dài, hệ thống gửi cảnh báo ngay đến giáo viên và Admin.
4. **Học sinh C** ra khỏi lớp: Camera AI tự động nhận diện, cập nhật trạng thái “đã ra lớp” -> Giáo viên nhận thông báo qua mobile app.

---

## Phần 6: Phương Án Backup Bằng Thẻ Từ/QR Code

### 1. Trên Xe Bus

- **Khi camera gặp sự cố**:
    - Tài xế dùng mobile app để quét thẻ từ/QR code học sinh khi lên/xuống xe.
    - Hệ thống vẫn cập nhật trạng thái và gửi thông báo (mobile app) cho phụ huynh.

### 2. Trong Lớp Học

- **Khi camera gặp sự cố**:
    - Giáo viên dùng mobile app để quét thẻ từ/QR code học sinh khi vào/ra lớp.
    - Hệ thống cập nhật trạng thái và gửi thông báo (mobile app) cho giáo viên.

---

## Phần 7: Ghi Chú

- **Các hạng mục chưa rõ/cần xác nhận**:
    1. Có làm chức năng điểm danh cho **tài xế** hay không? (Để đảm bảo đúng tài xế đã được phân công, tránh trường hợp thay người lái hộ).
    2. Quy trình xác minh tài xế: cần dùng camera AI nhận diện tài xế hay chỉ cần xác thực tài khoản trên mobile app?
    3. Phần cấu hình chi tiết về "thuật toán sign" vào lớp có thể được thiết kế mở rộng theo nhiều tiêu chí khác nhau.

---

## Kết Luận

Phiên bản cập nhật của hệ thống quản lý vận chuyển và điểm danh học sinh tự động nhấn mạnh:

1. **Mobile app**: Kênh chính cho phụ huynh, tài xế, giáo viên để nhận thông báo và thao tác cần thiết (quét mã, xác nhận).
2. **Giao diện web**: Dành cho **Admin** quản lý, **theo dõi tuyến đường tự động** và báo cáo.
3. **Thuật toán**:
    - **Thiết lập tuyến đường** trên xe bus hoàn toàn tự động (không thao tác thủ công).
    - **Sign học sinh vào lớp** có tùy chọn tự động hoặc dựa trên tiêu chí cụ thể.
