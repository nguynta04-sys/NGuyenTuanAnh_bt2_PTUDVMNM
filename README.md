# NGuyenTuanAnh_bt2_PTUDVMNM
# Môn phát triển ứng dụng với mã nguồn mở 
# Lớp K58KTP
# bài tập 2
# SỬ DỤNG DJANGO ĐỂ TẠO WEB QUẢN LÝ TIỆM CẦM ĐỒ

Ngày làm: 08/05/2026

1. TỔ CHỨC CSDL CHO HỆ THỐNG QUẢN LÝ TIỆM CẦM ĐỒ
<img width="683" height="902" alt="image" src="https://github.com/user-attachments/assets/6cde42c2-2682-466f-ad6f-d1e7183dffdc" />
<img width="682" height="838" alt="image" src="https://github.com/user-attachments/assets/a8d3eb90-79ae-4b8a-841e-516f2851d354" />

2. SỬ DỤNG DOCKER TRÊN UBUNTU ĐỂ:
   - Tạo thư mục
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d1ad8ee0-c8c3-4184-8af9-a9405cf69b36" />

Thêm các dịch vụ vào trong file docker-compose.yml 
a. Mariadb : chứa csdl của hệ thống này
b. Phpmyadmin: để soi được csdl (chỉ để xem, ko cần tạo bảng từ đây, django sẽ làm hết)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/027986ac-18a7-471e-882e-ae0c75255225" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/54b6efbc-9a7d-440b-b171-7efebd25967b" />

File này là "công thức" để Docker biết phải cài những gì
<img width="662" height="25" alt="image" src="https://github.com/user-attachments/assets/f5319541-b29d-479d-9e1f-68329228e6de" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eab2670e-397f-4c2d-a4d4-6b4846d4a0ae" />

- Tạo file requirements.txt
Để khai báo các thư viện cần dùng
<img width="645" height="65" alt="image" src="https://github.com/user-attachments/assets/d57c94d7-2291-47dc-bdaf-3f20c1093cad" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4b37d22a-5fbf-4b5d-b4c9-cdc51448ff49" />

- Sửa file docker-compose.yml
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/58f6d2e0-551b-4450-a792-5d42e3498ee1" />

--> 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3bcd5077-dad0-40ff-9b6f-7250374aad08" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f554c8a7-ae96-451a-b08d-e9b3fab95b42" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4a836315-8b3d-4a8a-8321-e37128eb7651" />

- Khai báo dữ liệu trong file model.py để django xây dựng các bảng và liên kết tới mariadb:
  <img width="1083" height="634" alt="image" src="https://github.com/user-attachments/assets/5aa8f48c-67c4-43d6-9dae-da5b7ca46f63" />
- Chỉnh sửa file admin.py:
  <img width="1096" height="633" alt="image" src="https://github.com/user-attachments/assets/620c079d-7fc8-47d3-8d26-83d037883bb3" />
- Cập nhật database:
 <img width="884" height="218" alt="image" src="https://github.com/user-attachments/assets/8cff96c1-9be6-4d56-9d16-e5f4183cb34b" />
- Kết quả: đã có các bảng trong Django và PhPAdmin:
  
<img width="1815" height="654" alt="image" src="https://github.com/user-attachments/assets/ee77ec33-5b96-4efa-9c19-f69bdb1d54ef" />
<img width="1737" height="854" alt="image" src="https://github.com/user-attachments/assets/d1051854-6e95-4d6b-be1f-632e28f3b868" />

- Thao tác trên Django và kiểm tra trên phpadmin:
  <img width="1857" height="816" alt="image" src="https://github.com/user-attachments/assets/3b239aaa-7d72-4d67-addb-323125b00ff4" />
<img width="1860" height="816" alt="image" src="https://github.com/user-attachments/assets/485e81bb-42df-4677-9d40-2082018e664c" />
<img width="1875" height="854" alt="image" src="https://github.com/user-attachments/assets/6cb8811f-6345-438b-aea9-9c7536c380a6" />
<img width="1603" height="726" alt="image" src="https://github.com/user-attachments/assets/c60366e4-3068-4e9e-9078-8f50fec97017" />
<img width="1611" height="819" alt="image" src="https://github.com/user-attachments/assets/f32b6bd8-df5e-4496-9c47-08c6620d1c50" />

 - Cấu hình view.py
   <img width="1100" height="639" alt="image" src="https://github.com/user-attachments/assets/0189e843-e977-4ab7-bfef-a8e2a32b2b65" />

 - Tạo template html để xây dựng giao diện hiển thị danh sách các con nợ:
   <img width="1086" height="638" alt="image" src="https://github.com/user-attachments/assets/eb618c10-41c3-4f90-9247-f0e169ffdf04" />

- Cấu hình url.py:
  <img width="1099" height="636" alt="image" src="https://github.com/user-attachments/assets/25161540-16b5-451a-86ca-edd1db138100" />
- Cấu hình setting.py:
  <img width="1100" height="639" alt="image" src="https://github.com/user-attachments/assets/26fc508e-78da-42a0-a4dd-c1cfeaac4656" />
- Kết quả hiển thị của trang các con nợ:
  <img width="1801" height="694" alt="image" src="https://github.com/user-attachments/assets/320f00f3-5130-4fb0-9afe-0c227b26f20e" />

 - Sử dụng cloudflare tunnel để public kết quả lên 1 sub-domain:
   + Máy chủ:
   <img width="1854" height="664" alt="image" src="https://github.com/user-attachments/assets/0f19a938-2411-42bd-9b48-1b46ec52fecd" />
   + Máy Khách:
   <img width="870" height="1883" alt="image" src="https://github.com/user-attachments/assets/b9f7e95c-e813-408b-b88b-da18e43f0b49" />


