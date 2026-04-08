# **UX exercise — MoMo Moni AI**

## **Sản phẩm: MoMo — Moni AI Assistant (Phân loại chi tiêu)**

## **4 paths**

### **1\. AI đúng**

* Thực tế: Tự động gán icon chính xác cho các giao dịch phổ biến (Ăn uống, Mua sắm...).  
* User thấy gì: Thấy icon danh mục hiện đúng ở lịch sử giao dịch.  
* UI: Hiện tag \+ icon category, hệ thống confirm ngầm bằng cách tự động cộng tiền vào báo cáo tổng.

### **2\. AI không chắc**

* Thực tế: AI nhận định đưa ra được biểu đồ chi tiêu nhưng thực tế chỉ gen ra text.  
* Vấn đề: Thiếu khả năng trực quan hóa (Visualization), gây đứt gãy trải nghiệm.  
* Hệ quả: Thông tin rời rạc, buộc người dùng phải tự đối chiếu thủ công với biểu đồ hệ thống.

### **3\. AI sai**

* Lỗi logic nặng: Khi chi tiêu 0đ, hệ thống vẫn chấm điểm và khen "Quá xuất sắc luôn\!" kèm lời mời tiếp tục sử dụng.  
* Vấn đề: AI chạy theo kịch bản cứng (Scripted), không thực sự đọc dữ liệu thực tế.  
* Sửa: Khi phát hiện sai, user phải tự vào sửa thủ công (4 bước).

### **4\. User mất niềm tin**

* Hậu quả: User thấy context không hợp lý, báo cáo không thực tế (lỗi 0đ) nên không tin vào điểm số của AI.  
* Fallback: Quay lại cách quản lý truyền thống qua nút (+) nhập tay ở trang chủ (dễ tìm).  
* Exit: Có thể tắt tính năng hoặc đơn giản là thoát ra trang chủ để không sử dụng.

## **Path yếu nhất: Path 2 \+ 3**

* Path 2: Thiếu khả năng Visualization, chỉ nhìn được dữ liệu 7 ngày gần nhất nếu không nói kỹ hơn → thiếu sự tổng quát.  
* Path 3: Quy trình sửa lỗi quá thủ công. AI không hiểu ngữ cảnh khi gen câu trả lời, chỉ chạy theo kịch bản có sẵn và hay "quên" (mất lịch sử chat).

## **Gap marketing vs thực tế**

* Marketing: "Trợ lý tài chính thông minh", tự động phân loại chính xác, quản lý rảnh tay.  
* Thực tế: Chỉ là bộ lọc từ khóa đơn giản, dữ liệu ngắn hạn nên thiếu tính cá nhân hóa, so sánh  
* Gap lớn nhất:   
  1\. Hứa tra biểu đồ nhưng chỉ gen ra text, user phải tự so khớp dữ liệu.   
  2\. Data blindness: Không nhận diện được context "không chi tiêu" để điều chỉnh kịch bản phù hợp.

## **Sketch**

* As-is: Chi tiêu 0đ \-\> AI khen "Xuất sắc" sáo rỗng \-\> Thoát app \-\> Chỗ gãy: Mất sạch lịch sử chat, user phải hỏi lại từ đầu.  
* To-be: \- Fix Logic: Nếu chi tiêu 0đ \-\> AI đưa ra lời khuyên nên dùng MoMo thay vì khen vẹt.  
  * Fix Retention: Lưu lịch sử chat để user theo dõi lộ trình tư vấn xuyên suốt.  
  * Fix Path 3: Thêm Bulk Categorization \-\> AI học và sửa toàn bộ lỗi tương tự \-\> Hiện: "Đã học, lần sau sẽ chính xác hơn".

