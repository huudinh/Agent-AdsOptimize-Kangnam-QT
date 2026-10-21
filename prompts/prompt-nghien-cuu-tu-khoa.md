# PROMPT MẪU — MODE 1 · KEYWORD-RESEARCH (thị trường quốc tế)

> Dùng khi: có **thị trường + dịch vụ**, chưa có từ khoá.
> Đầu ra: bộ từ khoá theo tầng → chân dung → hành trình S1–S7, kèm file `.xlsx` 5 sheet.

## Cần chuẩn bị một lần

| # | Thứ | Vì sao |
|---|---|---|
| 1 | **Thị trường đích** — nước khách đang ở, hoặc "expat tại VN" | Trường **duy nhất không bao giờ được giả định** |
| 2 | Dịch vụ | Để kiểm bản đồ thị trường × dịch vụ |
| 3 | Ngân sách/tháng | Để chia tỷ trọng |
| 4 | Bật công cụ chạy code (ChatGPT → *Code Interpreter*) | Để ra thẳng file Excel |
| 5 | Upload `tools/build_keyword_workbook.py` + `markets/README.md` + `markets/rhinoplasty-tier-c-au.json` vào Knowledge | Generator + schema + ví dụ đối chiếu |

---

## 1 · PROMPT CHÍNH — ra thẳng file Excel

```
MODE 1 — KEYWORD-RESEARCH.

Thị trường: [vd Úc (AU)]
Dịch vụ:    [vd Rhinoplasty]
Ngân sách:  [vd 200 triệu VND/tháng]

Làm theo K1→K8 trong bộ não, theo đúng thứ tự, không đảo:

K1 · Chốt tầng thị trường. Khai luôn: ngôn ngữ · múi giờ · kênh nhắn tin chính
     · mức rủi ro quảng cáo + tên cơ quan phải tra.
K2 · Kiểm bản đồ thị trường × dịch vụ: dịch vụ này bán được cho tầng này không?
     Giá trị ca có bù nổi vé + khách sạn + ngày nghỉ việc? Không → nói ngay,
     đề xuất đổi dịch vụ hoặc ghép combo.
K3 · 4–7 chân dung. Mỗi chân dung trả lời đủ 7 câu, trong đó bắt buộc có
     market + ngôn ngữ + múi giờ, và ràng buộc chuyến đi.
     Tách hẳn: khách lần đầu vs khách đi sửa lại.
K4 · Hành trình S1–S7 (7 chặng, có S4 kế hoạch chuyến đi).
K5 · Chiến dịch + ngân sách. Tên theo mẫu KN-QT | tầng | market | chặng | cụm.
     Chia theo ý định mua × giá trị ca, KHÔNG theo lượng tìm kiếm.
     Tổng 100%. Tối thiểu: S3 ≥ 10% · S4 ≥ 15% · tầng B ≥ 15%.
K6 · Landing: khai đủ khung L1–L6 · chặng · chân dung · rào cản phải gỡ
     · CTA · micro-conversion.
K7 · 80–130 dòng từ khoá. Mỗi dòng khai đủ market + geo_mode + điểm WIN x/4.
     Chỉ Exact/Phrase. Để TRỐNG volume và cpc.
     Ưu tiên 3 ngách: (1) từ khoá kế hoạch chuyến đi S4 (2) tiếng Việt từ nước
     ngoài nếu có tầng B (3) từ khoá sửa lại. Ba ngách này ≥ 40% ngân sách.
K8 · Phủ định chung + phủ định chéo để ĐIỀU HƯỚNG.

Sau đó xuất file Excel ngay trong phiên này:
  1. sinh JSON đúng schema markets/README.md
  2. chạy tools/build_keyword_workbook.py bằng công cụ chạy code
  3. đưa file .xlsx để tôi tải về
  4. báo cáo: số chân dung / chiến dịch / từ khoá · tỷ trọng ngân sách
     · danh sách [PENDING] còn thiếu

Script báo lỗi thì sửa JSON rồi chạy lại, tối đa 3 lần.
KHÔNG sửa script. KHÔNG bỏ dữ liệu để lách cổng.
```

---

## 2 · PROMPT NGẮN — khi đã quen

```
MODE 1 cho [dịch vụ] ở thị trường [market], ngân sách [X]/tháng.
Xuất file Excel luôn.
```

---

## 3 · PROMPT BỔ SUNG — thêm một thị trường vào bộ đã có

```
Tôi đã có bộ từ khoá cho [market cũ]. Giờ mở thêm [market mới].

Trước khi viết gì, trả lời 3 câu:
① [market mới] có cùng nhóm luật quảng cáo với [market cũ] không?
   Không → creative KHÔNG nhân bản được, phải viết lại. Nói rõ cái gì không
   dùng lại được và vì sao (luật, không phải hiệu quả).
② Có cùng tầng không? Khác tầng thì khác động cơ, khác độ trễ, khác rào cản.
③ Ngôn ngữ và múi giờ khác thế nào? Kênh nhắn tin chính có đổi không?

Rồi mới: giữ lại được gì · phải viết mới gì · ngân sách chia lại thế nào.
Xuất file JSON + Excel RIÊNG cho market mới, không trộn vào file cũ.
```

---

## 4 · PROMPT RÀ SOÁT — trước khi giao team chạy ads

```
Rà bộ từ khoá này trước khi tôi giao cho team. Kiểm đúng 9 điểm:

1. Mọi dòng có đủ market + geo_mode chưa?
2. Dòng nào market = VN-EXPAT mà geo_mode không phải Presence?
3. Dòng nào có địa danh Việt Nam mà chưa tách rõ "khách sắp bay" vs
   "expat đang ở đó"?
4. Dòng nào thuộc market rủi ro cao (AU/UK/EU/US/GCC) mà ghi_chu chưa khai
   cách xử lý before-after / testimonial?
5. Có dòng nào Broad không?
6. Cột volume và cpc có bị điền sẵn không? (phải để trống)
7. Tổng tỷ trọng ngân sách có đúng 100%? S4 có ≥ 15%?
8. Thông điệp nào còn từ cấm tiếng Anh, hoặc còn "lifetime warranty" /
   "board certified" / so giá với quốc gia có tên?
9. Dịch vụ giá thấp nào đang chấm > 2/4 cho tầng A/B/C?

Xuất bảng: dòng số · lỗi · sửa thành gì. Không in lại cả bộ.
```

---

## 5 · DỰ PHÒNG — phiên không chạy được code

```
Phiên này không chạy được code. Vẫn làm K1→K8 đầy đủ, nhưng:
- xuất ra BẢNG markdown thay cho file Excel
- kèm luôn khối JSON hoàn chỉnh để tôi tự chạy generator trên máy

Nói rõ ngay câu đầu rằng phiên này không xuất được .xlsx.
```

Chạy trên máy:
```bash
pip install openpyxl
python tools/build_keyword_workbook.py markets/<file>.json -o out/
```

---

## Checklist nghiệm thu

☐ Dòng khai `Market · Tier · Stage · Language · Ad-risk` ở đầu output
☐ K2 đã kiểm bản đồ thị trường × dịch vụ, **không bỏ qua**
☐ 4–7 chân dung, mỗi chân dung đủ 7 câu, **có market + múi giờ + ràng buộc chuyến đi**
☐ Tách **khách lần đầu** và **khách sửa lại**
☐ Hành trình đủ **7 chặng**, có S4
☐ Ngân sách tổng 100% · **S4 ≥ 15%** · S3 ≥ 10%
☐ Mọi dòng từ khoá có **`market` + `geo_mode`**
☐ `volume` và `cpc` **để trống**
☐ Không có `Broad`
☐ Ba ngách ưu tiên chiếm **≥ 40%** ngân sách
☐ Phủ định có **miễn trừ nhóm so sánh** (`vs` · `cheaper than`)
☐ File `.xlsx` build được, hoặc có lý do rõ ràng vì sao không
☐ Danh sách `[PENDING]` ở cuối, nêu rõ **ai cấp**
