# Victor-Hugo
- Họ và Tên: Hoàng Đình Hiếu
- Lớp: K59.KMT.K01
- MSSV: K235480106025
1. Dowload và cài đặt SQL server 2025
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/de19a45f-3e99-4055-a98f-20ea87c6d7c2" />
2. Cấu hình SQL server làm việc ở cổng động (Dynamic Port), TCP Dynamic Ports: 36025 (MSSV: K235480106025)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/630eac09-aede-4f8d-92e8-0dc6f9f624cb" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/932b35e1-7d7d-415f-b3c8-c478e5bf9421" />
3. Kiểm tra service SQL server và cổng

- chạy lệnh: `bin>netstat -ano | findstr LISTENING`
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0b6e4164-5c70-451d-928b-a9e7533beb72" />

4. Cài đặt SQL Server Management Studio (SSMS)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d44bfe16-9c87-4489-8b64-552324785ffa" />

5. Chạy phần mền SSMS đăng nhập vào bằng 2 cách:

Windows Authentication và SQL Server authentication.

**Windows Authentication**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e0c319ea-0e57-432f-aa10-2389c2b99aa7" />
**SQL Server Authentication**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/17af9168-3e54-4f10-a2cc-9c53de410924" />

6. Tạo Database mới 
Màn hình SSMS sau khi tạo CaiTriSinhVien xong (Thấy CaiTriSinhVien trong Object Explorer)
<img width="1920" height="1080" alt="2026-04-08 (6)" src="https://github.com/user-attachments/assets/f62008a9-4367-4566-adaa-4bbad7d3639d" />

Cửa sổ File Explorer thấy 2 file .mdf và .ldf 
<img width="1920" height="1080" alt="2026-04-08 (7)" src="https://github.com/user-attachments/assets/863942ec-1d68-44ad-91e9-deb87c561431" />

7. Tạo bảng dữ liệu với khóa chính (Primary Key) là trường masv
<img width="1920" height="1080" alt="2026-04-08 (8)" src="https://github.com/user-attachments/assets/5be4a3d9-8de2-4c87-a220-607337869172" />

8. Import dữ liệu từ file csv mẫu vào trong bảng vừa tạo
<img width="1920" height="1080" alt="2026-04-08 (9)" src="https://github.com/user-attachments/assets/b9e1aec5-82c3-4eeb-b324-24a990400880" />

9. Kiểm tra xem số dòng của bảng dữ liệu sau khi import: Kết quả sẽ ok sẽ khoảng 12020 dòng.

Gõ lệnh: `SELECT COUNT(*) AS TongSoDong FROM SinhVien;`
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ab2e2c30-94a9-450f-8abf-fdd7016dfdad" />

10. INSERT thông tin cá nhân



