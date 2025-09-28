# k58ktp_WEB_baitap1
nội dung bài tập 1

TẠO SOLUTION GỒM CÁC PROJECT SAU:

1. DLL đa năng, keyword: c# window library -> Class Library (.NET Framework) bắt buộc sử dụng .NET Framework 2.0: giải bài toán bất kỳ, độc lạ càng tốt, phải có dấu ấn cá nhân trong kết quả, biên dịch ra DLL. DLL độc lập vì nó ko nhập, ko xuất, nó nhận input truyền vào thuộc tính của nó, và trả về dữ liệu thông qua thuộc tính khác, hoặc thông qua giá trị trả về của hàm. Nó độc lập thì sẽ sử dụng được trên app dạng console (giao diện dòng lệnh - đen sì), cũng sử dụng được trên app desktop (dạng cửa sổ), và cũng sử dụng được trên web form (web chạy qua iis).
   
2. Console app, bắt buộc sử dụng .NET Framework 2.0, sử dụng được DLL trên: nhập được input, gọi DLL, hiển thị kết quả, phải có dấu án cá nhân. keyword: c# window Console => Console App (.NET Framework), biên dịch ra EXE
 
3. Windows Form Application, bắt buộc sử dụng .NET Framework 2.0**, sử dụng được DLL đa năng trên, kéo các control vào để có thể lấy đc input, gọi DLL truyền input để lấy đc kq, hiển thị kq ra window form, phải có dấu án cá nhân; keyword: c# window Desktop => Windows Form Application (.NET Framework), biên dịch ra EX
   
4. Web đơn giản, bắt buộc sử dụng .NET Framework 2.0, sử dụng web server là IIS, dùng file hosts để tự tạo domain, gắn domain này vào iis, file index.html có sử dụng html css js để xây dựng giao diện nhập được các input cho bài toán, dùng mã js để tiền xử lý dữ liệu, js để gửi lên backend. backend là api.aspx, trong code của api.aspx.cs thì lấy được các input mà js gửi lên, rồi sử dụng được DLL đa năng trên. kết quả gửi lại json cho client, js phía client sẽ nhận được json này hậu xử lý để thay đổi giao diện theo dữ liệu nhận dược, phải có dấu án cá nhân. keyword: c# window web => ASP.NET Web Application (.NET Framework) + tham khảo link chatgpt thầy gửi. project web này biên dịch ra DLL, phải kết hợp với IIS mới chạy được.


BÀI LÀM


1. DLL đa năng, keyword: c# window library -> Class Library (.NET Framework) bắt buộc sử dụng .NET Framework 2.0: giải bài toán bất kỳ, độc lạ càng tốt, phải có dấu ấn cá nhân trong kết quả, biên dịch ra DLL. DLL độc lập vì nó ko nhập, ko xuất, nó nhận input truyền vào thuộc tính của nó, và trả về dữ liệu thông qua thuộc tính khác, hoặc thông qua giá trị trả về của hàm. Nó độc lập thì sẽ sử dụng được trên app dạng console (giao diện dòng lệnh - đen sì), cũng sử dụng được trên app desktop (dạng cửa sổ), và cũng sử dụng được trên web form (web chạy qua iis)
Cấu hình project (Configure your new project)

<img width="1100" height="1005" alt="Screenshot 2025-09-28 211713" src="https://github.com/user-attachments/assets/0654a07d-af73-447c-8786-860de05b7674" />

- viết code trong project (triển khai logic của DLL).

<img width="1909" height="1080" alt="Screenshot 2025-09-28 212115" src="https://github.com/user-attachments/assets/79562ba1-7e53-4a18-b43e-fc0d259b4655" />


2. Console app, bắt buộc sử dụng .NET Framework 2.0, sử dụng được DLL trên: nhập được input, gọi DLL, hiển thị kết quả, phải có dấu án cá nhân. keyword: c# window Console => Console App (.NET Framework), biên dịch ra EXE
Cấu hình project (Configure Project).


<img width="1113" height="991" alt="Screenshot 2025-09-28 212800" src="https://github.com/user-attachments/assets/4adad2f8-43d1-4471-90f8-4223aadb0970" />



 - viết code (Code Implementation)-cài đặt logic ứng dụng.


<img width="1920" height="1080" alt="Screenshot 2025-09-28 213008" src="https://github.com/user-attachments/assets/c290a4b5-3e20-4fc5-84a3-5d97ff725bdd" />




3. Windows Form Application, bắt buộc sử dụng .NET Framework 2.0**, sử dụng được DLL đa năng trên, kéo các control vào để có thể lấy đc input, gọi DLL truyền input để lấy đc kq, hiển thị kq ra window form, phải có dấu án cá nhân; keyword: c# window Desktop => Windows Form Application (.NET Framework), biên dịch ra EXE

- Cấu hình project (Configure New Project).
<img width="1109" height="1012" alt="Screenshot 2025-09-28 213447" src="https://github.com/user-attachments/assets/627b1bfd-848d-4410-9bcc-ca05e5dce1fa" />


- Sau khi nhấn Create và Visual Studio sinh ra project: Form1.cs, From1.designer.cs, From1.designer

From1.cs
<img width="1917" height="1075" alt="Screenshot 2025-09-28 213737" src="https://github.com/user-attachments/assets/adff258c-d9b4-48c9-9678-eaa54a581c1f" />



From1.designer.cs

<img width="1920" height="1075" alt="Screenshot 2025-09-28 213637" src="https://github.com/user-attachments/assets/8fd96036-6e47-4b69-af93-0e9cf6dff5e1" />

<img width="1920" height="1080" alt="Screenshot 2025-09-28 213645" src="https://github.com/user-attachments/assets/e89baf76-934a-4ea4-868c-245eacab259f" />


<img width="1919" height="1077" alt="Screenshot 2025-09-28 213717" src="https://github.com/user-attachments/assets/9141dc72-e7c6-4580-8f21-fc0619276de6" />

<img width="1920" height="1080" alt="Screenshot 2025-09-28 213723" src="https://github.com/user-attachments/assets/ec19a73b-7c02-4863-8c33-9f601cf69fc6" />


From1.cs[design]


<img width="1920" height="1063" alt="Screenshot 2025-09-28 213619" src="https://github.com/user-attachments/assets/58315bc0-b369-4c17-8911-75ed5bd5045a" />



4. Web đơn giản, bắt buộc sử dụng .NET Framework 2.0, sử dụng web server là IIS, dùng file hosts để tự tạo domain, gắn domain này vào iis, file index.html có sử dụng html css js để xây dựng giao diện nhập được các input cho bài toán, dùng mã js để tiền xử lý dữ liệu, js để gửi lên backend. backend là api.aspx, trong code của api.aspx.cs thì lấy được các input mà js gửi lên, rồi sử dụng được DLL đa năng trên. kết quả gửi lại json cho client, js phía client sẽ nhận được json này hậu xử lý để thay đổi giao diện theo dữ liệu nhận dược, phải có dấu án cá nhân. keyword: c# window web => ASP.NET Web Application (.NET Framework) + tham khảo link chatgpt thầy gửi. project web này biên dịch ra DLL, phải kết hợp với IIS mới chạy được.

- Tạo project (Create New Project / Project Setup).
  
<img width="1102" height="1008" alt="Screenshot 2025-09-28 214100" src="https://github.com/user-attachments/assets/2c160798-5963-4e7f-8127-7744feb47e43" />

Cấu hình IIS

<img width="1902" height="1073" alt="Screenshot 2025-09-28 232431" src="https://github.com/user-attachments/assets/fba1d0e2-2175-4be4-b70e-bb50e608b108" />


phát triển và lập trình.

Giao diện (UI).

<img width="1887" height="990" alt="Screenshot 2025-09-28 232907" src="https://github.com/user-attachments/assets/4cd32f40-550a-4f7d-838b-fdf061a2d018" />



<img width="1881" height="987" alt="Screenshot 2025-09-28 232823" src="https://github.com/user-attachments/assets/ce274348-a3ee-403d-ac8f-c6b0452cb465" />



code-behind (logic)


<img width="1920" height="1080" alt="Screenshot 2025-09-28 232612" src="https://github.com/user-attachments/assets/63b162d1-6da3-4e68-9dad-668cf3b45dba" />


<img width="1914" height="983" alt="Screenshot 2025-09-28 232619" src="https://github.com/user-attachments/assets/48182011-68d8-48a1-b1de-5bcd6b46c869" />




html css js

<img width="1916" height="1075" alt="Screenshot 2025-09-28 215015" src="https://github.com/user-attachments/assets/07d15c36-eefb-4581-aede-7fd0cf50497e" />



<img width="1920" height="1080" alt="Screenshot 2025-09-28 215021" src="https://github.com/user-attachments/assets/1069f91b-b1e9-4a70-b648-e55487021a57" />



<img width="1920" height="1080" alt="Screenshot 2025-09-28 215029" src="https://github.com/user-attachments/assets/c821c72e-2664-4669-b217-d86f8c533f75" />









KẾT QUẢ

<img width="1920" height="1080" alt="Screenshot 2025-09-28 232254" src="https://github.com/user-attachments/assets/d17b75aa-5bde-47c7-9d81-4088faa70692" />








