# BÀI LÀM PHA 2

  

-  **Họ tên:** Hà Duy Mạnh 

-  **Lớp:** CNTT1

-  **Link repository Pha2:**[https://github.com/adaptable14/HN-K26-CNTT1_PromptAI_Pha1-Pha2](https://github.com/adaptable14/HN-K26-CNTT1_PromptAI_Pha1-Pha2)

-  **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** Chat GPT

  

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

  

## 4.2. Trích xuất tin nhắn đặt vé ra JSON

  

**KET QUA AI**

  

```[
  {
    "ma_dich_vu": "TRAM",
    "ngay_hen": "2026-12-17",
    "nguoi_lon": 2,
    "tre_em": 1,
    "khung_gio": "chieu",
    "ghi_chu": null
  },
  {
    "ma_dich_vu": "CAOVOI",
    "ngay_hen": "2027-01-06",
    "nguoi_lon": 3,
    "tre_em": 0,
    "khung_gio": null,
    "ghi_chu": "Một người bị tiểu đường"
  },
  {
    "ma_dich_vu": "TAYTRANG",
    "ngay_hen": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "khung_gio": "sang",
    "ghi_chu": "Một người dị ứng thuốc tê"
  }
]


```

  

- **Link trò chuyện:**:https://chatgpt.com/share/6b07e5a1-5058-83ec-bfda-6490a2939ad5

  

## 4.3. Báo giá vé bằng Chain-of-Thought

  

**KET QUA AI**

  



### **a) Prompt**

**PROMPT**


Bạn là nhân viên tư vấn báo giá dịch vụ nha khoa.

NHIỆM VỤ:
Hãy tính tổng tiền cho yêu cầu báo giá dựa trên bảng giá và quy tắc tính giá được cung cấp.

YÊU CẦU:
Thực hiện tính toán từng bước theo đúng thứ tự sau và ghi rõ công thức, phép tính và kết quả:

1. Tiền người lớn:
   - Lấy số người lớn nhân với giá dịch vụ tương ứng.

2. Tiền trẻ em:
   - Trẻ từ 6 đến 12 tuổi tính 80% giá người lớn.
   - Trẻ dưới 6 tuổi được khám miễn phí.

3. Tiền vé:
   - Cộng tiền người lớn và tiền trẻ em.

4. Giảm giá nhóm:
   - Nhóm có từ 5 người lớn trở lên được giảm 10% trên tiền dịch vụ.
   - Tính rõ số tiền được giảm.

5. Phí X-quang:
   - Mỗi phim có giá 150.000 đồng.
   - Phí X-quang không được giảm giá.

6. Tổng tiền:
   - Tổng tiền = Tiền dịch vụ sau giảm + Phí X-quang.

BẢNG GIÁ DỊCH VỤ:
- CAOVOI – Khám và cạo vôi răng: 350.000 đồng/người.
- TRAM – Trám răng thẩm mỹ (1 răng): 500.000 đồng/người.
- TAYTRANG – Tẩy trắng răng: 2.500.000 đồng/người.

QUY TẮC:
- Không tự ý thay đổi bảng giá.
- Không bỏ qua bất kỳ bước tính toán nào.
- Không áp dụng giảm giá cho phí X-quang.
- Trình bày kết quả rõ ràng, dễ hiểu.
- Không tự suy đoán thông tin ngoài dữ liệu được cung cấp.

YÊU CẦU BÁO GIÁ:
Nhóm nhân viên công ty sử dụng dịch vụ CAOVOI gồm:
- 6 người lớn.
- 2 trẻ em (7 tuổi và 11 tuổi).
- 1 bé 4 tuổi.
- Có 3 người cần chụp X-quang, mỗi người 1 phim.

ĐỊNH DẠNG ĐẦU RA:
Trình bày đầy đủ 6 bước tính toán theo đúng thứ tự.

Dòng cuối cùng bắt buộc phải viết đúng mẫu:
[RESULT: <tổng tiền> đồng]





  

- **Link trò chuyện:** :https://chatgpt.com/share/6b07e617-4de8-83ec-8044-cfc6cdb5c47e

  

### b) Kiểm tra kết quả AI



**1. Tiền người lớn:**

6 × 350.000 = 2.100.000 đồng.

**2. Tiền trẻ em:**

-   Trẻ 7 tuổi: 350.000 × 80% = 280.000 đồng.
    
-   Trẻ 11 tuổi: 350.000 × 80% = 280.000 đồng.
    
-   Bé 4 tuổi: Miễn phí = 0 đồng.
    

Tổng tiền trẻ em:

280.000 + 280.000 + 0 = 560.000 đồng.

**3. Tiền vé:**

2.100.000 + 560.000 = 2.660.000 đồng.

**4. Giảm giá nhóm:**

Nhóm có 6 người lớn nên được giảm 10%.

2.660.000 × 10% = 266.000 đồng.

Tiền sau giảm:

2.660.000 − 266.000 = 2.394.000 đồng.

**5. Phí X-quang:**

3 × 150.000 = 450.000 đồng.

**6. Tổng tiền:**

2.394.000 + 450.000 = 2.844.000 đồng.

[RESULT: 2.844.000 đồng]

  

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

  

**KET QUA AI**

  



### **a) PROMPT – Trạm 1**

```
Đọc email khiếu nại trong thẻ Trạm 1 – đọc email.

Trả về duy nhất một đối tượng JSON gồm đúng 4 trường:

{
  "loai_su_co": "tre_hen" | "thiet_bi" | "bac_si" | "khac",
  "so_khach": số nguyên,
  "so_lan_hen_bi_tre": số nguyên hoặc null,
  "tom_tat": "không quá 20 từ"
}

Yêu cầu:
- Xác định đúng loại sự cố dựa trên nội dung email.
- Không tự suy đoán thông tin không có trong email.
- Nếu không có thông tin về số lần hẹn bị trễ, trả về null.
- Tóm tắt nội dung khiếu nại không quá 20 từ.
- Không thêm giải thích bên ngoài JSON.
```

### **b) Hai điều cần kiểm tra ở JSON đầu ra của Trạm 1**

**1. Kiểm tra cấu trúc JSON**

-   Có đúng 4 trường không?
    
-   Tên trường có chính xác không?
    
-   Kiểu dữ liệu có đúng không?
    
    -   `loai_su_co`: chuỗi.
        
    -   `so_khach`: số nguyên.
        
    -   `so_lan_hen_bi_tre`: số nguyên hoặc `null`.
        
    -   `tom_tat`: chuỗi không quá 20 từ.
        
    
-   JSON có dấu ngoặc kép, dấu phẩy đúng vị trí không?
    

**2. Kiểm tra nội dung có đúng email không**

-   `loai_su_co` phải phản ánh đúng nguyên nhân khiếu nại.
    
-   Không được xếp nhầm `tre_hen` nếu vấn đề thực tế là nhân viên xếp nhầm lịch.
    
-   `so_khach` phải đúng số lượng khách được đề cập.
    
-   `so_lan_hen_bi_tre` phải đúng thông tin trong email.
    
-   `tom_tat` phải ngắn gọn và đúng nội dung.
    

### **c) CÂU LỆNH VIẾT TIẾP**

```
Viết tiếp đoạn phản hồi ngay từ chỗ bị ngắt dưới đây, không lặp lại phần đã viết:

"... Nha Khoa nụ cười xin hoàn lại quý khánh Khoản "

Yêu cầu:
- Viết tiếp tự nhiên, lịch sự và chuyên nghiệp.
- Giữ đúng ngữ cảnh email phản hồi khiếu nại.
- Nêu rõ khoản tiền hoàn lại nếu có dữ liệu.
- Đưa ra lời xin lỗi và cam kết cải thiện dịch vụ.
- Không tự bịa số tiền hoặc thông tin chưa được cung cấp.
- Chỉ viết phần tiếp theo, không viết lại đoạn trước.
```



  

**Link trò chuyện:**:https://chatgpt.com/share/6b07e6d4-9d94-83ec-a994-ae0b1dc34c3a

  

## 4.5. Prompt chấm bài theo Rubric

  

**KET QUA AI**

  


### **1. Các lỗi bị trừ điểm**

**Lỗi 1: Sai giá dịch vụ**

-   **Câu bị lỗi:** “Trám răng bên em 450k/răng thôi”
    
-   **Lý do sai:** Giá chuẩn của dịch vụ TRAM là 500.000 đồng/răng, không phải 450.000 đồng/răng.
    
-   **Câu sửa lại:** “Dạ, dịch vụ trám răng bên em có giá 500.000 đồng/răng ạ.”
    

**Lỗi 2: Cam kết kết quả không có căn cứ**

-   **Câu bị lỗi:** “đẹp như răng thật luôn.”
    
-   **Lý do sai:** Nhân viên cam kết kết quả tuyệt đối mà chưa có thông tin đánh giá tình trạng răng của khách.
    
-   **Câu sửa lại:** “Dạ, trám răng giúp cải thiện hình dáng và thẩm mỹ của răng. Kết quả cụ thể sẽ tùy thuộc vào tình trạng răng của anh ạ.”
    

**Lỗi 3: Sai chính sách bảo hành**

-   **Câu bị lỗi:** “Bong sau 8 tháng thì em làm lại free cho anh nha.”
    
-   **Lý do sai:** Theo chính sách, từ tháng 7 đến tháng 12 khách chỉ được giảm 50%, không được làm lại miễn phí.
    
-   **Câu sửa lại:** “Nếu miếng trám bong sau 8 tháng, anh sẽ được giảm 50% chi phí khi làm lại ạ.”
    

**Lỗi 4: Chưa mời khách cung cấp thông tin đặt lịch**

-   **Câu bị lỗi:** “Cần gì cứ inbox em ạ!”
    
-   **Lý do sai:** Chưa chủ động hỏi ngày hẹn và khung giờ mong muốn để hỗ trợ đặt lịch.
    
-   **Câu sửa lại:** “Anh vui lòng cho em biết ngày hẹn và khung giờ mong muốn để em hỗ trợ đặt lịch ạ.”
    

**Lỗi 5: Giọng điệu chưa chuyên nghiệp**

-   **Câu bị lỗi:** “450k/răng thôi”, “free”, “nha”, “Cần gì cứ inbox em ạ!”
    
-   **Lý do sai:** Sử dụng một số từ ngữ thân mật, chưa phù hợp với phong cách tư vấn chuyên nghiệp.
    
-   **Câu sửa lại:** Sử dụng cách diễn đạt lịch sự như “500.000 đồng/răng”, “miễn phí”, “ạ” và “Em sẵn sàng hỗ trợ anh”.
    

### **2. Bảng chấm điểm theo Rubric**

Tiêu chí

Điểm

Minh chứng

Đề xuất sửa

Đúng thông tin (50%)

1/5

Sai giá dịch vụ và sai chính sách bảo hành.

Sửa giá thành 500.000 đồng/răng, bảo hành tháng 8 giảm 50%.

Đầy đủ (30%)

1/3

Có trả lời câu hỏi nhưng chưa giải thích rõ kết quả thẩm mỹ và chưa hỏi ngày, giờ đặt lịch.

Bổ sung tư vấn và lời mời đặt lịch.

Giọng điệu (20%)

1/2

Có lời chào lịch sự nhưng sử dụng từ ngữ suồng sã.

Sử dụng ngôn ngữ lịch sự, chuyên nghiệp.

**Tổng cộng**

**3/10**

**Còn nhiều lỗi về thông tin và tư vấn.**

**Cần chỉnh sửa trước khi sử dụng.**

### **3. Câu trả lời tư vấn sau khi sửa**

“Dạ, em chào anh! Dịch vụ trám răng bên em có giá 500.000 đồng/răng. Phương pháp này giúp cải thiện hình dáng và thẩm mỹ của răng, kết quả cụ thể tùy thuộc vào tình trạng răng của anh. Về bảo hành, nếu miếng trám bong trong 6 tháng đầu, bên em sẽ làm lại miễn phí; từ tháng thứ 7 đến tháng thứ 12, anh được giảm 50% chi phí làm lại. Anh vui lòng cho em biết ngày hẹn và khung giờ mong muốn để em hỗ trợ đặt lịch ạ.”

**TỔNG ĐIỂM: 3/10.**




  

**Link trò chuyện:**:https://chatgpt.com/share/6b07e71d-73fc-83ec-abde-6a91a55a9092


