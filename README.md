📝 Notebook

Notebook là ứng dụng ghi chú cá nhân chạy trực tiếp trên trình duyệt, giúp bạn tạo, chỉnh sửa, tìm kiếm, sắp xếp và quản lý ghi chú một cách tiện lợi.

Ứng dụng có giao diện hiện đại, hỗ trợ WYSIWYG và Markdown, thư mục, tag, yêu thích, ghim, thùng rác, khóa ghi chú bằng mật khẩu, nhập/xuất dữ liệu và nhiều kiểu trình bày trang. Dữ liệu ghi chú được lưu cục bộ trong trình duyệt bằng IndexedDB.

✨ Tính năng

📝 Tạo và chỉnh sửa ghi chú

🔎 Tìm kiếm ghi chú theo tiêu đề và nội dung

⭐ Đánh dấu ghi chú yêu thích

📌 Ghim ghi chú quan trọng

🔒 Khóa ghi chú bằng mật khẩu

🗑️ Thùng rác và khôi phục ghi chú

📂 Tạo và quản lý thư mục

🏷️ Gắn Tag cho ghi chú

🎨 Chọn màu nhận diện cho từng ghi chú

😀 Tùy chỉnh emoji cho ghi chú

🌙 Dark Mode / Light Mode

🇻🇳 Tiếng Việt / 🇬🇧 English

💾 Tự động lưu thay đổi

📊 Hiển thị số từ và số ký tự

🖨️ In ghi chú

📋 Sao chép nội dung

✍️ Chế độ soạn thảo WYSIWYG

Markdown mode để làm việc với Markdown

Các tính năng trên được triển khai trực tiếp trong ứng dụng hiện tại.

📄 Định dạng trang

Notebook cung cấp 5 kiểu trình bày trang:

Kiểu

Mô tả

📄 Standard

Giao diện ghi chú tiêu chuẩn

📑 Lined

Trang có dòng kẻ ngang

🔲 Grid

Trang dạng ô vuông

💻 Code

Giao diện tối ưu cho nội dung mã nguồn

📖 Reader

Giao diện đọc tập trung

Các kiểu trang được tích hợp trực tiếp trong giao diện chỉnh sửa.

✍️ Trình soạn thảo

Ở chế độ WYSIWYG, Notebook hỗ trợ nhiều thao tác định dạng:

Bold

Italic

<u>Underline</u>

Chọn font

Thay đổi kích thước chữ

Đổi màu chữ

Highlight

Căn trái

Căn giữa

Căn phải

Danh sách

Nội dung HTML phong phú

Ngoài ra có thể chuyển sang Markdown mode để chỉnh sửa nội dung trực tiếp dưới dạng Markdown.

🔐 Khóa ghi chú

Notebook cho phép khóa từng ghi chú bằng mật khẩu.

Mật khẩu được chuyển thành SHA-256 hash trước khi lưu vào dữ liệu ghi chú, sau đó hash được sử dụng để xác thực khi mở khóa.

Lưu ý: Đây là cơ chế khóa ghi chú phía trình duyệt, không nên xem là giải pháp bảo mật cấp doanh nghiệp cho dữ liệu cực kỳ nhạy cảm.

💾 Lưu trữ dữ liệu

Notebook sử dụng IndexedDB để lưu dữ liệu cục bộ trên thiết bị.

Cơ sở dữ liệu hiện có các store cho:

Notes

Folders

Tags

Dữ liệu được đọc và ghi trực tiếp bằng API IndexedDB của trình duyệt.

⚠️ Lưu ý về dữ liệu

Vì dữ liệu được lưu trong trình duyệt, việc xóa dữ liệu website hoặc trình duyệt có thể làm mất ghi chú nếu bạn chưa sao lưu.

Nên sử dụng chức năng Export để tạo bản sao lưu định kỳ.

📤 Xuất dữ liệu

Notebook hỗ trợ xuất một ghi chú hoặc toàn bộ ghi chú.

Các định dạng hiện có:

.JSON
.TXT
.MD
.HTML
.DOCX
.PDF

Khi xuất nhiều ghi chú, ứng dụng có thể đóng gói chúng thành một file .ZIP.

📥 Nhập dữ liệu

Notebook hỗ trợ nhập:

.JSON
.TXT
.MD
.DOCX
.DOC
.HTML
.PDF

File Markdown được chuyển đổi thông qua marked, trong khi PDF được đọc bằng PDF.js để lấy nội dung văn bản.

🌐 Ngôn ngữ

Notebook hiện hỗ trợ:

🇻🇳 Tiếng Việt

🇬🇧 English

Bạn có thể chuyển đổi ngôn ngữ trực tiếp từ nút VI / EN trên giao diện.

🌙 Giao diện

Notebook hỗ trợ:

☀️ Light Mode

🌙 Dark Mode

Giao diện được xây dựng với Tailwind CSS và hỗ trợ dark mode thông qua class dark.

🛠️ Công nghệ sử dụng

Dự án được xây dựng theo hướng frontend, không yêu cầu backend riêng.

Core

HTML5

JavaScript

React 18

JSX thông qua Babel Standalone

UI

Tailwind CSS

Plus Jakarta Sans

Fira Code

Thư viện

CryptoJS

Marked

Turndown

JSZip

FileSaver.js

html2pdf.js

PDF.js

Các thư viện được tải trực tiếp từ CDN trong index.html.

📁 Cấu trúc dự án

Notebook/
│
├── index.html       # Ứng dụng Notebook
├── README.md        # Tài liệu dự án
└── CNAME            # Cấu hình domain GitHub Pages

Repository hiện sử dụng một file index.html làm ứng dụng chính, cùng với README.md và CNAME.

🚀 Chạy dự án

Cách 1 — Mở trực tiếp

Clone repository:

git clone https://github.com/alphatcx123-tech/Notebook.git

Đi vào thư mục:

cd Notebook

Sau đó mở:

index.html

bằng trình duyệt.

Cách 2 — Live Server

Nếu sử dụng VS Code, bạn có thể cài extension Live Server, sau đó chạy index.html thông qua Live Server.

🌍 Demo

Website:https://alphatcx123-tech.github.io/Notebook/

Repository cũng đang cấu hình CNAME và GitHub Pages cho dự án.

🔒 Quyền riêng tư

Notebook được thiết kế để lưu ghi chú trực tiếp trong trình duyệt thay vì yêu cầu một cơ sở dữ liệu backend.

Điều này giúp ghi chú có thể được sử dụng cục bộ trên thiết bị mà không cần triển khai server riêng.

📌 Lưu ý

Dữ liệu phụ thuộc vào bộ nhớ của trình duyệt.

Nên thường xuyên xuất dữ liệu để sao lưu.

Tính năng nhập/xuất phụ thuộc vào thư viện và khả năng xử lý của trình duyệt.

Cơ chế khóa ghi chú sử dụng SHA-256 để lưu hash mật khẩu, không phải mã hóa toàn bộ dữ liệu ghi chú bằng AES-256.

👨‍💻 Tác giả

ATCX

Repository:https://github.com/alphatcx123-tech/Notebook

📄 License

Repository hiện chưa khai báo file LICENSE riêng. Nếu muốn phát hành dự án dưới một giấy phép open-source cụ thể, nên bổ sung file LICENSE tương ứng.

<div align="center">

<strong>Notebook — Simple. Private. Organized.</strong>

<br><br>

© 2026 ATCX. All rights reserved.

</div>
