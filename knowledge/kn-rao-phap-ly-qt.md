# RÀO PHÁP LÝ — Quảng cáo thẩm mỹ cho thị trường QUỐC TẾ
Version: 1.0 — 2026-10-21
Áp cho **MỌI** output. Agent tự rà trước khi xuất. Chạm ranh → gắn cờ ⚠️ chờ người duyệt. **Fail = không xuất.**

---

## §0. HAI TẦNG PHÁP LÝ — đọc trước mọi thứ khác

Nội dung của gói này chịu **hai hệ luật cùng lúc**:

| Tầng | Áp vì | Luôn áp? |
|---|---|---|
| ① **Luật Việt Nam** | Cơ sở ở VN, dịch vụ là khám chữa bệnh. Cần **giấy xác nhận nội dung quảng cáo** của cơ quan y tế | ✅ **Luôn**, bất kể khách ở đâu |
| ② **Luật nước người xem** | Nền tảng áp chính sách theo **vị trí người nhìn thấy quảng cáo** | ✅ Theo từng `market` |

→ Một mẫu hợp pháp ở VN **vẫn có thể** bị từ chối hoặc bị cơ quan nước đích xử lý.
→ Mỗi output phải ghi rõ **đang nhắm `market` nào** và **đã rà theo luật nước nào**.

⛔ **Agent không đưa ra kết luận pháp lý.** Agent nêu tên cơ quan phải tra, gắn cờ rủi ro, đề xuất biến thể hạ rủi ro. Dòng kết luận luôn là: *"cần Pháp chế xác nhận cho thị trường [X] trước khi bật."*

> ⚠️ **File này áp cho CẢ hai kênh:** quảng cáo trả tiền **và** nội dung GEO (câu trả lời AI). Nhầm lẫn phổ biến nhất là tưởng *"nội dung tiếng Anh thì không cần GXNNDQC"* — **sai**: nội dung EN vẫn chịu luật quảng cáo & KCB Việt Nam (rào **R9**). Bảng rào R0–R9 đầy đủ ở [`kn-truy-van-geo-qt.md`](kn-truy-van-geo-qt.md) §7.

---

## §1. BẢNG TỪ CẤM → TỪ ĐÚNG (tiếng Anh)

Đây là bảng dùng để **tự quét mọi output tiếng Anh**. Quét cả headline · description · primary text · copy landing · từ khoá · thông điệp.

| ⛔ Cấm | ✅ Thay bằng |
|---|---|
| best / the best / No.1 / #1 / top-rated / leading / finest / premier | *(bỏ)* hoặc USP đo được: *"licensed by the Vietnamese Ministry of Health"* |
| guaranteed results / guaranteed success / 100% success | *"outcomes are assessed individually by the surgeon"*\* |
| permanent / permanent results / forever / lifetime results | *"long-lasting; ageing or trauma can change the result over time"*\* |
| **lifetime warranty** *(không có T&C)* | *"follow-up and warranty policy — see terms"* + `[PENDING: warranty T&C — Legal]` |
| painless / pain-free / no pain | *"pain is managed under an anaesthesia protocol prescribed by the surgeon"* |
| no scars / scar-free | *"incision sites are chosen to minimise visible scarring; outcome depends on aftercare"*\* |
| no complications / risk-free / completely safe / absolutely safe | *"performed in a sterile operating theatre under a documented surgical protocol, reviewed by the medical board"* |
| perfect / flawless | *"a result in proportion with your face"*\* |
| cheapest / unbeatable price / lowest price in Asia | *"published price list — 10% international service charge applies"* |
| **"70% cheaper than Australia"** và mọi so sánh giá có tên quốc gia/cơ sở | *"Our full price list is published. Compare it yourself."* — để bảng giá nói thay *(luật ③)* |
| **"back to work in 3 days"** và mọi mốc hồi phục/ở lại CỨNG | khoảng + *"varies by case"* + nêu rõ mốc nào *(luật ②)* |
| miracle / life-changing / transform your life | mô tả kết quả cụ thể, kiểm chứng được |
| **"board certified"** khi chỉ có tư cách hội | *"member of [society]"* gắn **đúng tên cá nhân** — và chỉ khi đủ 3 điều kiện *(luật ④)* |
| FDA approved / FDA certified *(nói về dịch vụ)* | chỉ nói về **vật liệu cụ thể có hồ sơ**, nêu đúng tên; không gắn cho dịch vụ |
| overweight / fat / obese *(ngôn từ về cân nặng)* | *(bỏ hẳn)* — vi phạm policy Meta/Google ở mọi thị trường *(luật ⑤)* |

Mọi con số và cam kết mức độ gắn dấu `*` dẫn chú thích: ***"Results vary by individual."*** *(nguyên văn disclaimer site đang dùng — dùng lại đúng câu này)*

---

## §2. HÌNH ẢNH / VIDEO — theo thị trường

| Loại | Tầng A (KH·LA·ID·PH·MY·IN) | Tầng B/D (kiều bào · expat) | **Tầng C (AU·UK·EU·US·GCC)** |
|---|---|---|---|
| **Before–after mặt** | ✅ nếu có văn bản đồng ý + đã duyệt | ✅ nếu có văn bản đồng ý + đã duyệt | 🔴 **Mặc định KHÔNG** — cần Pháp chế duyệt riêng từng thị trường |
| **Before–after cơ thể / giảm béo** | ⛔ không | ⛔ không | ⛔ **không** |
| **Testimonial về kết quả lâm sàng** | ✅ nếu thật | ✅ nếu thật | 🔴 **KHÔNG** — AHPRA (Úc) cấm thẳng |
| **Testimonial về trải nghiệm phi lâm sàng** *(phiên dịch · đưa đón · khách sạn · thái độ nhân viên)* | ✅ | ✅ | ✅ **dùng được** — đây là lối đi hợp lệ cho tầng C |
| Ảnh bác sĩ · phòng mổ · cơ sở · thiết bị | ✅ ảnh thật của hệ thống | ✅ | ✅ |
| Cận cảnh thao tác mổ · máu · vết mổ | ⛔ | ⛔ | ⛔ |
| **Ảnh stock / ảnh AI** thay cho trust | ⛔ | ⛔ | ⛔ |

**Luật nền:** ⛔ **không tạo ảnh kết quả giả**, không dùng ảnh stock/AI mô phỏng kết quả rồi trình bày như case thật. Chưa có ảnh thật đã duyệt → **ô ảnh tạm** theo mẫu `kn-khung-landing-qt.md`.

---

## §3. FORM & DỮ LIỆU CÁ NHÂN — rào riêng của gói QT

Gói nội địa chỉ cần checkbox đồng ý xử lý dữ liệu cá nhân. Gói QT **không đủ** như thế.

| Thị trường | Yêu cầu thêm | Mức |
|---|---|---|
| **EU / EEA / UK** | **GDPR / UK GDPR**: cơ sở pháp lý rõ ràng (consent), thông báo quyền của chủ thể dữ liệu, **và nêu rõ việc chuyển dữ liệu sang Việt Nam** (nước thứ ba). Dữ liệu sức khoẻ là **special category** → mức bảo vệ cao nhất | 🔴 **Chặn** nếu thiếu |
| **Úc** | Privacy Act / APPs — thông báo thu thập + tiết lộ ra nước ngoài | 🔴 Chặn nếu thiếu |
| **Canada** | PIPEDA | 🟠 |
| **Việt Nam** | Quy định bảo vệ dữ liệu cá nhân hiện hành | ✅ Luôn |
| **Mọi thị trường** | Ảnh khách gửi để *pre-consultation* là **dữ liệu sức khoẻ** | 🔴 Luôn |

**Năm luật cứng cho form quốc tế:**
① Checkbox đồng ý **không được tick sẵn**, và phải nêu rõ dữ liệu được chuyển sang **Việt Nam**.
② Link **privacy policy** phải có và phải mở được trước khi submit.
③ Ảnh gửi cho bước *pre-consultation* phải có dòng riêng nêu rõ: ai xem · lưu ở đâu · bao lâu · có dùng cho marketing không *(mặc định: **không**)*.
④ ⛔ **Không** nạp ảnh khách · hộ chiếu · hồ sơ bệnh án lên công cụ công cộng (gồm cả công cụ AI).
⑤ Nhắm **EU/UK** mà chưa có bản privacy notice đạt GDPR → **không bật chiến dịch**, ghi `[BLOCKED: GDPR notice — Legal]`.

> ⚠️ Form trên trang tham chiếu hiện thu: name · phone + country code · email · **nationality** · country · location · referred · preferred date · gender · kênh nhắn tin. Trường `nationality` + ảnh → **đã là dữ liệu đủ để chịu GDPR** khi khách ở EU/UK.

---

## §4. SÁU LUẬT RIÊNG CỦA GÓI QUỐC TẾ

**① KHÔNG chạy nội dung chưa khai `market`.** Không biết người xem ở đâu thì không biết luật nào áp. Dòng từ khoá hoặc mẫu quảng cáo thiếu `market` → **không xuất**.

**② KHÔNG hứa số ngày ở lại hoặc mốc hồi phục cứng.** Với gói QT, con số này nặng hơn gói nội địa vì nó quyết định **ngày bay**. Bay quá sớm sau phẫu thuật là **rủi ro y khoa thật**, không chỉ là copy sai. Luôn dạng khoảng + *"varies by case"* + nêu rõ mốc (cắt chỉ · tái khám cuối · được phép bay). Chưa có số từ Khoa Chuyên môn → `[PENDING: minimum stay — Medical Dept]`.

**③ KHÔNG so sánh giá với một quốc gia hoặc cơ sở có tên.** *"Cheaper than Korea"* · *"70% less than Australia"* là claim cần bằng chứng, và ở AU/UK là rủi ro quảng cáo. Cách hợp lệ: **công bố bảng giá đầy đủ** và để khách tự so. Và **luôn** kèm 3 dòng bắt buộc của bảng giá (`kn-ho-so-thuong-hieu-qt.md` §6).

**④ KHÔNG dùng claim hội–hiệp hội ở mức thương hiệu.** VSAPS · ASPS · ASAPS · ISAPS · AAFPRS chỉ được nêu khi đủ **ba điều kiện**: gắn **đúng tên cá nhân** · có **hồ sơ thành viên còn hiệu lực** tại Pháp chế · **không** trình bày như board certification hoặc giấy phép hành nghề. Thiếu một điều kiện → bỏ claim.
*Vì sao:* tư cách hội là của từng người. Viết ở mức thương hiệu/ekip là claim **không kiểm chứng được**, và nhầm nó với board certification là điểm bị chất vấn nhiều nhất ở US/AU.
*Xung đột đã biết:* site quốc tế đang hiển thị các hội này ở mức thương hiệu, trong khi gói nội địa cấm thẳng. **Pháp chế phải chốt một dòng dùng chung cho cả hai site.** Chi tiết: `kn-ho-so-thuong-hieu-qt.md` §4.2.

**⑤ KHÔNG dùng ngôn từ về cân nặng và không dùng before–after cơ thể.** Vi phạm policy Meta/Google ở mọi thị trường, không riêng thị trường nào.

**⑥ KHÔNG giới thiệu 5 viện thẩm mỹ tỉnh cho khách quốc tế.** Site quốc tế chỉ công bố 2 cơ sở, **cả hai là tuyến bệnh viện**. Đưa viện tỉnh vào nội dung quốc tế là tự tạo lại bẫy vượt phạm vi giấy phép mà gói này vốn không có.

---

## §4b. BỐN RÀO CỨNG TỪ BỘ TRUY VẤN GEO — bổ sung 2026-10-21

Bốn rào dưới đây đến từ `HCI-Knowledge/GEOQUOCTE.xlsx` (bảng rào R0–R9). Chúng **không có trong v1.0 của file này**, và đó là một lỗ thật — cả bốn đều là **rào cứng**, áp cho **cả nội dung GEO và quảng cáo trả tiền**.

Bảng R0–R9 đầy đủ: [`kn-truy-van-geo-qt.md`](kn-truy-van-geo-qt.md) §7.

| Mã | Rào | ⛔ Không được | ✅ Thay bằng | Người duyệt |
|---|---|---|---|---|
| **R2** | **Danh mục kỹ thuật (DMKT)** | Quảng cáo kỹ thuật **ngoài danh mục đã phê duyệt** của cơ sở — cụ thể **deep plane · BBL · abs etching** | Chỉ nêu kỹ thuật **thuộc DMKT đã phê duyệt** | Pháp chế |
| **R3** | **Đúng pháp nhân** — ĐIỂM NÓNG | Site EN **gộp nhiều cơ sở/pháp nhân**; dùng tên "Kangnam" cho dịch vụ mà cơ sở đó **không có phạm vi** | Site EN trỏ **đúng bệnh viện có giấy phép + phạm vi**; NAP từng cơ sở | Pháp chế |
| **R7** | **Túi ngực · thiết bị · filler** | Nêu hãng **không dùng thật**; máy/filler **không rõ số lưu hành** | Chỉ hãng **thực dùng, có số lưu hành** + chứng nhận; khách được xem thẻ | BS + Pháp chế |
| **R8** | **KCB cho người nước ngoài** — **NÓNG NHẤT** | Tiếp nhận khách nước ngoài khi **cơ sở/bác sĩ chưa đủ điều kiện**, hoặc **không có phiên dịch chuyên môn** | Đủ điều kiện pháp lý + phiên dịch + **hồ sơ song ngữ** + kênh theo dõi từ xa | Pháp chế + Điều phối QT |

### 🔴 R8 là rào quan trọng nhất mà gói này từng thiếu

R2 · R3 · R7 nói về **câu chữ**. **R8 nói về việc có được tiếp nhận khách hay không** — nó không phải rào nội dung, nó là **điều kiện hoạt động**.

→ Một chiến dịch chạy tốt, landing chấm 90 điểm, mẫu quảng cáo 14/14 — nhưng cơ sở **chưa đủ điều kiện R8** thì **lead đổ về là rủi ro, không phải thành tích**.
→ R8 áp cho **toàn bộ site EN**, không riêng một cụm nào.
→ **Luật:** trước khi bật bất kỳ chiến dịch quốc tế nào, Agent phải nhắc người dùng xác nhận R8 — và ghi `[PENDING: R8 — đủ điều kiện KCB cho người nước ngoài · Pháp chế + Điều phối QT]` vào danh sách cuối output.

### Hai dịch vụ phải chốt trước khi làm bất kỳ nội dung nào

| Dịch vụ | Phải chốt gì | Vì sao |
|---|---|---|
| **Nha khoa** *(Q08 — dental tourism)* | **Pháp nhân RHM**: Kangnam Dental hay Nha Khoa Paris | R3. Dental tourism có nhu cầu lớn nhưng sai pháp nhân là sai phạm vi giấy phép |
| **BBL** *(Q09 — Brazilian butt lift)* | ① kỹ thuật **có trong DMKT** của cơ sở không · ② nội dung **nói thật rủi ro thuyên tắc mỡ** | R2. Đây là thủ thuật **rủi ro cao nhất ngành**. Chỉ định phải chặt |

⛔ Chưa chốt → **không viết nội dung, không chạy từ khoá** cho hai nhóm này.

---

## §5. KHÔNG ĐƯỢC LÀM

- **Không chẩn đoán** qua ảnh/mô tả, **không kê đơn**, **không báo giá ca cụ thể** — chỉ tư vấn định hướng rồi mời thăm khám. Với gói QT, bước *pre-consultation dựa trên ảnh* trên site **là của bác sĩ**, không phải của Agent: Agent không được viết nội dung mô phỏng một đánh giá y khoa.
- **Không nêu tên hạ thấp đối thủ** — gồm cả cơ sở ở Thái Lan, Hàn Quốc, Thổ Nhĩ Kỳ. So sánh bằng bộ tiêu chí khách quan để khách tự đánh giá.
- **Không hứa visa, thư mời, hay kết quả nhập cảnh** — chưa có xác nhận từ bộ phận quốc tế thì để `[PENDING]`.
- **Không hứa thanh toán / hoàn tiền / chi trả chi phí bay cho ca chỉnh sửa** khi chưa có T&C bằng văn bản.
- **Không dùng máy dịch** cho nội dung y khoa ở ngôn ngữ không phải tiếng Anh. Chưa có người bản ngữ rà → `[PENDING: native review — <ngôn ngữ>]`, không bật.

---

## §6. HUMAN-IN-THE-LOOP — bắt buộc duyệt trước khi chạy

Mọi mẫu quảng cáo · landing · bảng giá · nội dung có phát ngôn bác sĩ · before–after · bản dịch là **bản đề xuất chờ duyệt**.

**Bốn cửa duyệt của gói QT:**
① **Pháp chế VN** — luật quảng cáo y tế + giấy xác nhận nội dung quảng cáo.
② **Pháp chế / cố vấn thị trường đích** — cho `market` thuộc AU · UK · EU · US · GCC.
③ **Khoa Chuyên môn** — mọi phát ngôn y khoa, **và số ngày ở lại**.
④ **Người bản ngữ** — mọi bản dịch không phải tiếng Anh.

---

## §7. 🔶 CẦN XÁC NHẬN TRƯỚC KHI BẬT CHIẾN DỊCH

| # | Hạng mục | Trạng thái |
|---|---|---|
| 1 | Số giấy xác nhận nội dung quảng cáo cho từng nội dung/chiến dịch | `[CHỜ CẬP NHẬT]` |
| 2 | **Dòng claim hội–hiệp hội dùng chung cho hai site** *(luật ④)* | `[CHỜ CẬP NHẬT]` |
| 3 | **T&C bảo hành / chỉnh sửa** — phạm vi · thời hạn · loại trừ · ai trả chi phí bay | `[CHỜ CẬP NHẬT]` |
| 4 | **Số ngày tối thiểu ở VN** từng dịch vụ | `[CHỜ CẬP NHẬT]` |
| 5 | Privacy notice đạt **GDPR/UK GDPR** + thông báo chuyển dữ liệu sang VN | `[CHỜ CẬP NHẬT]` |
| 6 | Danh sách case + ảnh **đã có văn bản đồng ý**, và đồng ý đó **có phạm vi quốc tế** hay không | `[CHỜ CẬP NHẬT]` |
| 7 | Rà quảng cáo theo thị trường đích: AU (AHPRA) · UK (ASA/CAP) · US (FTC) · GCC | `[CHỜ CẬP NHẬT]` |
| 8 | **Muslim-Friendly Care gồm những gì** — claim vô nghĩa nếu không khai cụ thể | `[CHỜ CẬP NHẬT]` |
| 9 | Hỗ trợ visa / thư mời — có hay không | `[CHỜ CẬP NHẬT]` |
| 10 | Phương thức thanh toán quốc tế + mức đặt cọc | `[CHỜ CẬP NHẬT]` |
| 11 | **Gỡ 3 lỗi trên trang tham chiếu**: tên *"Dr. Granzow"* · *"Trusted by 0+ clients"* · *"results are permanent"* | `[CHỜ CẬP NHẬT]` |
| 12 | 🔴 **R8 — cơ sở + bác sĩ đủ điều kiện KCB cho người nước ngoài**, có phiên dịch chuyên môn và hồ sơ song ngữ | `[CHỜ CẬP NHẬT]` |
| 13 | **R2 — danh mục kỹ thuật (DMKT)** đã phê duyệt của từng cơ sở: deep plane · BBL · abs etching có trong danh mục không | `[CHỜ CẬP NHẬT]` |
| 14 | **R3 — pháp nhân cho site EN**, và riêng **nha khoa: Kangnam Dental hay Nha Khoa Paris** | `[CHỜ CẬP NHẬT]` |
| 15 | **R7 — số lưu hành** của túi ngực · thiết bị · filler thực dùng | `[CHỜ CẬP NHẬT]` |

Dòng 11 là lỗi đang hiển thị trên bản live — xem `kn-ho-so-thuong-hieu-qt.md` §4.4.

---

## §8. CỔNG TỰ ĐỘNG

`tools/build_keyword_workbook.py` **chặn build** nếu:
- `thong_diep` hoặc `tu_khoa` chứa từ cấm ở §1 (bản tiếng Anh **và** tiếng Việt cho tầng B);
- dòng từ khoá có tên thành phố VN mà **không khai** `market` + `geo_mode` *(cổng GEO-TARGET)*;
- dòng từ khoá thuộc `market` nhóm **rủi ro cao** (AU · UK · EU · GCC) mà `ghi_chu` **chưa khai** cách xử lý creative rủi ro *(cổng REGULATED)*;
- còn claim `lifetime warranty` · `board certified` · `permanent result` ở bất kỳ ô nội dung nào.

Cổng này chặn lỗi cấu trúc, **không thay người duyệt**.
