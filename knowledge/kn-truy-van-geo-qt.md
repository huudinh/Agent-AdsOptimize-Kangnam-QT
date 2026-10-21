# BỘ TRUY VẤN GEO — QUỐC TẾ (Generative Engine Optimization)
Version: 1.0 — 2026-10-21 · nguồn: `HCI-Knowledge/GEOQUOCTE.xlsx`, bản cập nhật 14/09/2026

> **83 truy vấn tiếng Anh · 15 cụm · 53 truy vấn CORE 80/20.**
> Mục tiêu: khi khách nước ngoài hỏi AI bằng tiếng Anh về thẩm mỹ tại Việt Nam, **câu trả lời trích dẫn Kangnam** — trước hết ở 4 cụm quyết định: chọn cơ sở · an toàn/giấy phép · giá USD · logistics chuyến đi.
> Mục tiêu quý: **Share of Voice ≥ 30%** ở các cụm Tầng A.

---

## §0. ⚠️ HAI CHỮ "GEO" — ĐỪNG NHẦM

Gói này dùng chữ **GEO** cho **hai thứ khác nhau**. Nhầm hai thứ này là nhầm cả kênh.

| Viết là | Nghĩa | Thuộc | Đo bằng |
|---|---|---|---|
| **GEO** *(file này)* | **Generative Engine Optimization** — tối ưu để **AI trích dẫn** Kangnam khi khách hỏi ChatGPT · Gemini · AI Overview | **Organic / nội dung**, không trả tiền click | **Share of Voice** — AI có nhắc Kangnam không |
| **GEO-TARGET** *(`geo_mode`)* | **Geo-targeting** — nhắm vị trí người xem trong Google Ads: `Presence` vs `Presence+Interest` | **Paid ads** | CPL · chi phí/khách đến khám |

**Quy ước từ v1.1 trở đi:**
- Nói **"cổng GEO-TARGET"** khi nói về nhắm vị trí quảng cáo (trường `geo_mode`).
- Nói **"GEO"** hoặc **"truy vấn GEO"** khi nói về tối ưu câu trả lời AI (file này).

Hai kênh **dùng chung** chân dung · rào cản · rào pháp lý, nhưng **khác hẳn** ở: cách đo (SoV vs CPL), tốc độ (GEO tính theo quý, ads tính theo tuần), và ai sản xuất (người viết bản ngữ vs ad ops).

---

## §1. VÌ SAO KHÁCH QUỐC TẾ CẦN BỘ RIÊNG

Khách quốc tế hỏi AI **theo thứ tự này**, và nó khác hẳn khách Việt:

```
① Vietnam / cơ sở này có an toàn & được cấp phép không?
      ↓
② Giá USD bao nhiêu so với nước nhà / Thái / Hàn?
      ↓
③ Chuyến đi thu xếp ra sao, phải ở lại bao lâu?
      ↓
④ MỚI TỚI từng dịch vụ cụ thể
```

→ **Hệ quả quan trọng nhất:** **Tầng A là 4 cụm NGANG dịch vụ**, không phải trang dịch vụ.
Làm trang dịch vụ trước khi có trang thực thể + safety + pricing + logistics là **đi sai thứ tự** — AI không có gì để trích dẫn khi khách hỏi câu ① ② ③.

**Ba nỗi sợ chi phối** *(nguyên văn file nguồn)*:

| # | Nỗi sợ | Cụm xử lý | Số TV | % điểm |
|---|---|---|---|---|
| ① | **Sợ không an toàn / không phép** — *"'developing country' = rủi ro"* | Q12 + Q10 | 13 | **28,3%** |
| ② | **Sợ hỏng rồi về nước không ai lo** — nỗi sợ riêng của du lịch y tế | Q14 + Q15 | 9 | 10,9% |
| ③ | **Sợ chuyến đi rối & giá ẩn** | Q13 + Q11 | 12 | 18,6% |

---

## §2. ✅ BẢNG ÁNH XẠ — GEO 6 giai đoạn ↔ ADS 7 chặng

File nguồn dùng **6 giai đoạn**; bộ não gói này dùng **7 chặng S1–S7**. Hai hệ **gần nhau nhưng KHÔNG trùng khớp**.

⛔ **Không đánh số lại một hệ theo hệ kia.** File nguồn do team khác bảo trì; đổi số của nó là làm hỏng file của họ. Dùng bảng ánh xạ dưới đây.

| GEO *(file nguồn)* | ADS *(bộ não gói này)* | Khớp? |
|---|---|---|
| **G-S1 · AWARENESS** (Cold) | **S1 · NHẬN BIẾT** | ✅ khớp |
| **G-S2 · RESEARCH** (Warm) — *"kỹ thuật nào, SMAS hay deep plane"* | **S2 · SO SÁNH ĐIỂM ĐẾN** *(chọn nước)* | ⚠️ **lệch** — G-S2 là chọn **kỹ thuật**, S2 là chọn **nước** |
| **G-S3 · CONSIDER & FEAR** ★★★ — gồm cả **giá (Q11)** | **S3 · NỖI SỢ** + **S5 · THỰC HIỆN** *(giá)* | ⚠️ **lệch** — G-S3 gộp giá; ADS tách giá sang S5 |
| **G-S4 · PLAN THE TRIP** (Hot) | **S4 · LÊN KẾ HOẠCH CHUYẾN ĐI** | ✅ **khớp chính xác** |
| **G-S5 · AFTERCARE & FOLLOW-UP** | **S6 · HẬU PHẪU TỪ XA** | ✅ khớp (lệch số) |
| **G-S6 · RETURN & LTV** | **S7 · GẮN BÓ & GIỚI THIỆU** | ✅ khớp (lệch số) |
| — | **S5 · THỰC HIỆN** *(đặt lịch)* | ⚠️ GEO không có chặng "đặt lịch" riêng — hợp lý, vì AI không chốt đơn |

**Hai chỗ lệch phải nhớ khi dùng chéo hai bộ:**
① **"S2"** ở hai bộ là hai thứ khác nhau. Nội dung G-S2 (so sánh kỹ thuật) thực chất phục vụ **S3 ADS**; nội dung chọn nước của ADS S2 nằm ở **Q01 + Q10 + Q12** của GEO.
② **Giá**: GEO coi giá là phần của nỗi sợ (G-S3); ADS coi giá là chặng hành động (S5). Cả hai đều đúng cho kênh của mình — AI được hỏi giá rất sớm, còn người bấm quảng cáo giá thì đã sẵn sàng đặt lịch.

### Ánh xạ nỗi sợ → 4 rào cản của bộ não

| 3 nỗi sợ GEO | 4 rào cản ADS |
|---|---|
| ① không an toàn / không phép | **NGỜ** + **SỢ** |
| ② **hỏng rồi về nước không ai lo** | **XA** ★ |
| ③ chuyến đi rối & giá ẩn | **XA** + **NGẠI** |

> ✅ **Xác nhận độc lập:** file nguồn gọi nỗi sợ ② là *"nỗi sợ riêng của medical tourism"* — đúng là rào cản **XA** mà bộ não gói này dựng riêng. Hai bộ được làm độc lập nhưng tìm ra cùng một thứ. Đây là tín hiệu tốt: rào cản XA không phải suy diễn, nó có trong hành vi thật.

---

## §3. XẾP HẠNG 15 CỤM — 80/20

**Luật triển khai:** làm **hết Tầng A** (4 cụm, lũy kế **46,9% điểm**) rồi mới sang trang dịch vụ. ⛔ Không làm ngược.

| # | Mã | Cụm | Tầng | Cơ hội GEO | Số TV | CORE | Điểm | % | Lũy kế |
|---|---|---|---|---|---|---|---|---|---|
| 1 | **Q10** | Choosing a hospital & surgeon in Vietnam + thực thể Kan… | A | 3/3 | 7 | 6 | 456 | **15.5%** | 15.5% |
| 2 | **Q12** | Safety, risks, accreditation & licensing ⭐⭐ | A | 3/3 | 6 | 5 | 375 | **12.8%** | 28.3% |
| 3 | **Q11** | Cost & price transparency (USD) ⭐⭐ | A | 3/3 | 6 | 4 | 345 | **11.7%** | 40.0% |
| 4 | **Q13** | Medical tourism logistics — trip, stay, timeline ⭐ | A | 2/3 | 6 | 5 | 202 | **6.9%** | 46.9% |
| 5 | **Q02** | Liposuction & body contouring (abdomen, chin, arm, thig… | B | 2/3 | 7 | 4 | 210 | **7.1%** | 54.0% |
| 6 | **Q04** | Breast augmentation, lift & reduction | B | 2/3 | 6 | 4 | 212 | **7.2%** | 61.2% |
| 7 | **Q06** | Rhinoplasty in Vietnam (Ho Chi Minh City / Hanoi) | B | 2/3 | 5 | 4 | 178 | **6.1%** | 67.3% |
| 8 | **Q03** | Facelift (SMAS, deep plane, mini, midface, temporal, br… | B | 2/3 | 6 | 3 | 174 | **5.9%** | 73.2% |
| 9 | **Q05** | Eye surgery (blepharoplasty, eye rejuvenation) | B | 2/3 | 5 | 3 | 158 | **5.4%** | 78.6% |
| 10 | **Q15** | Revision surgery — fixing results from another country ⭐ | B | 2/3 | 4 | 3 | 142 | **4.8%** | 83.4% |
| 11 | **Q14** | Aftercare & remote follow-up after returning home | B | 2/3 | 5 | 4 | 178 | **6.1%** | 89.5% |
| 12 | **Q07** | Skin clinic & non-surgical (Thermage, PicoSure, HIFU, l… | C | 2/3 | 6 | 3 | 156 | **5.3%** | 94.8% |
| 13 | **Q09** | BBL — Brazilian butt lift, fat grafting, butt implants | C | 1/3 | 4 | 3 | 71 | **2.4%** | 97.2% |
| 14 | **Q08** | Dental clinic in Vietnam (aligners, veneers, implants,… | C | 1/3 | 5 | 2 | 69 | **2.3%** | 99.5% |
| 15 | **Q01** | Vietnam as a medical tourism destination (awareness) | D | 1/3 | 5 | 0 | 14 | **0.5%** |  |

**Khuyến nghị hành động từng cụm** *(nguyên văn file nguồn)*:

- **Q10** — Điều kiện để AI trả lời 'Kangnam' khi khách hỏi 'aesthetic hospital in Vietnam': trang thực thể EN + hồ sơ bác sĩ schema + tiêu chí chọn cơ sở.
- **Q12** — Nỗi sợ số 1 của khách quốc tế: 'Vietnam có an toàn không'. Trang safety nói thật + bằng chứng kiểm chứng được.
- **Q11** — Khách quốc tế so giá với nước nhà + Thái/Hàn. Bảng giá USD công khai min–max theo thủ thuật là đòn quyết định.
- **Q13** — Rào cản chuyển đổi đặc thù quốc tế: visa, bao lâu phải ở lại, ai đón, phiên dịch. Guide chi tiết = giảm rơi rụng.
- **Q02** — Nhu cầu lớn nhất từ mindmap: 8 nhánh lipo. Trang lipo EN theo vùng + hi-def/abs etching; nhấn an toàn thể tích hút.
- **Q04** — Giá trị đơn cao: nhấn túi ngực chính hãng có số lưu hành + bảo hành hãng; phân biệt augmentation/lift/reduction.
- **Q06** — Dịch vụ chữ ký chuẩn Hàn: mũi cấu trúc, sụn tự thân; nối với bộ Rhinoplasty quốc tế đã làm.
- **Q03** — Nhóm khách 45+ giá trị cao: phân biệt kỹ thuật SMAS/deep plane/mini; nhấn bác sĩ có phạm vi & DMKT.
- **Q05** — Nối với bộ Mắt (VN) — dịch tầng quốc tế: blepharoplasty trên/dưới, Asian double eyelid, eye rejuvenation.
- **Q15** — Lợi thế Kangnam (sửa hỏng) đưa ra quốc tế: khách bị hỏng ở nước khác tìm nơi sửa giá hợp lý. Rất ít đối thủ làm.
- **Q14** — Nỗi sợ riêng của khách quốc tế: 'about sau khi tôi về nước thì sao'. Chính sách theo dõi từ xa rõ ràng = tăng chốt.
- **Q07** — Lớp LTV cho expat sống tại VN: điều trị định kỳ. Nhấn máy chính hãng có số lưu hành, bác sĩ thực hiện.
- **Q09** — Rủi ro cao nhất ngành (thuyên tắc mỡ). Nội dung phải nói thật, chỉ định chặt; chỉ nếu kỹ thuật thuộc DMKT cơ sở.
- **Q08** — Dental tourism lớn nhưng cần chốt PHÁP NHÂN RHM (Kangnam dental hay Nha Khoa Paris) trước khi xuất bản.
- **Q01** — Cửa vào rộng, không bán: Vietnam vs các điểm đến, xu hướng, hệ thống y tế; dẫn mềm sang Q10/Q12.

**Bốn tầng ưu tiên:**

| Tầng | Cụm | Vai trò | Ngân sách EN |
|---|---|---|---|
| **A · CORE 80/20** | **Q10 · Q12 · Q11 · Q13** | 4 cụm **ngang dịch vụ** — điểm quyết định | **70%**, Sóng 1 (90 ngày) |
| **B · Đòn bẩy chuyển đổi** | Q02 Lipo · Q04 Ngực · Q06 Mũi · Q03 Facelift · Q05 Mắt · Q15 Revision · Q14 Aftercare | Trang dịch vụ + 2 cụm gỡ nỗi sợ XA | Sóng 2 |
| **C · Uy tín & giữ chân** | Q07 Skin clinic *(LTV expat)* · Q09 BBL · Q08 Dental | LTV + ngách rủi ro cao | Sóng 3 |
| **D · Cửa vào rộng** | Q01 Awareness | Không bán, dẫn mềm sang Q10/Q12 | Sóng 3 |

---

## §4. BỘ TRUY VẤN MASTER — 83 truy vấn

**Cách đọc cột:**
- **Góc hỏi (fan-out)** — kiểu câu hỏi: `Thực thể` · `Kiểm chứng` · `So sánh` · `Rủi ro` · `Chi phí` · `Thời gian` · `Điều kiện` · `Local` · `Định nghĩa` · `Quy trình` · `Kết quả` · `Xử lý` · `Bằng chứng` · `Hướng dẫn` · `Đánh giá` · `Chăm sóc`.
- **CORE** — thuộc nhóm 53 truy vấn 80/20, làm trước.
- **Khối trả lời cần có** — brief giao cho người viết. Đây là cột quan trọng nhất khi sản xuất nội dung.
- **Rào** — mã rào pháp lý R0–R9 (§7). Rà theo mã này **trước khi đăng**.

### Q10 · Choosing a hospital & surgeon in Vietnam + thực thể Kangnam ⭐⭐⭐

*Giai đoạn GEO: S3 · CONSIDER & FEAR (Warm→Hot) · 7 truy vấn · 6 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q10-01` | Best aesthetic hospital in Vietnam for plastic surgery — how do I choose? | Thực thể | Hot | P1 | ✅ | **R3** |
| `Q10-02` | Is Kangnam Aesthetic Hospital legit and licensed? | Kiểm chứng | Hot | P1 | ✅ | **R3** |
| `Q10-03` | Who are the surgeons at Kangnam and what are their credentials? | Thực thể | Hot | P1 | ✅ | **R4** |
| `Q10-04` | Aesthetic clinic vs aesthetic hospital in Vietnam — what's the difference? | So sánh | Hot | P1 | ✅ | **R3** |
| `Q10-05` | Plastic surgery in Ho Chi Minh City vs Hanoi — which is better for foreigners? | Local | Warm | P1 | ✅ | **R3** |
| `Q10-06` | Are there English-speaking plastic surgeons in Vietnam? | Điều kiện | Warm | P1 | ✅ | **R8** |
| `Q10-07` | Real patient reviews of plastic surgery at Kangnam Vietnam? | Bằng chứng | Warm | P2 |  | **R5** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (7 truy vấn)</summary>

**`Q10-01`** · Best aesthetic hospital in Vietnam for plastic surgery — how do I choose?

- *Từ khoá ưu tiên:* `aesthetic hospital vietnam`
- *Khối trả lời cần có:* Pillar thực thể EN: giấy phép, quy mô, giám đốc chuyên môn, tiêu chí chọn cơ sở; tránh 'best/#1'.
- *Trang đích:* `kangnamaesthetichospital.com/aesthetic-hospital-vietnam (pillar thực thể)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q10-02`** · Is Kangnam Aesthetic Hospital legit and licensed?

- *Từ khoá ưu tiên:* `kangnam aesthetic hospital review`
- *Khối trả lời cần có:* Số GPHĐ, cơ quan cấp, cách tự tra; pháp nhân đúng cơ sở phục vụ khách nước ngoài.
- *Trang đích:* `kangnamaesthetichospital.com/aesthetic-hospital-vietnam (pillar thực thể)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q10-03`** · Who are the surgeons at Kangnam and what are their credentials?

- *Từ khoá ưu tiên:* `kangnam surgeons`
- *Khối trả lời cần có:* Hồ sơ bác sĩ EN: CCHN, phạm vi, năm kinh nghiệm, ca; schema Person; đã xác minh.
- *Trang đích:* `kangnamaesthetichospital.com/our-surgeons (hồ sơ bác sĩ EN + schema)`
- *Rào:* R4 · Chỉ nêu bác sĩ đã xác minh CCHN + phạm vi; hồ sơ EN không thêm chức danh (KF-11 N.4)

**`Q10-04`** · Aesthetic clinic vs aesthetic hospital in Vietnam — what's the difference?

- *Từ khoá ưu tiên:* `aesthetic clinic vs hospital vietnam`
- *Khối trả lời cần có:* Phân tuyến pháp lý: phẫu thuật gây mê phải ở bệnh viện; clinic/beauty center chỉ thủ thuật nhỏ.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q10-05`** · Plastic surgery in Ho Chi Minh City vs Hanoi — which is better for foreigners?

- *Từ khoá ưu tiên:* `plastic surgery ho chi minh city`
- *Khối trả lời cần có:* Trang local EN từng cơ sở (NAP, sân bay, khách sạn gần); tiêu chí khách quan.
- *Trang đích:* `kangnamaesthetichospital.com/aesthetic-hospital-vietnam (pillar thực thể)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q10-06`** · Are there English-speaking plastic surgeons in Vietnam?

- *Từ khoá ưu tiên:* `english speaking plastic surgeon vietnam`
- *Khối trả lời cần có:* Bác sĩ/điều phối viên nói tiếng Anh + phiên dịch chuyên môn theo R8.
- *Trang đích:* `kangnamaesthetichospital.com/our-surgeons (hồ sơ bác sĩ EN + schema)`
- *Rào:* R8 · KCB cho người nước ngoài: cơ sở đủ điều kiện + bác sĩ + phiên dịch + hồ sơ (KF-11 N.8) — NÓNG

**`Q10-07`** · Real patient reviews of plastic surgery at Kangnam Vietnam?

- *Từ khoá ưu tiên:* `kangnam vietnam reviews`
- *Khối trả lời cần có:* Patient stories có văn bản đồng ý, quốc tịch, thủ thuật, mốc thời gian; link Google review.
- *Trang đích:* `kangnamaesthetichospital.com/patient-stories (case có văn bản đồng ý)`
- *Rào:* R5 · Ảnh/video KH phải có văn bản đồng ý minh thị, kể cả KH nước ngoài (KF-11 N.5)

</details>

### Q12 · Safety, risks, accreditation & licensing ⭐⭐

*Giai đoạn GEO: S3 · CONSIDER & FEAR (Warm→Hot) · 6 truy vấn · 5 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q12-01` | Is plastic surgery in Vietnam safe? | Rủi ro | Hot | P1 | ✅ | **R1** |
| `Q12-02` | What accreditation or license should a Vietnamese cosmetic hospital have? | Kiểm chứng | Hot | P1 | ✅ | **R3** |
| `Q12-03` | What happens if something goes wrong after surgery in Vietnam? | Rủi ro | Hot | P1 | ✅ | **R1** |
| `Q12-04` | Anesthesia safety standards in Vietnamese hospitals? | Rủi ro | Warm | P1 | ✅ | **R2** |
| `Q12-05` | Are implants and devices used in Vietnam FDA/CE approved? | Kiểm chứng | Warm | P1 | ✅ | **R7** |
| `Q12-06` | How do I verify a plastic surgeon's license in Vietnam? | Kiểm chứng | Warm | P2 |  | **R4** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q12-01`** · Is plastic surgery in Vietnam safe?

- *Từ khoá ưu tiên:* `is plastic surgery in vietnam safe`
- *Khối trả lời cần có:* BLUF: an toàn khi chọn bệnh viện được cấp phép; dạy tra cứu; nói thật rủi ro chung.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q12-02`** · What accreditation or license should a Vietnamese cosmetic hospital have?

- *Từ khoá ưu tiên:* `vietnam cosmetic hospital license`
- *Khối trả lời cần có:* Giải thích GPHĐ Bộ/Sở Y tế + DMKT + đăng ký bác sĩ; cách xác minh online.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q12-03`** · What happens if something goes wrong after surgery in Vietnam?

- *Từ khoá ưu tiên:* `plastic surgery complications abroad`
- *Khối trả lời cần có:* Quy trình xử lý biến chứng, theo dõi nội trú, kênh liên hệ 24/7, chính sách sửa; không cam kết.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q12-04`** · Anesthesia safety standards in Vietnamese hospitals?

- *Từ khoá ưu tiên:* `anesthesia safety vietnam`
- *Khối trả lời cần có:* Bác sĩ gây mê, phòng mổ, hồi sức; chỉ nêu thiết bị/nhân sự cơ sở thực có.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R2 · Kỹ thuật phải thuộc danh mục kỹ thuật (DMKT) được duyệt của cơ sở (KF-11 N.2)

**`Q12-05`** · Are implants and devices used in Vietnam FDA/CE approved?

- *Từ khoá ưu tiên:* `fda approved implants vietnam`
- *Khối trả lời cần có:* Túi ngực/thiết bị chính hãng có số lưu hành VN + chứng nhận hãng; khách được xem thẻ.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q12-06`** · How do I verify a plastic surgeon's license in Vietnam?

- *Từ khoá ưu tiên:* `verify plastic surgeon license vietnam`
- *Khối trả lời cần có:* Hướng dẫn tra CCHN + cơ sở đăng ký; dấu hiệu cảnh báo.
- *Trang đích:* `kangnamaesthetichospital.com/safety-accreditation`
- *Rào:* R4 · Chỉ nêu bác sĩ đã xác minh CCHN + phạm vi; hồ sơ EN không thêm chức danh (KF-11 N.4)

</details>

### Q11 · Cost & price transparency (USD) ⭐⭐

*Giai đoạn GEO: S3 · CONSIDER & FEAR (Warm→Hot) · 6 truy vấn · 4 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q11-01` | How much does plastic surgery cost in Vietnam compared to the US/Australia/UK? | So sánh | Hot | P1 | ✅ | **R6** |
| `Q11-02` | Kangnam price list — rhinoplasty, breast augmentation, liposuction, facelift in USD? | Chi phí | Hot | P1 | ✅ | **R9** |
| `Q11-03` | Vietnam vs Thailand vs Korea for cosmetic surgery — cost and quality? | So sánh | Hot | P1 | ✅ | **R6** |
| `Q11-04` | Does the price include hospital stay, anesthesia, follow-ups and medication? | Chi phí | Warm | P1 | ✅ | **R9** |
| `Q11-05` | Can I pay in USD or by international credit card? Any deposit? | Điều kiện | Warm | P2 |  | **R1** |
| `Q11-06` | Is cheap plastic surgery in Vietnam a red flag? | Rủi ro | Warm | P2 |  | **R6** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q11-01`** · How much does plastic surgery cost in Vietnam compared to the US/Australia/UK?

- *Từ khoá ưu tiên:* `plastic surgery cost vietnam`
- *Khối trả lời cần có:* Bảng so sánh chi phí theo thủ thuật (USD) với tiêu chí khách quan; không hạ thấp nước khác.
- *Trang đích:* `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)`
- *Rào:* R6 · So sánh quốc gia/cơ sở nêu tiêu chí khách quan, không hạ thấp (KF-11 N.6)

**`Q11-02`** · Kangnam price list — rhinoplasty, breast augmentation, liposuction, facelift in USD?

- *Từ khoá ưu tiên:* `kangnam price list`
- *Khối trả lời cần có:* Bảng giá USD min–max từng thủ thuật + ngày cập nhật + gói gồm gì.
- *Trang đích:* `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

**`Q11-03`** · Vietnam vs Thailand vs Korea for cosmetic surgery — cost and quality?

- *Từ khoá ưu tiên:* `vietnam vs thailand plastic surgery`
- *Khối trả lời cần có:* So sánh khách quan (giá, giấy phép, bác sĩ, thời gian lưu trú); tránh nói xấu.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R6 · So sánh quốc gia/cơ sở nêu tiêu chí khách quan, không hạ thấp (KF-11 N.6)

**`Q11-04`** · Does the price include hospital stay, anesthesia, follow-ups and medication?

- *Từ khoá ưu tiên:* `all inclusive plastic surgery package vietnam`
- *Khối trả lời cần có:* Làm rõ cấu phần gói; tránh phát sinh; minh bạch.
- *Trang đích:* `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

**`Q11-05`** · Can I pay in USD or by international credit card? Any deposit?

- *Từ khoá ưu tiên:* `pay usd plastic surgery vietnam`
- *Khối trả lời cần có:* Phương thức thanh toán thực tế, đặt cọc, hoàn cọc; kênh chính thức.
- *Trang đích:* `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q11-06`** · Is cheap plastic surgery in Vietnam a red flag?

- *Từ khoá ưu tiên:* `cheap plastic surgery vietnam`
- *Khối trả lời cần có:* Vì sao giá VN thấp hơn (chi phí vận hành) + cảnh báo giá rẻ bất thường/cơ sở không phép.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R6 · So sánh quốc gia/cơ sở nêu tiêu chí khách quan, không hạ thấp (KF-11 N.6)

</details>

### Q13 · Medical tourism logistics — trip, stay, timeline ⭐

*Giai đoạn GEO: S4 · PLAN THE TRIP (Hot) · 6 truy vấn · 5 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q13-01` | How long do I need to stay in Vietnam after plastic surgery? | Thời gian | Hot | P1 | ✅ | **R1** |
| `Q13-02` | Do I need a medical visa for cosmetic surgery in Vietnam? | Điều kiện | Warm | P1 | ✅ | **R8** |
| `Q13-03` | Does Kangnam offer airport pickup, hotel and interpreter for international patients? | Điều kiện | Warm | P1 | ✅ | **R8** |
| `Q13-04` | Can I fly right after liposuction / breast augmentation? | Rủi ro | Warm | P1 | ✅ | **R1** |
| `Q13-05` | How do I book a consultation from abroad — online consult before flying? | Quy trình | Warm | P1 | ✅ | **R1** |
| `Q13-06` | Best time of year to travel to Vietnam for surgery (weather, holidays)? | Hướng dẫn | Warm | P3 |  | **R0** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q13-01`** · How long do I need to stay in Vietnam after plastic surgery?

- *Từ khoá ưu tiên:* `how long stay vietnam after surgery`
- *Khối trả lời cần có:* Bảng số ngày lưu trú tối thiểu theo thủ thuật + mốc cắt chỉ/tái khám trước khi bay.
- *Trang đích:* `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q13-02`** · Do I need a medical visa for cosmetic surgery in Vietnam?

- *Từ khoá ưu tiên:* `medical visa vietnam cosmetic surgery`
- *Khối trả lời cần có:* Thông tin visa/e-visa hiện hành (dẫn nguồn chính thức); hỗ trợ thư mời nếu có.
- *Trang đích:* `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)`
- *Rào:* R8 · KCB cho người nước ngoài: cơ sở đủ điều kiện + bác sĩ + phiên dịch + hồ sơ (KF-11 N.8) — NÓNG

**`Q13-03`** · Does Kangnam offer airport pickup, hotel and interpreter for international patients?

- *Từ khoá ưu tiên:* `medical tourism package vietnam`
- *Khối trả lời cần có:* Dịch vụ điều phối quốc tế thực có: đón sân bay, lưu trú đối tác, phiên dịch chuyên môn (R8).
- *Trang đích:* `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)`
- *Rào:* R8 · KCB cho người nước ngoài: cơ sở đủ điều kiện + bác sĩ + phiên dịch + hồ sơ (KF-11 N.8) — NÓNG

**`Q13-04`** · Can I fly right after liposuction / breast augmentation?

- *Từ khoá ưu tiên:* `flying after surgery`
- *Khối trả lời cần có:* Khuyến cáo y khoa về bay sau mổ (huyết khối, sưng); mốc theo thủ thuật; bác sĩ quyết định.
- *Trang đích:* `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q13-05`** · How do I book a consultation from abroad — online consult before flying?

- *Từ khoá ưu tiên:* `online consultation plastic surgery vietnam`
- *Khối trả lời cần có:* Quy trình tư vấn online, gửi ảnh, báo giá sơ bộ, khám trực tiếp trước mổ.
- *Trang đích:* `kangnamaesthetichospital.com/faq (hub Q&A quốc tế)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q13-06`** · Best time of year to travel to Vietnam for surgery (weather, holidays)?

- *Từ khoá ưu tiên:* `best time travel vietnam surgery`
- *Khối trả lời cần có:* Gợi ý mùa, tránh Tết, lịch làm việc; nội dung hướng dẫn.
- *Trang đích:* `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)`
- *Rào:* R0 · Thấp — nội dung kiến thức, giữ giọng giáo dục, CTA mềm

</details>

### Q02 · Liposuction & body contouring (abdomen, chin, arm, thigh, hi-def, abs etching)

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 7 truy vấn · 4 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q02-01` | Liposuction in Vietnam — how much and is it safe? | Chi phí | Hot | P1 | ✅ | **R9** |
| `Q02-02` | Hi-def liposuction / abs etching in Vietnam — who is a good candidate? | Điều kiện | Warm | P1 | ✅ | **R1** |
| `Q02-03` | Double chin liposuction vs non-surgical fat reduction — which one? | So sánh | Warm | P1 | ✅ | **R1** |
| `Q02-04` | Abdominal liposuction vs tummy tuck — what do I actually need? | So sánh | Warm | P1 | ✅ | **R1** |
| `Q02-05` | How much fat can be safely removed in one session? | Rủi ro | Warm | P2 |  | **R1** |
| `Q02-06` | Arm and thigh liposuction recovery time before I can travel home? | Thời gian | Warm | P2 |  | **R1** |
| `Q02-07` | Six pack surgery — is it real and does it last? | Kết quả | Warm | P2 |  | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (7 truy vấn)</summary>

**`Q02-01`** · Liposuction in Vietnam — how much and is it safe?

- *Từ khoá ưu tiên:* `liposuction vietnam cost`
- *Khối trả lời cần có:* Dải giá USD theo vùng + tiêu chí an toàn (giới hạn thể tích, bệnh viện).
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

**`Q02-02`** · Hi-def liposuction / abs etching in Vietnam — who is a good candidate?

- *Từ khoá ưu tiên:* `hi def liposuction vietnam`
- *Khối trả lời cần có:* Chỉ định (BMI, cơ nền); không phải ai cũng phù hợp; kết quả tùy cơ địa.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q02-03`** · Double chin liposuction vs non-surgical fat reduction — which one?

- *Từ khoá ưu tiên:* `double chin liposuction vietnam`
- *Khối trả lời cần có:* So sánh phẫu thuật vs không phẫu thuật theo mức mỡ/da; định tuyến.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q02-04`** · Abdominal liposuction vs tummy tuck — what do I actually need?

- *Từ khoá ưu tiên:* `liposuction vs tummy tuck`
- *Khối trả lời cần có:* Phân biệt mỡ vs da thừa/cơ tách; bác sĩ đánh giá trực tiếp.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q02-05`** · How much fat can be safely removed in one session?

- *Từ khoá ưu tiên:* `safe liposuction volume`
- *Khối trả lời cần có:* Giới hạn an toàn theo thể trạng; vì sao hút quá nhiều nguy hiểm.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q02-06`** · Arm and thigh liposuction recovery time before I can travel home?

- *Từ khoá ưu tiên:* `liposuction recovery travel`
- *Khối trả lời cần có:* Mốc hồi phục + số ngày ở lại; mặc gen; bay khi nào.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q02-07`** · Six pack surgery — is it real and does it last?

- *Từ khoá ưu tiên:* `six pack surgery vietnam`
- *Khối trả lời cần có:* Giải thích abs etching thực tế; duy trì bằng lối sống; không 'vĩnh viễn'.
- *Trang đích:* `kangnamaesthetichospital.com/liposuction-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q04 · Breast augmentation, lift & reduction

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 6 truy vấn · 4 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q04-01` | Breast augmentation in Vietnam — cost, implants used and safety? | Chi phí | Hot | P1 | ✅ | **R7** |
| `Q04-02` | Which breast implant brands does Kangnam use — are they FDA approved? | Kiểm chứng | Hot | P1 | ✅ | **R7** |
| `Q04-03` | Breast lift vs breast augmentation — which do I need? | So sánh | Warm | P1 | ✅ | **R1** |
| `Q04-04` | Breast reduction in Vietnam for foreigners — recovery and scars? | Rủi ro | Warm | P1 | ✅ | **R1** |
| `Q04-05` | How long before I can fly home after breast surgery? | Thời gian | Warm | P2 |  | **R1** |
| `Q04-06` | Implant warranty — what if there's a rupture after I return home? | Điều kiện | Warm | P2 |  | **R7** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q04-01`** · Breast augmentation in Vietnam — cost, implants used and safety?

- *Từ khoá ưu tiên:* `breast augmentation vietnam`
- *Khối trả lời cần có:* Dải giá USD theo hãng túi + số lưu hành + bảo hành hãng; an toàn bệnh viện.
- *Trang đích:* `kangnamaesthetichospital.com/breast-augmentation-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q04-02`** · Which breast implant brands does Kangnam use — are they FDA approved?

- *Từ khoá ưu tiên:* `breast implant brands vietnam`
- *Khối trả lời cần có:* Danh sách hãng túi thực dùng + chứng nhận + thẻ bảo hành khách giữ.
- *Trang đích:* `kangnamaesthetichospital.com/breast-augmentation-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q04-03`** · Breast lift vs breast augmentation — which do I need?

- *Từ khoá ưu tiên:* `breast lift vs augmentation`
- *Khối trả lời cần có:* Phân biệt sa trễ vs thiếu thể tích; có thể kết hợp; bác sĩ đánh giá.
- *Trang đích:* `kangnamaesthetichospital.com/breast-augmentation-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q04-04`** · Breast reduction in Vietnam for foreigners — recovery and scars?

- *Từ khoá ưu tiên:* `breast reduction vietnam`
- *Khối trả lời cần có:* Đường mổ, sẹo, hồi phục; nói thật; kết quả tùy cơ địa.
- *Trang đích:* `kangnamaesthetichospital.com/breast-augmentation-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q04-05`** · How long before I can fly home after breast surgery?

- *Từ khoá ưu tiên:* `fly after breast augmentation`
- *Khối trả lời cần có:* Số ngày ở lại + mốc tái khám; khuyến cáo bay.
- *Trang đích:* `kangnamaesthetichospital.com/breast-augmentation-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q04-06`** · Implant warranty — what if there's a rupture after I return home?

- *Từ khoá ưu tiên:* `breast implant warranty abroad`
- *Khối trả lời cần có:* Bảo hành hãng toàn cầu + chính sách cơ sở; kênh xử lý từ xa; không hứa tuyệt đối.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

</details>

### Q06 · Rhinoplasty in Vietnam (Ho Chi Minh City / Hanoi)

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 5 truy vấn · 4 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q06-01` | Rhinoplasty in Ho Chi Minh City — cost and best surgeons? | Local | Hot | P1 | ✅ | **R4** |
| `Q06-02` | Korean-style structural rhinoplasty in Vietnam — what does it mean? | Định nghĩa | Warm | P1 | ✅ | **R6** |
| `Q06-03` | Ethnic / Western rhinoplasty in Vietnam — do surgeons have experience with non-Asian noses? | Điều kiện | Warm | P1 | ✅ | **R5** |
| `Q06-04` | Rhinoplasty recovery — how many days before I can fly? | Thời gian | Warm | P2 |  | **R1** |
| `Q06-05` | Revision rhinoplasty in Vietnam for a botched nose job done elsewhere? | Xử lý | Warm | P1 | ✅ | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (5 truy vấn)</summary>

**`Q06-01`** · Rhinoplasty in Ho Chi Minh City — cost and best surgeons?

- *Từ khoá ưu tiên:* `rhinoplasty ho chi minh city`
- *Khối trả lời cần có:* Trang rhinoplasty EN + local HCM: giá USD, bác sĩ mũi đã xác minh, case.
- *Trang đích:* `kangnamaesthetichospital.com/rhinoplasty-vietnam`
- *Rào:* R4 · Chỉ nêu bác sĩ đã xác minh CCHN + phạm vi; hồ sơ EN không thêm chức danh (KF-11 N.4)

**`Q06-02`** · Korean-style structural rhinoplasty in Vietnam — what does it mean?

- *Từ khoá ưu tiên:* `korean rhinoplasty vietnam`
- *Khối trả lời cần có:* Giải thích mũi cấu trúc, sụn tự thân vs nhân tạo; ai hợp; tránh nói quá 'chuẩn Hàn'.
- *Trang đích:* `kangnamaesthetichospital.com/rhinoplasty-vietnam`
- *Rào:* R6 · So sánh quốc gia/cơ sở nêu tiêu chí khách quan, không hạ thấp (KF-11 N.6)

**`Q06-03`** · Ethnic / Western rhinoplasty in Vietnam — do surgeons have experience with non-Asian noses?

- *Từ khoá ưu tiên:* `western rhinoplasty vietnam`
- *Khối trả lời cần có:* Kinh nghiệm với cấu trúc mũi phương Tây (giảm bướu, thu đầu mũi); case phù hợp có đồng ý.
- *Trang đích:* `kangnamaesthetichospital.com/rhinoplasty-vietnam`
- *Rào:* R5 · Ảnh/video KH phải có văn bản đồng ý minh thị, kể cả KH nước ngoài (KF-11 N.5)

**`Q06-04`** · Rhinoplasty recovery — how many days before I can fly?

- *Từ khoá ưu tiên:* `rhinoplasty recovery fly`
- *Khối trả lời cần có:* Mốc tháo nẹp/cắt chỉ, sưng; số ngày ở lại.
- *Trang đích:* `kangnamaesthetichospital.com/rhinoplasty-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q06-05`** · Revision rhinoplasty in Vietnam for a botched nose job done elsewhere?

- *Từ khoá ưu tiên:* `revision rhinoplasty vietnam`
- *Khối trả lời cần có:* Trang revision: tiếp nhận ca hỏng từ nước ngoài, đánh giá, giới hạn; liên kết Q15.
- *Trang đích:* `kangnamaesthetichospital.com/revision-surgery`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q03 · Facelift (SMAS, deep plane, mini, midface, temporal, brow lift)

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 6 truy vấn · 3 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q03-01` | Facelift in Vietnam — cost and which technique (SMAS vs deep plane)? | So sánh | Hot | P1 | ✅ | **R2** |
| `Q03-02` | Mini facelift vs full facelift — which is right for my age? | So sánh | Warm | P1 | ✅ | **R1** |
| `Q03-03` | Brow lift or temporal lift for hooded eyes — what's the difference? | So sánh | Warm | P2 |  | **R1** |
| `Q03-04` | How long does a facelift last and how long is recovery abroad? | Kết quả | Warm | P1 | ✅ | **R1** |
| `Q03-05` | Facelift scars — will they be visible? | Rủi ro | Warm | P2 |  | **R1** |
| `Q03-06` | Is a midface lift better than fillers for sagging cheeks? | So sánh | Warm | P2 |  | **R7** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q03-01`** · Facelift in Vietnam — cost and which technique (SMAS vs deep plane)?

- *Từ khoá ưu tiên:* `facelift vietnam cost`
- *Khối trả lời cần có:* Dải giá USD + so sánh kỹ thuật theo bằng chứng; kỹ thuật phải thuộc DMKT.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R2 · Kỹ thuật phải thuộc danh mục kỹ thuật (DMKT) được duyệt của cơ sở (KF-11 N.2)

**`Q03-02`** · Mini facelift vs full facelift — which is right for my age?

- *Từ khoá ưu tiên:* `mini facelift vs full facelift`
- *Khối trả lời cần có:* Chỉ định theo mức sa trễ/tuổi; kết quả tùy cơ địa.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q03-03`** · Brow lift or temporal lift for hooded eyes — what's the difference?

- *Từ khoá ưu tiên:* `brow lift vietnam`
- *Khối trả lời cần có:* Phân biệt brow/temporal lift vs blepharoplasty; định tuyến sang Q05.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q03-04`** · How long does a facelift last and how long is recovery abroad?

- *Từ khoá ưu tiên:* `facelift recovery abroad`
- *Khối trả lời cần có:* Độ bền trung bình + mốc hồi phục + số ngày ở lại; không 'permanent'.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q03-05`** · Facelift scars — will they be visible?

- *Từ khoá ưu tiên:* `facelift scars`
- *Khối trả lời cần có:* Vị trí đường mổ, quá trình mờ sẹo; nói thật.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q03-06`** · Is a midface lift better than fillers for sagging cheeks?

- *Từ khoá ưu tiên:* `midface lift vs filler`
- *Khối trả lời cần có:* So sánh phẫu thuật vs không phẫu thuật theo mức độ; định tuyến Q07.
- *Trang đích:* `kangnamaesthetichospital.com/facelift-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

</details>

### Q05 · Eye surgery (blepharoplasty, eye rejuvenation)

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 5 truy vấn · 3 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q05-01` | Blepharoplasty in Vietnam — cost, upper vs lower eyelid? | Chi phí | Hot | P1 | ✅ | **R9** |
| `Q05-02` | Asian double eyelid surgery in Vietnam — is Kangnam experienced with it? | Thực thể | Warm | P1 | ✅ | **R5** |
| `Q05-03` | Eye rejuvenation without surgery — what options are there in Vietnam? | So sánh | Warm | P2 |  | **R7** |
| `Q05-04` | Lower blepharoplasty for eye bags — will it leave scars? | Rủi ro | Warm | P1 | ✅ | **R1** |
| `Q05-05` | How many days after eyelid surgery can I fly home? | Thời gian | Warm | P2 |  | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (5 truy vấn)</summary>

**`Q05-01`** · Blepharoplasty in Vietnam — cost, upper vs lower eyelid?

- *Từ khoá ưu tiên:* `blepharoplasty vietnam`
- *Khối trả lời cần có:* Dải giá USD theo mí trên/dưới + chỉ định; an toàn.
- *Trang đích:* `kangnamaesthetichospital.com/blepharoplasty-vietnam`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

**`Q05-02`** · Asian double eyelid surgery in Vietnam — is Kangnam experienced with it?

- *Từ khoá ưu tiên:* `double eyelid surgery vietnam`
- *Khối trả lời cần có:* Kinh nghiệm cắt mí Á Đông; kỹ thuật; case có đồng ý.
- *Trang đích:* `kangnamaesthetichospital.com/blepharoplasty-vietnam`
- *Rào:* R5 · Ảnh/video KH phải có văn bản đồng ý minh thị, kể cả KH nước ngoài (KF-11 N.5)

**`Q05-03`** · Eye rejuvenation without surgery — what options are there in Vietnam?

- *Từ khoá ưu tiên:* `eye rejuvenation vietnam`
- *Khối trả lời cần có:* Botox/filler/laser vùng mắt vs phẫu thuật; rủi ro filler vùng mắt.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q05-04`** · Lower blepharoplasty for eye bags — will it leave scars?

- *Từ khoá ưu tiên:* `lower blepharoplasty scars`
- *Khối trả lời cần có:* Đường trong/ngoài; nói thật sẹo; tùy cơ địa.
- *Trang đích:* `kangnamaesthetichospital.com/blepharoplasty-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q05-05`** · How many days after eyelid surgery can I fly home?

- *Từ khoá ưu tiên:* `fly after blepharoplasty`
- *Khối trả lời cần có:* Mốc cắt chỉ + số ngày lưu trú.
- *Trang đích:* `kangnamaesthetichospital.com/blepharoplasty-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q15 · Revision surgery — fixing results from another country ⭐

*Giai đoạn GEO: S3 · CONSIDER & FEAR (Warm→Hot) · 4 truy vấn · 3 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q15-01` | I had a botched nose/breast/eyelid surgery abroad — can it be fixed in Vietnam? | Xử lý | Hot | P1 | ✅ | **R1** |
| `Q15-02` | How long should I wait before revision surgery? | Điều kiện | Warm | P1 | ✅ | **R1** |
| `Q15-03` | Does revision cost more than the first surgery? | Chi phí | Warm | P1 | ✅ | **R9** |
| `Q15-04` | Can you review my previous surgery records/photos before I fly? | Quy trình | Warm | P2 |  | **R5** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (4 truy vấn)</summary>

**`Q15-01`** · I had a botched nose/breast/eyelid surgery abroad — can it be fixed in Vietnam?

- *Từ khoá ưu tiên:* `revision surgery vietnam`
- *Khối trả lời cần có:* Trang revision EN: tiếp nhận, đánh giá online, giới hạn, thời điểm sửa; không hứa.
- *Trang đích:* `kangnamaesthetichospital.com/revision-surgery`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q15-02`** · How long should I wait before revision surgery?

- *Từ khoá ưu tiên:* `how long wait revision surgery`
- *Khối trả lời cần có:* Mốc mô ổn định; rủi ro sửa sớm; bác sĩ quyết định.
- *Trang đích:* `kangnamaesthetichospital.com/revision-surgery`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q15-03`** · Does revision cost more than the first surgery?

- *Từ khoá ưu tiên:* `revision surgery cost`
- *Khối trả lời cần có:* Vì sao phức tạp hơn; dải chi phí; cần khám mới báo giá.
- *Trang đích:* `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

**`Q15-04`** · Can you review my previous surgery records/photos before I fly?

- *Từ khoá ưu tiên:* `send medical records before revision`
- *Khối trả lời cần có:* Quy trình gửi hồ sơ/ảnh, bảo mật, tư vấn online.
- *Trang đích:* `kangnamaesthetichospital.com/faq (hub Q&A quốc tế)`
- *Rào:* R5 · Ảnh/video KH phải có văn bản đồng ý minh thị, kể cả KH nước ngoài (KF-11 N.5)

</details>

### Q14 · Aftercare & remote follow-up after returning home

*Giai đoạn GEO: S5 · AFTERCARE & FOLLOW-UP (Existing) · 5 truy vấn · 4 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q14-01` | How does follow-up work after I return home from surgery in Vietnam? | Điều kiện | Hot | P1 | ✅ | **R8** |
| `Q14-02` | Can my local doctor remove stitches / do check-ups after I leave Vietnam? | Điều kiện | Warm | P1 | ✅ | **R1** |
| `Q14-03` | What is Kangnam's warranty or policy if I need a correction later? | Điều kiện | Warm | P1 | ✅ | **R1** |
| `Q14-04` | What aftercare supplies and medications will I take home? | Chăm sóc | Warm | P2 |  | **R1** |
| `Q14-05` | Signs of complications I should watch for after flying home? | Rủi ro | Warm | P1 | ✅ | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (5 truy vấn)</summary>

**`Q14-01`** · How does follow-up work after I return home from surgery in Vietnam?

- *Từ khoá ưu tiên:* `aftercare after plastic surgery abroad`
- *Khối trả lời cần có:* Kênh theo dõi từ xa (video call, ảnh định kỳ), điều phối viên, phối hợp bác sĩ địa phương.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R8 · KCB cho người nước ngoài: cơ sở đủ điều kiện + bác sĩ + phiên dịch + hồ sơ (KF-11 N.8) — NÓNG

**`Q14-02`** · Can my local doctor remove stitches / do check-ups after I leave Vietnam?

- *Từ khoá ưu tiên:* `remove stitches home country`
- *Khối trả lời cần có:* Hướng dẫn phối hợp, hồ sơ xuất viện tiếng Anh, cái gì phải làm trước khi bay.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q14-03`** · What is Kangnam's warranty or policy if I need a correction later?

- *Từ khoá ưu tiên:* `plastic surgery warranty vietnam`
- *Khối trả lời cần có:* Chính sách theo văn bản + điều kiện; không 'lifetime guarantee' tuyệt đối.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q14-04`** · What aftercare supplies and medications will I take home?

- *Từ khoá ưu tiên:* `aftercare kit plastic surgery`
- *Khối trả lời cần có:* Danh sách vật tư/thuốc kèm đơn tiếng Anh; lưu ý hải quan.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q14-05`** · Signs of complications I should watch for after flying home?

- *Từ khoá ưu tiên:* `complication signs after surgery`
- *Khối trả lời cần có:* Dấu hiệu nguy hiểm phải đi khám ngay tại địa phương + báo cơ sở.
- *Trang đích:* `kangnamaesthetichospital.com/aftercare-remote-followup`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q07 · Skin clinic & non-surgical (Thermage, PicoSure, HIFU, laser, filler, botox, scars, tattoo removal)

*Giai đoạn GEO: S6 · RETURN & LTV · 6 truy vấn · 3 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q07-01` | Thermage / HIFU in Vietnam — is the machine genuine and how much? | Kiểm chứng | Warm | P1 | ✅ | **R7** |
| `Q07-02` | PicoSure Pro laser in Vietnam for pigmentation and tattoo removal? | Định nghĩa | Warm | P1 | ✅ | **R7** |
| `Q07-03` | Lip filler and botox in Vietnam — safe brands and prices for expats? | Chi phí | Warm | P1 | ✅ | **R7** |
| `Q07-04` | Best skin clinic in Ho Chi Minh City for expats? | Local | Warm | P2 |  | **R3** |
| `Q07-05` | Scar treatment options in Vietnam after surgery or acne? | Định nghĩa | Warm | P2 |  | **R1** |
| `Q07-06` | Non-surgical facial rejuvenation packages for a 1-week trip? | Hướng dẫn | Warm | P2 |  | **R9** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (6 truy vấn)</summary>

**`Q07-01`** · Thermage / HIFU in Vietnam — is the machine genuine and how much?

- *Từ khoá ưu tiên:* `thermage vietnam`
- *Khối trả lời cần có:* Máy chính hãng + số lưu hành + đầu tip mới; giá USD; kết quả tùy cơ địa.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q07-02`** · PicoSure Pro laser in Vietnam for pigmentation and tattoo removal?

- *Từ khoá ưu tiên:* `picosure vietnam`
- *Khối trả lời cần có:* Chỉ định, số buổi, giá; máy chính hãng.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q07-03`** · Lip filler and botox in Vietnam — safe brands and prices for expats?

- *Từ khoá ưu tiên:* `lip filler vietnam`
- *Khối trả lời cần có:* Hãng filler/botox có số lưu hành; bác sĩ tiêm; giá USD; rủi ro tắc mạch.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R7 · Túi ngực/thiết bị/filler chính hãng, có số lưu hành; không thổi phồng (KF-11 N.7)

**`Q07-04`** · Best skin clinic in Ho Chi Minh City for expats?

- *Từ khoá ưu tiên:* `skin clinic ho chi minh city expat`
- *Khối trả lời cần có:* Trang skin clinic EN + local; tiêu chí khách quan; tránh 'best'.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q07-05`** · Scar treatment options in Vietnam after surgery or acne?

- *Từ khoá ưu tiên:* `scar treatment vietnam`
- *Khối trả lời cần có:* Laser/tiêm/microneedling theo loại sẹo; kỳ vọng thực tế.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q07-06`** · Non-surgical facial rejuvenation packages for a 1-week trip?

- *Từ khoá ưu tiên:* `non surgical rejuvenation vietnam`
- *Khối trả lời cần có:* Gói không phẫu thuật phù hợp lịch ngắn; không phát sinh downtime.
- *Trang đích:* `kangnamaesthetichospital.com/skin-clinic-vietnam`
- *Rào:* R9 · QC dịch vụ KCB (kể cả tiếng Anh): soát GXNNDQC tại Sở Y tế (KF-11 N.9)

</details>

### Q09 · BBL — Brazilian butt lift, fat grafting, butt implants

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 4 truy vấn · 3 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q09-01` | Brazilian butt lift in Vietnam — is it safe and how much? | Rủi ro | Hot | P1 | ✅ | **R2** |
| `Q09-02` | Butt fat grafting vs butt implants — pros, cons and risks? | So sánh | Warm | P1 | ✅ | **R1** |
| `Q09-03` | How much fat survives after a BBL and how long does it last? | Kết quả | Warm | P2 |  | **R1** |
| `Q09-04` | BBL recovery — sitting, flying and how long to stay in Vietnam? | Thời gian | Warm | P1 | ✅ | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (4 truy vấn)</summary>

**`Q09-01`** · Brazilian butt lift in Vietnam — is it safe and how much?

- *Từ khoá ưu tiên:* `brazilian butt lift vietnam`
- *Khối trả lời cần có:* Nói thật rủi ro thuyên tắc mỡ; kỹ thuật tiêm nông; chỉ nếu trong DMKT; giá USD.
- *Trang đích:* `kangnamaesthetichospital.com/brazilian-butt-lift-vietnam`
- *Rào:* R2 · Kỹ thuật phải thuộc danh mục kỹ thuật (DMKT) được duyệt của cơ sở (KF-11 N.2)

**`Q09-02`** · Butt fat grafting vs butt implants — pros, cons and risks?

- *Từ khoá ưu tiên:* `butt implants vs fat grafting`
- *Khối trả lời cần có:* So sánh theo bằng chứng; rủi ro từng loại; ai hợp.
- *Trang đích:* `kangnamaesthetichospital.com/brazilian-butt-lift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q09-03`** · How much fat survives after a BBL and how long does it last?

- *Từ khoá ưu tiên:* `bbl fat survival`
- *Khối trả lời cần có:* Tỉ lệ mỡ sống trung bình; không 'permanent'; có thể cần dặm.
- *Trang đích:* `kangnamaesthetichospital.com/brazilian-butt-lift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q09-04`** · BBL recovery — sitting, flying and how long to stay in Vietnam?

- *Từ khoá ưu tiên:* `bbl recovery fly`
- *Khối trả lời cần có:* Kiêng ngồi, số ngày lưu trú dài hơn; khuyến cáo bay.
- *Trang đích:* `kangnamaesthetichospital.com/brazilian-butt-lift-vietnam`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q08 · Dental clinic in Vietnam (aligners, veneers, implants, crowns)

*Giai đoạn GEO: S2 · RESEARCH (Warm) · 5 truy vấn · 2 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q08-01` | Dental implants in Vietnam for foreigners — cost, brands and warranty? | Chi phí | Hot | P1 | ✅ | **R3** |
| `Q08-02` | Veneers in Ho Chi Minh City vs Hanoi — price and quality? | Local | Warm | P1 | ✅ | **R3** |
| `Q08-03` | Clear aligners in Vietnam — can I continue treatment from abroad? | Điều kiện | Warm | P2 |  | **R1** |
| `Q08-04` | Porcelain crowns in Vietnam — will they damage my natural teeth? | Rủi ro | Warm | P2 |  | **R1** |
| `Q08-05` | Can I get implants and veneers done in one trip to Vietnam? | Thời gian | Warm | P2 |  | **R1** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (5 truy vấn)</summary>

**`Q08-01`** · Dental implants in Vietnam for foreigners — cost, brands and warranty?

- *Từ khoá ưu tiên:* `dental implants vietnam`
- *Khối trả lời cần có:* Dải giá USD theo hãng trụ + số lưu hành + bảo hành; đúng pháp nhân RHM.
- *Trang đích:* `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q08-02`** · Veneers in Ho Chi Minh City vs Hanoi — price and quality?

- *Từ khoá ưu tiên:* `veneers ho chi minh city`
- *Khối trả lời cần có:* Giá USD, loại sứ chính hãng; đạo đức mài răng; local theo cơ sở RHM.
- *Trang đích:* `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)`
- *Rào:* R3 · Gắn ĐÚNG pháp nhân bệnh viện có giấy phép; site EN phải trỏ đúng cơ sở (KF-11 N.3)

**`Q08-03`** · Clear aligners in Vietnam — can I continue treatment from abroad?

- *Từ khoá ưu tiên:* `aligners vietnam remote`
- *Khối trả lời cần có:* Theo dõi từ xa, số lần về VN, lộ trình.
- *Trang đích:* `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q08-04`** · Porcelain crowns in Vietnam — will they damage my natural teeth?

- *Từ khoá ưu tiên:* `porcelain crowns vietnam`
- *Khối trả lời cần có:* Nói thật mài răng; chỉ định đúng; ưu tiên bảo tồn răng thật.
- *Trang đích:* `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

**`Q08-05`** · Can I get implants and veneers done in one trip to Vietnam?

- *Từ khoá ưu tiên:* `dental work one trip vietnam`
- *Khối trả lời cần có:* Lộ trình 1 hay 2 chuyến (tích hợp xương); kế hoạch thực tế.
- *Trang đích:* `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)`
- *Rào:* R1 · Không cam kết kết quả/permanent/100% safe; "results vary" (KF-11 N.1)

</details>

### Q01 · Vietnam as a medical tourism destination (awareness)

*Giai đoạn GEO: S1 · AWARENESS (Cold) · 5 truy vấn · 0 CORE*

| ID | Truy vấn khách gõ vào AI (EN) | Góc hỏi | Nhiệt | Ưu tiên | CORE | Rào |
|---|---|---|---|---|---|---|
| `Q01-01` | Is Vietnam a good destination for medical tourism / cosmetic surgery? | Định nghĩa | Cold | P2 |  | **R0** |
| `Q01-02` | Why are so many people getting plastic surgery in Vietnam now? | Đánh giá | Cold | P2 |  | **R0** |
| `Q01-03` | What cosmetic procedures is Vietnam known for? | Định nghĩa | Cold | P2 |  | **R0** |
| `Q01-04` | Do Vietnamese plastic surgeons train in Korea or the US? | Kiểm chứng | Cold | P3 |  | **R4** |
| `Q01-05` | Medical tourism in Vietnam — what are the main risks to be aware of? | Rủi ro | Cold | P3 |  | **R0** |

<details><summary>Brief nội dung + trang đích + rào pháp lý (5 truy vấn)</summary>

**`Q01-01`** · Is Vietnam a good destination for medical tourism / cosmetic surgery?

- *Từ khoá ưu tiên:* `vietnam medical tourism`
- *Khối trả lời cần có:* Tổng quan khách quan: giá, bác sĩ đào tạo, bệnh viện tư; dẫn tiêu chí chọn.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R0 · Thấp — nội dung kiến thức, giữ giọng giáo dục, CTA mềm

**`Q01-02`** · Why are so many people getting plastic surgery in Vietnam now?

- *Từ khoá ưu tiên:* `plastic surgery vietnam trend`
- *Khối trả lời cần có:* Xu hướng, số liệu có nguồn; giọng giáo dục.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R0 · Thấp — nội dung kiến thức, giữ giọng giáo dục, CTA mềm

**`Q01-03`** · What cosmetic procedures is Vietnam known for?

- *Từ khoá ưu tiên:* `popular cosmetic procedures vietnam`
- *Khối trả lời cần có:* Nhóm thủ thuật phổ biến; dẫn mềm sang trang dịch vụ.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R0 · Thấp — nội dung kiến thức, giữ giọng giáo dục, CTA mềm

**`Q01-04`** · Do Vietnamese plastic surgeons train in Korea or the US?

- *Từ khoá ưu tiên:* `vietnamese plastic surgeon training`
- *Khối trả lời cần có:* Đào tạo/chứng chỉ thực tế của bác sĩ; chỉ nêu đã xác minh.
- *Trang đích:* `kangnamaesthetichospital.com/our-surgeons (hồ sơ bác sĩ EN + schema)`
- *Rào:* R4 · Chỉ nêu bác sĩ đã xác minh CCHN + phạm vi; hồ sơ EN không thêm chức danh (KF-11 N.4)

**`Q01-05`** · Medical tourism in Vietnam — what are the main risks to be aware of?

- *Từ khoá ưu tiên:* `medical tourism vietnam risks`
- *Khối trả lời cần có:* Rủi ro chung (cơ sở không phép, theo dõi từ xa); dẫn sang Q12.
- *Trang đích:* `kangnamaesthetichospital.com/blog (kiến thức EN)`
- *Rào:* R0 · Thấp — nội dung kiến thức, giữ giọng giáo dục, CTA mềm

</details>


---

## §5. BẢN ĐỒ NỘI DUNG — trang đích theo cụm

Nội dung tiếng Anh **do người viết bản ngữ / biên tập chuẩn y khoa**. ⛔ **Không dịch máy** (xem §7 và `kn-rao-phap-ly-qt.md` §5).

| # | Mã | Tầng | Giai đoạn GEO | Vai trò trong phễu | Dạng nội dung cần sản xuất | Trang đích chính |
|---|---|---|---|---|---|---|
| 1 | **Q10** | A | S3 · CONSIDER & FEAR (War… | NEO THỰC THỂ + điểm quyết định | Pillar 'Aesthetic hospital in Vietnam' + trang surgeons (schema Person) + local HCM/HN EN + tiêu chí chọn | `kangnamaesthetichospital.com/aesthetic-hospital-vietnam (pillar thực thể)` |
| 2 | **Q12** | A | S3 · CONSIDER & FEAR (War… | Gỡ nỗi sợ số 1 | Trang Safety & Accreditation: giấy phép, gây mê, thiết bị, quy trình biến chứng — kiểm chứng được | `kangnamaesthetichospital.com/safety-accreditation` |
| 3 | **Q11** | A | S3 · CONSIDER & FEAR (War… | Tín hiệu mua | Bảng giá USD min–max công khai + bài so sánh chi phí quốc gia (khách quan) | `kangnamaesthetichospital.com/pricing (bảng giá USD công khai)` |
| 4 | **Q13** | A | S4 · PLAN THE TRIP (Hot) | Đòn bẩy chuyển đổi đặc thù | Medical tourism guide: số ngày ở lại theo thủ thuật, visa, đón/lưu trú, online consult | `kangnamaesthetichospital.com/medical-tourism-guide (lịch trình, lưu trú, phiên dịch)` |
| 5 | **Q02** | B | S2 · RESEARCH (Warm) | Nhu cầu lớn nhất | Trang lipo EN theo vùng + hi-def/abs etching + recovery-to-fly | `kangnamaesthetichospital.com/liposuction-vietnam` |
| 6 | **Q04** | B | S2 · RESEARCH (Warm) | Giá trị đơn cao | Trang breast EN + hãng túi + bảo hành toàn cầu | `kangnamaesthetichospital.com/breast-augmentation-vietnam` |
| 7 | **Q06** | B | S2 · RESEARCH (Warm) | Dịch vụ chữ ký | Trang rhinoplasty EN (nối bộ Rhinoplasty quốc tế) + Western nose cases | `kangnamaesthetichospital.com/rhinoplasty-vietnam` |
| 8 | **Q03** | B | S2 · RESEARCH (Warm) | Khách 45+ giá trị cao | Trang facelift EN so sánh kỹ thuật + recovery abroad | `kangnamaesthetichospital.com/facelift-vietnam` |
| 9 | **Q05** | B | S2 · RESEARCH (Warm) | Nối bộ Mắt VN | Trang blepharoplasty EN + Asian double eyelid | `kangnamaesthetichospital.com/blepharoplasty-vietnam` |
| 10 | **Q15** | B | S3 · CONSIDER & FEAR (War… | Lợi thế khác biệt | Trang Revision surgery EN + quy trình gửi hồ sơ online | `kangnamaesthetichospital.com/revision-surgery` |
| 11 | **Q14** | B | S5 · AFTERCARE & FOLLOW-U… | Gỡ nỗi sợ 'về nước ai lo' | Trang Aftercare & remote follow-up + hồ sơ xuất viện EN + chính sách văn bản | `kangnamaesthetichospital.com/aftercare-remote-followup` |
| 12 | **Q07** | C | S6 · RETURN & LTV | LTV cho expat | Trang skin clinic EN: máy chính hãng, bảng giá, gói định kỳ | `kangnamaesthetichospital.com/skin-clinic-vietnam` |
| 13 | **Q09** | C | S2 · RESEARCH (Warm) | Rủi ro cao — làm cẩn trọng | Trang BBL EN nói thật rủi ro + chỉ định chặt | `kangnamaesthetichospital.com/brazilian-butt-lift-vietnam` |
| 14 | **Q08** | C | S2 · RESEARCH (Warm) | Dental tourism | Trang dental EN (implant, veneer, aligner) | `kangnamaesthetichospital.com/dental-clinic-vietnam (pháp nhân RHM — cần chốt)` |
| 15 | **Q01** | D | S1 · AWARENESS (Cold) | Cửa vào rộng | Blog EN 'Vietnam as a destination' + trends | `kangnamaesthetichospital.com/blog (kiến thức EN)` |

**Bốn trang Tầng A phải có trước mọi trang dịch vụ:**

| Trang | Phục vụ | Nội dung lõi |
|---|---|---|
| `/aesthetic-hospital-vietnam` *(pillar thực thể)* | Q10 | Giấy phép · quy mô · hồ sơ bác sĩ (schema `Person`) · tiêu chí chọn cơ sở · local HCM/HN |
| `/safety-accreditation` | Q12 | Giấy phép · chuẩn gây mê · thiết bị có **số lưu hành** · quy trình xử lý biến chứng |
| `/pricing` | Q11 | **Bảng giá USD min–max công khai** + bài so sánh chi phí quốc gia (khách quan) |
| `/medical-tourism-guide` | Q13 | **Số ngày ở lại theo thủ thuật** · visa · đón/lưu trú · online consult trước khi bay |

> ⚠️ Trang `/medical-tourism-guide` cần **số ngày ở lại** — trường dữ liệu vẫn đang `[CHỜ CẬP NHẬT]` ở `kn-thi-truong-quoc-te.md` §8. **Không viết trang này bằng số tự suy.** Đây là cùng một nút thắt đã chặn khối B08 của landing.

---

## §6. ĐO LƯỜNG — 20 PROMPT SHARE OF VOICE

**Cách chạy** *(nguyên văn file nguồn)*:
- **Chế độ ẩn danh**, ngôn ngữ giao diện **tiếng Anh**, **VPN/IP từ thị trường mục tiêu** (US/AU/UK) nếu có.
- Ghi **1** nếu Kangnam được nhắc/trích dẫn, **0** nếu không — trên **3 nền tảng**: ChatGPT · Gemini · AI Overview.
- Ghi **tên đối thủ AI nhắc** (Thái Lan / Hàn Quốc / cơ sở VN khác) để biết **ai đang chiếm câu trả lời**.
- Baseline: **09/2026**. Chạy **đều mỗi tháng**.
- **Mục tiêu quý: SoV ≥ 30% ở cụm Tầng A.**

**Prompt 1–6 phủ đủ 4 cụm Tầng A** — nếu chỉ chạy được 6 prompt thì chạy 6 cái đó.

| # | Prompt kiểm tra (dán nguyên văn) | Cụm đo | Mã | Tầng |
|---|---|---|---|---|
| 1 | **Best aesthetic hospital in Vietnam for foreigners?** | Thực thể | Q10 | A |
| 2 | **Is Kangnam Aesthetic Hospital legit?** | Thực thể | Q10 | A |
| 3 | **Is plastic surgery in Vietnam safe?** | An toàn | Q12 | A |
| 4 | **How much does plastic surgery cost in Vietnam?** | Chi phí | Q11 | A |
| 5 | **Vietnam vs Thailand for cosmetic surgery?** | Chi phí | Q11 | A |
| 6 | **How long should I stay in Vietnam after surgery?** | Logistics | Q13 | A |
| 7 | **Liposuction in Vietnam — cost and safety?** | Lipo | Q02 | B |
| 8 | **Breast augmentation in Vietnam — which implants?** | Ngực | Q04 | B |
| 9 | **Rhinoplasty in Ho Chi Minh City — recommended surgeons?** | Mũi | Q06 | B |
| 10 | **Facelift in Vietnam — SMAS or deep plane?** | Facelift | Q03 | B |
| 11 | **Blepharoplasty in Vietnam cost?** | Mắt | Q05 | B |
| 12 | **Can a botched surgery from Turkey/Korea be fixed in Vietnam?** | Revision | Q15 | B |
| 13 | **How does follow-up work after I fly home from Vietnam?** | Aftercare | Q14 | B |
| 14 | **Thermage in Vietnam — genuine machine?** | Skin | Q07 | C |
| 15 | **Brazilian butt lift in Vietnam — safe?** | BBL | Q09 | C |
| 16 | **Dental implants in Vietnam for foreigners?** | Dental | Q08 | C |
| 17 | **Is Vietnam good for medical tourism?** | Awareness | Q01 | D |
| 18 | **English-speaking plastic surgeons in Vietnam?** | Thực thể | Q10 | A |
| 19 | **Are implants used in Vietnam FDA approved?** | An toàn | Q12 | A |
| 20 | **Medical visa Vietnam cosmetic surgery?** | Logistics | Q13 | A |

**Công thức:** `SoV = (số prompt có nhắc Kangnam) / (tổng số prompt)` — tính riêng từng nền tảng.

> ⚠️ Cột *"đối thủ được AI nhắc"* là cột có giá trị nhất và hay bị bỏ trống. SoV = 0 mà không biết **ai** đang được trích dẫn thay mình thì không sửa được gì.

---

## §7. RÀO PHÁP LÝ R0–R9 — soát trước khi đăng

**Nguyên tắc nền** *(nguyên văn)*: **KHÔNG CHẮC → DỪNG → HỎI PHÁP CHẾ → RỒI MỚI ĐĂNG.**
Nội dung tiếng Anh **vẫn chịu luật quảng cáo & KCB Việt Nam** — đây là nhầm lẫn phổ biến nhất.

| Mã | Rào | ⛔ KHÔNG được làm | ✅ Thay bằng | Cụm áp dụng | Số TV | CORE | Người duyệt |
|---|---|---|---|---|---|---|---|
| **R0** | Thấp — nội dung kiến thức | Chèn quảng cáo dịch vụ vào bài kiến thức nền | Giữ giọng giáo dục; CTA mềm | Q01 | 5 | 0 | Content lead |
| **R1** | Cam kết kết quả | '100% safe','permanent results','lifetime guarantee','no scars' | 'Results vary'; nêu độ bền trung bình; mô tả có/không phù hợp | Toàn bộ | 36 | 21 | BS + Pháp chế |
| **R2** | Danh mục kỹ thuật (DMKT) | Quảng cáo kỹ thuật (deep plane, BBL, abs etching) ngoài danh mục được duyệt | Chỉ nêu kỹ thuật thuộc DMKT đã phê duyệt | Q02 Q03 Q09 Q12 | 3 | 3 | Pháp chế |
| **R3** | Đúng pháp nhân | Site EN gộp nhiều cơ sở/pháp nhân; dùng tên 'Kangnam' cho dịch vụ cơ sở không có phạm vi | Site EN trỏ đúng bệnh viện có giấy phép + phạm vi; NAP từng cơ sở | Q10 Q07 Q08 — ĐIỂM NÓNG | 8 | 7 | Pháp chế |
| **R4** | Bác sĩ | Thêm chức danh EN không có thật ('board-certified' khi không đúng); bác sĩ chưa xác minh | Chỉ dùng bác sĩ đã xác minh (KF-02); dịch đúng học vị/CCHN | Q10 Q06 Q01 | 4 | 2 | Pháp chế |
| **R5** | Hình ảnh khách hàng | Dùng ảnh KH nước ngoài khi mới đồng ý miệng; chỉnh ảnh | Văn bản đồng ý minh thị (song ngữ); ảnh cùng điều kiện chụp | Q10 Q05 Q06 Q15 | 4 | 2 | BS + Pháp chế |
| **R6** | So sánh quốc gia / đối thủ | Hạ thấp Thái Lan/Hàn Quốc/cơ sở khác; tự nhận 'best in Vietnam' | Bảng tiêu chí khách quan (giá, giấy phép, thời gian); tránh so sánh trực tiếp | Q11 Q06 Q12 | 4 | 3 | Pháp chế |
| **R7** | Túi ngực / thiết bị / filler | Nêu hãng không dùng thật; máy/filler không rõ số lưu hành | Chỉ hãng thực dùng có số lưu hành + chứng nhận; khách được xem thẻ | Q04 Q07 Q05 Q12 | 9 | 6 | BS + Pháp chế |
| **R8** | KCB cho người nước ngoài — NÓNG | Tiếp nhận khách nước ngoài khi cơ sở/bác sĩ chưa đủ điều kiện; không có phiên dịch chuyên môn | Đủ điều kiện pháp lý + phiên dịch + hồ sơ song ngữ + kênh theo dõi từ xa | Q10 Q13 Q14 — toàn bộ site EN | 4 | 4 | Pháp chế + Điều phối QT |
| **R9** | Giấy xác nhận nội dung QC | QC dịch vụ/giá bằng tiếng Anh chưa xin GXNNDQC (tưởng nội dung EN không cần) | Xác minh GXNNDQC cho cả bản EN trước khi chạy | Q11 Q02 Q05 Q07 Q15 | 6 | 5 | Pháp chế |

**Quy trình bắt buộc** *(nguyên văn)*:
```
Content EN soạn → tự kiểm checklist → BS thẩm định chuyên môn
→ Pháp chế duyệt nội dung & hình ảnh (KỂ CẢ BẢN EN)
→ GXNNDQC nếu là QC dịch vụ → mới đăng
```
Riêng **nha khoa (Q08)**: ✅ **đã gỡ chặn 2026-10-21** — Kangnam có chuyên khoa Nha khoa thẩm mỹ dưới chính pháp nhân BVTM Kangnam Sài Gòn (**287/BYT-GPHĐ**). Khi viết: **trỏ về cơ sở TP.HCM** và ghi đúng số 287; muốn làm cho **Hà Nội (194)** thì phải xác nhận riêng.

### 🔴 Bốn rào mà `kn-rao-phap-ly-qt.md` v1.0 CHƯA CÓ — đã bổ sung

Bộ truy vấn GEO mang vào bốn rào pháp lý **cứng** mà file pháp lý của gói này còn thiếu. Chúng áp cho **cả nội dung GEO và quảng cáo trả tiền**:

| Mã | Rào | Vì sao nó là rào cứng, không phải khuyến nghị |
|---|---|---|
| **R2** | **Danh mục kỹ thuật (DMKT)** | ⛔ Không được quảng cáo kỹ thuật **ngoài danh mục đã phê duyệt** của cơ sở — cụ thể **deep plane · BBL · abs etching**. Đây là vượt phạm vi hoạt động, không phải chuyện câu chữ. Chạm 3 truy vấn, cả 3 đều CORE |
| **R3** | **Đúng pháp nhân** | ⛔ Site EN **không được gộp nhiều cơ sở/pháp nhân**, không dùng tên "Kangnam" cho dịch vụ mà cơ sở đó không có phạm vi. **Điểm nóng** — chạm 8 truy vấn, 7 CORE |
| **R7** | **Túi ngực · thiết bị · filler** | ⛔ Chỉ nêu **hãng thực dùng, có số lưu hành** + chứng nhận; khách được xem thẻ. Chạm **9 truy vấn**, 6 CORE — nhiều thứ hai sau R1 |
| **R8** | **KCB cho người nước ngoài — NÓNG NHẤT** | ⛔ Không tiếp nhận khách nước ngoài khi **cơ sở/bác sĩ chưa đủ điều kiện**, hoặc **không có phiên dịch chuyên môn**. Cần: đủ điều kiện pháp lý + phiên dịch + **hồ sơ song ngữ** + kênh theo dõi từ xa. Áp cho **toàn bộ site EN** |

> **R8 là rào quan trọng nhất mà gói này thiếu.** Nó không nói về câu chữ quảng cáo — nó nói rằng **việc tiếp nhận khách quốc tế** có điều kiện pháp lý riêng. Một chiến dịch chạy tốt, landing hoàn hảo, nhưng cơ sở chưa đủ điều kiện R8 thì **lead đổ về là rủi ro, không phải thành tích**.

---

## §8. AGENT DÙNG BỘ NÀY THẾ NÀO

**MODE 5 · GEO-ANSWER** — xem §15b bộ não. Luồng:

```
① Chọn cụm (Q01–Q15) theo tầng ưu tiên — Tầng A trước, không đảo
② Lấy các truy vấn CORE của cụm đó ở §4
③ Đọc cột "Khối trả lời cần có" → đó là brief, không phải gợi ý
④ Rà mã rào R# của từng truy vấn ở §7 TRƯỚC khi viết
⑤ Viết nội dung EN cho trang đích ở §5
⑥ Kiểm 4 rào mới R2/R3/R7/R8 + rào R1 (cam kết kết quả)
⑦ Ghi lại prompt đo SoV tương ứng ở §6 để tháng sau đo
```

**Ba luật khi viết nội dung GEO** *(khác hẳn viết quảng cáo)*:

**① Viết để ĐƯỢC TRÍCH DẪN, không để thuyết phục.** AI trích dẫn nội dung **trả lời trực tiếp, có thể kiểm chứng, có cấu trúc**. Một đoạn nói *"chúng tôi là lựa chọn hàng đầu"* không bao giờ được trích; một đoạn nói *"Licence No. 194/BYT-GPHĐ, issued by the Ministry of Health on [date]"* thì có.

**② Khung PAS, không phải AIDA.** Người đọc nội dung GEO **chưa chủ động tìm Kangnam** — họ hỏi AI một câu hỏi chung. Luật này đã có trong `kn-khung-landing-qt.md`: *"PAS chỉ dùng cho SEO · GEO · social nguội"*.

**③ Trả lời câu hỏi đúng như khách gõ.** Cột *"truy vấn khách gõ vào AI"* là **nguyên văn**, không phải từ khoá để nhồi. Đặt nó làm tiêu đề `H2`/`H3` và trả lời ngay bên dưới trong 2–3 câu đầu.

⛔ **Không trộn GEO với quảng cáo trả tiền:** nội dung GEO **không gắn `market`/`geo_mode`** (AI không có geo-targeting), **không chấm cổng WIN 3/4** (không có CPC), và **không đo bằng CPL** (đo bằng SoV). Cổng WIN và cổng GEO-TARGET **không áp** cho MODE 5.

---

## §9. NHỮNG GÌ BỘ NÀY XÁC NHẬN VÀ NHỮNG GÌ NÓ SỬA

**Xác nhận** *(hai bộ làm độc lập, trùng kết luận)*:
- **Rào cản XA** — file nguồn gọi là *"nỗi sợ riêng của medical tourism"*, cụm Q14+Q15.
- **Chặng kế hoạch chuyến đi** — **G-S4 khớp chính xác S4** của bộ não, và cả hai đều xếp nó là chặng đòn bẩy đặc thù.
- **Số ngày ở lại là nút thắt** — Q13-01 là truy vấn **Hot/P1/CORE** đứng đầu cụm logistics, và trang `/medical-tourism-guide` không viết được nếu thiếu số.
- **Giá phải hiện, bằng USD** — Q11 là cụm hạng 3, *"bảng giá USD công khai min–max là đòn quyết định"*.
- **Không hạ thấp Thái/Hàn, không tự nhận "best"** — R6, trùng luật §4 của `kn-rao-phap-ly-qt.md`.

**Sửa / bổ sung cho gói:**
- ➕ **4 rào pháp lý R2 · R3 · R7 · R8** (§7) — đã thêm vào `kn-rao-phap-ly-qt.md`.
- ➕ **Thứ tự quyết định của khách quốc tế** (§1): an toàn → giá → chuyến đi → **mới tới dịch vụ**. Hệ quả: Tầng A là 4 cụm **ngang dịch vụ**.
- ➕ **Hai dịch vụ cần chốt trước khi làm nội dung**: **Q08 Dental** (pháp nhân RHM) và **Q09 BBL** (chỉ nếu kỹ thuật thuộc DMKT, và phải nói thật rủi ro thuyên tắc mỡ).
- ⚠️ **Làm rõ chữ "GEO"** (§0) — trước v1.1, "cổng GEO-TARGET" trong gói này nghĩa là geo-targeting; nay đổi thành **"cổng GEO-TARGET"** để không nhầm với Generative Engine Optimization.

---

## §10. NGUỒN & CẬP NHẬT

| | |
|---|---|
| **File nguồn** | `HCI-Knowledge/GEOQUOCTE.xlsx` — 8 sheet |
| **Bản cập nhật** | 14/09/2026 · baseline đo SoV: 09/2026 |
| **Trích xuất vào file này** | 2026-10-21 |
| **Ai bảo trì file nguồn** | Team GEO/Content — **không sửa file nguồn từ gói này** |

**Khi file nguồn đổi:** trích xuất lại, **giữ nguyên hệ số G-S1…G-S6 của họ**, cập nhật bảng ánh xạ §2 nếu họ thêm/bớt giai đoạn. ⛔ Không đánh số lại theo S1–S7 của bộ não.

Hai bộ anh em dùng cùng phương pháp GEO: [`Agent-KN-GEO-Plant`](../../Agent-KN-GEO-Plant/) · [`Agent-PR-GEO-Plant`](../../Agent-PR-GEO-Plant/).
