# Biểu Đồ Kết Quả

Trang web hiển thị biểu đồ từ file Excel (.xlsx)

## Cách sử dụng

### Cách 1: Sử dụng với server (Khuyến nghị - tự động load data.xlsx)
1. Sử dụng Python server hoặc bất kỳ web server nào:
```bash
# Python 3
python3 -m http.server 8000

# Sau đó mở trình duyệt và truy cập:
# http://localhost:8000
```
2. Trang web sẽ tự động tải và hiển thị biểu đồ từ file `data.xlsx`

### Cách 2: Mở trực tiếp (chọn file thủ công)
1. Mở file `index.html` bằng trình duyệt web (Chrome, Firefox, Edge...)
2. Click vào nút "Chọn File Excel"
3. Chọn file `data.xlsx` hoặc file Excel khác của bạn
4. Các biểu đồ sẽ tự động hiển thị cho từng cột

### Cách 3: Deploy lên GitHub Pages
1. Tạo repository trên GitHub
2. Upload các file: `index.html` và `data.xlsx`
3. Vào Settings > Pages > Source: chọn branch main
4. Truy cập link GitHub Pages, trang web sẽ tự động load file `data.xlsx`

## Tính năng

- ✅ Đọc file Excel (.xlsx, .xls)
- ✅ Tự động phát hiện loại dữ liệu (số hoặc text)
- ✅ Biểu đồ đường (line chart) cho dữ liệu số
- ✅ Biểu đồ cột (bar chart) cho dữ liệu text/category
- ✅ Giao diện đẹp, hiện đại
- ✅ Responsive (hiển thị tốt trên mọi thiết bị)
- ✅ Không cần cài đặt thêm phần mềm

## Lưu ý

- File Excel nên có dòng đầu tiên là tiêu đề cột
- Mỗi cột sẽ được hiển thị thành một biểu đồ riêng
- Dữ liệu số sẽ hiển thị dưới dạng biểu đồ đường
- Dữ liệu text sẽ hiển thị dưới dạng biểu đồ cột (đếm số lần xuất hiện)
