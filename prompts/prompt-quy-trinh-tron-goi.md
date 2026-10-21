# PROMPT MẪU — QUY TRÌNH TRỌN GÓI: từ THỊ TRƯỜNG tới file HTML

> Dây chuyền **MODE 1 → 2 → 3**, có **3 chốt dừng** để người duyệt chen vào.
> Dùng khi mở một thị trường mới từ con số không.

```
┌──────────────────────────────────────────────────────────────┐
│ B1  MODE 1 · tầng + chân dung + hành trình S1–S7             │
│ B2  MODE 1 · chiến dịch + ngân sách + bản đồ landing         │
│ B3  MODE 1 · từ khoá (có market + geo_mode) → file .xlsx     │
│     ──────── CHỐT 1: duyệt bộ từ khoá ────────               │
│ B4  MODE 2 · mẫu quảng cáo cho 2–3 nhóm ưu tiên cao nhất     │
│     ──────── CHỐT 2: Pháp chế VN + thị trường đích ────────  │
│ B5  MODE 3 · dựng landing cho các nhóm đã duyệt              │
│ B6  MODE 3 · rà soát + scorecard + bảng kê ảnh               │
│     ──────── CHỐT 3: duyệt landing + cấp ảnh ────────        │
└──────────────────────────────────────────────────────────────┘
```

**Vì sao có 3 chốt:** gói này chịu **hai hệ pháp lý** và dữ liệu y khoa (số ngày ở lại) **không nằm trong tay marketing**. Chạy thẳng một hơi từ thị trường tới HTML sẽ ra một bộ đẹp nhưng không bật được.

---

## 1 · PROMPT TỔNG — chạy cả 6 bước, dừng ở 3 chốt

```
Chạy trọn gói cho:
  Thị trường: [vd Úc (AU)]
  Dịch vụ:    [vd Rhinoplasty]
  Ngân sách:  [vd 200 triệu VND/tháng]

Làm theo dây chuyền B1→B6, DỪNG LẠI ở 3 chốt và chờ tôi duyệt.

── B1 · NỀN ──
Chốt tầng thị trường (ngôn ngữ · múi giờ · kênh nhắn tin · mức rủi ro quảng cáo
+ tên cơ quan phải tra). Kiểm bản đồ thị trường × dịch vụ: dịch vụ này bán được
cho tầng này không? Giá trị ca có bù nổi vé + khách sạn + ngày nghỉ?
→ 4–7 chân dung (mỗi chân dung đủ 7 câu, có market + múi giờ + ràng buộc
  chuyến đi; tách khách lần đầu vs khách sửa lại)
→ hành trình S1–S7

── B2 · CHIẾN DỊCH ──
Tên theo mẫu KN-QT | tầng | market | chặng | cụm.
Ngân sách theo ý định mua × giá trị ca, tổng 100%, S3 ≥ 10% · S4 ≥ 15%.
Bản đồ landing: khung L1–L6 · chặng · chân dung · rào cản phải gỡ · CTA · micro.

── B3 · TỪ KHOÁ ──
80–130 dòng, mỗi dòng đủ market + geo_mode + WIN x/4.
Chỉ Exact/Phrase. volume và cpc để TRỐNG.
Ba ngách ưu tiên ≥ 40% ngân sách: S4 trip-planning · tiếng Việt từ nước ngoài
(nếu có tầng B) · từ khoá sửa lại.
Sinh JSON + chạy generator → đưa file .xlsx.

>>> CHỐT 1. In bảng tóm tắt (số chân dung / chiến dịch / từ khoá, tỷ trọng
    ngân sách, danh sách [PENDING]) rồi DỪNG. Hỏi tôi có duyệt không.

── B4 · MẪU QUẢNG CÁO ──
Chỉ làm cho 2–3 nhóm có điểm ưu tiên cao nhất, không làm cả bộ.
B1→B7 đầy đủ. Đếm ký tự từng dòng. Chấm 14 điểm, ≥ 12 mới xuất.

>>> CHỐT 2. Liệt kê rõ: cần Pháp chế VN duyệt gì · cần Pháp chế thị trường
    [X] duyệt gì · creative nào đang bị chặn vì luật market. Rồi DỪNG.

── B5 · LANDING ──
Dựng landing cho các nhóm đã duyệt. Khung chọn theo chặng × tầng.
Rà bộ bằng chứng theo market TRƯỚC khi viết.
Kiểm B08 (số ngày ở lại) + B09 (ai lo sau khi về) — chưa có số thì [PENDING].

── B6 · NGHIỆM THU ──
Scorecard từng trang + bảng kê ảnh cần cấp (có cột phạm vi đồng ý quốc tế)
+ danh sách [PENDING] gộp cả 3 bước, nhóm theo AI PHẢI CẤP.

>>> CHỐT 3. DỪNG. Chờ duyệt landing + cấp ảnh.
```

---

## 2 · PROMPT NGẮN

```
Chạy trọn gói cho [dịch vụ] ở [market], ngân sách [X]/tháng.
Dừng ở 3 chốt: sau bộ từ khoá, sau mẫu quảng cáo, sau landing.
```

---

## 3 · ĐƯỜNG TẮT — đã có bộ từ khoá, chỉ cần từ B4

```
Tôi đã có bộ từ khoá cho [market] / [dịch vụ] (đính kèm hoặc dán dưới đây).

Bỏ B1→B3. Bắt đầu từ B4.
Trước khi viết mẫu quảng cáo, kiểm nhanh 3 điểm của bộ từ khoá tôi gửi:
① mọi dòng có market + geo_mode chưa?
② dòng nào thuộc market rủi ro cao mà chưa khai cách xử lý creative?
③ nhóm nào đáng làm mẫu trước (điểm ưu tiên cao nhất)?
Thiếu gì thì nói, đừng tự điền.
```

---

## Bàn giao giữa các bước — thứ bắt buộc phải chảy xuống

Mỗi bước phải nhận đủ những trường này từ bước trước. Thiếu một trường là bước sau phải **đoán**, và đoán sai ở gói này là rủi ro pháp lý.

| Trường | B1→B2 | B2→B3 | B3→B4 | B4→B5 |
|---|---|---|---|---|
| `market` | ✅ | ✅ | ✅ | ✅ |
| Tầng (A/B/C/D) | ✅ | ✅ | ✅ | ✅ |
| `geo_mode` | — | ✅ | ✅ | ✅ |
| Chặng S1–S7 | ✅ | ✅ | ✅ | ✅ |
| Mã chân dung `CDx` | ✅ | ✅ | ✅ | ✅ |
| **Rào cản phải gỡ** | ✅ | ✅ | ✅ | ✅ |
| Khung landing L1–L6 | — | ✅ | — | ✅ |
| **Mức rủi ro quảng cáo + bằng chứng được phép dùng** | ✅ | ✅ | ✅ | ✅ |
| Ngôn ngữ + múi giờ + kênh nhắn tin | ✅ | ✅ | ✅ | ✅ |
| Danh sách `[PENDING]` tích luỹ | ✅ | ✅ | ✅ | ✅ |

> Dòng **"bằng chứng được phép dùng"** là dòng hay bị rơi nhất, và rơi nó là đắt nhất: team viết landing tầng C dựa vào before–after, tới bước duyệt mới phát hiện phải bỏ cả khối, và trang phải làm lại từ bước chọn bằng chứng.

---

## Nghiệm thu cuối tuyến

☐ File `.xlsx` build được, mọi dòng từ khoá có `market` + `geo_mode`
☐ Mẫu quảng cáo chấm **≥ 12/14**, đã đếm ký tự
☐ Landing chấm **≥ 80**, có B08 + B09
☐ **Một danh sách `[PENDING]` gộp**, nhóm theo người cấp:
  · Khoa Chuyên môn — số ngày ở lại · theo dõi hậu phẫu · lịch tái khám từ xa
  · Pháp chế VN — giấy xác nhận nội dung quảng cáo · T&C bảo hành · số CCHN bác sĩ
  · Pháp chế thị trường đích — rà theo AHPRA/ASA/FTC/GCC · GDPR notice nếu có EU/UK
  · Bộ phận quốc tế — phiên dịch · visa · đưa đón · Muslim-friendly gồm gì
  · Tài chính — phương thức thanh toán quốc tế + mức đặt cọc
  · Brand — chốt cặp font Cormorant + Inter (lệch với Roboto của production)
☐ Đã nói rõ **chưa có gì được bật** cho tới khi qua đủ 3 chốt
