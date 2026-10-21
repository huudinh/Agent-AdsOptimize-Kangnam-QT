# PROMPT MẪU — MODE 3 · LDP-BUILD (landing page quốc tế)

> Đầu ra: copy-deck 14 khối, hoặc HTML một file theo **Design System Kangnam International v1.0**.
> Mẫu dựng sẵn để đối chiếu: [`template/lp-skeleton-en.html`](../template/lp-skeleton-en.html) — khung **L3 Trip-plan**, đầy đủ token · form quốc tế · ô ảnh tạm · khối `[PENDING]`.

## Trang tham chiếu dùng để làm gì — và KHÔNG dùng để làm gì

Trang production: `https://kangnamaesthetichospital.com/top-plastic-surgery-in-vietnam/`
(bản lưu: `template/lp-reference-top-plastic-surgery.html` + `template/lp-reference-style.css`)

| ✅ Lấy | ❌ Không lấy |
|---|---|
| Token màu (`--primary-color #005F88` · `--second-color #00BAC3`) | **Câu FAQ** — có tên *"Dr. Granzow"*, một bác sĩ của cơ sở khác |
| Nhịp section, cách trình bày credential bar | **Con số social proof** — bản live đang hiện *"Trusted by 0+ clients"* |
| **Spec form quốc tế** (country code · nationality · kênh nhắn tin) | **Câu định vị superlative** — *"The Leading / Top-Rated Aesthetic Hospital in Vietnam"* |
| **Khối 5 bước cho khách ở xa** (*Out of Town Patients*) | Claim *"Lifetime warranty"* và *"the results are permanent"* |

Chi tiết 3 lỗi đang có trên bản live: `knowledge/kn-ho-so-thuong-hieu-qt.md` §4.4.

---

## 1 · PROMPT ĐẦY ĐỦ — dựng 1 landing page

```
MODE 3 — LDP-BUILD.

Cụm từ khoá: [dán từ khoá]
Market:      [vd AU]
Tầng:        [vd C]
Dịch vụ:     [vd Rhinoplasty]
Cơ sở:       [Hanoi hoặc Ho Chi Minh City]
Chặng:       [vd S4 — không biết thì tự suy và nói rõ]

Làm theo 12 bước của §14 bộ não:

① Chốt khung L1–L6 theo CHẶNG × TẦNG, nói rõ vì sao chọn khung đó.
② Lấy trust / bác sĩ / quy trình từ kn-ho-so-thuong-hieu-qt.md.
   Giá lấy tại /price-list/ ở thời điểm chạy.
③ Rà bộ bằng chứng theo market TRƯỚC KHI VIẾT. Market AU/UK/EU/US/GCC thì
   loại testimonial kết quả và before-after ra khỏi kế hoạch ngay từ đầu,
   không loại sau. Nói rõ trụ bằng chứng còn lại là gì.
④ Kiểm khối B08 (your trip) và B09 (after you fly home):
   - có số ngày ở lại chưa? chưa thì [PENDING: minimum stay — Medical Dept]
   - có nói ai liên hệ, kênh gì, trong bao lâu chưa?
   ⛔ KHÔNG tự suy số ngày ở lại.
⑤ Xuất bản đồ 14 khối theo đúng thứ tự của khung đã chọn.
⑥ Copy từng khối. Màn hero có 3 phương án headline:
   góc Bác sĩ / góc Quy trình-An toàn / góc Logistics chuyến đi.
⑦ Bộ CTA + microcopy + form theo spec §7 của kn-khung-landing-qt.md
   + thank-you page CÓ QUY ĐỔI MÚI GIỜ của khách.
⑧ Spec UI & mobile.
⑨ BẢNG KÊ ẢNH CẦN CẤP — có cột "đồng ý có phạm vi quốc tế hay không".
⑩ Kết quả cổng pháp lý THEO MARKET + danh sách [PENDING].
⑪ Scorecard từng tiêu chí + tổng (≥ 80 mới giao).
⑫ 2 giả thuyết A/B + KPI + sau bao lâu đánh giá lại.

Hỏi tôi "copy-deck trước, hay dựng thẳng HTML?" trước khi dựng.
```

---

## 2 · PROMPT NGẮN

```
MODE 3 — landing cho "[từ khoá]", market [X], tầng [Y], dịch vụ [Z].
Chọn khung, nói rõ vì sao, rồi dựng. HTML một file.
```

---

## 3 · PROMPT DỰNG THẲNG HTML

```
Dựng HTML một file cho landing này.

Tuân Design System Kangnam International v1.0:
- Token: --teal #005F88 · --teal-900 #00394F · --navy #003C77
  · --gold #B08D4F · --cta #E15A01 · --champagne #FAF7F2
- Tỷ lệ 78% trắng/champagne · 15% teal · 5% gold · 2% cam
- Cormorant Garamond 600 (≥28px) cho display + Inter cho body/UI
- body 17px · input 16px · section padding 96/48px
- responsive max-width 1140px, KHÔNG phải thẻ 480px như gói nội địa
- Bảy rào tương phản: không --teal-400 làm chữ trên trắng (2,38)
  · --gold chữ nhỏ trên trắng chỉ 3,10 → ≥24px hoặc ≥19px/700, nhỏ hơn
    dùng --gold-dk (4,77) · --cta là màu NỀN NÚT, trắng trên nó 3,71
    → nhãn ≥19px/700, nút nhỏ hơn dùng --cta-press (4,76)
  · --ink-3 (3,52) không dùng cho chữ thân → dùng --ink-2 (6,93)

Form bắt buộc có: country code + phone · email · country/market · service
· 1 kênh nhắn tin · preferred contact time + time zone
· consent nêu rõ chuyển dữ liệu sang Việt Nam + link privacy policy.

tel: phải đủ mã quốc gia (+84). WhatsApp deep-link kiểm thật.

Ảnh chưa có → ô ảnh tạm viền đứt, ghi rõ tỉ lệ + nội dung cần + ai duyệt.
⛔ Không ảnh stock, không ảnh AI, không <img> trỏ URL không tồn tại.

Cuối file kèm comment: §LEGAL (chưa được bật) + BẢNG KÊ ẢNH CẦN CẤP + self-score.

Đối chiếu template/lp-skeleton-en.html cho đúng khuôn.
```

---

## 4 · PROMPT CHO KHUNG L3 — trang quan trọng nhất

```
Dựng landing khung L3 Trip-plan cho [dịch vụ], market [X].

Đây là trang trả lời rào cản XA, và là trang có đòn bẩy cao nhất của cả gói.
Hai khối không được làm sơ sài:

B08 · YOUR TRIP, STEP BY STEP
  - 5 bước: pre-consultation → reservation → consultation → operation → discharge
  - Bước 2 PHẢI có số ngày ở lại (hoặc [PENDING]) và nói rõ mốc nào:
    ngày cắt chỉ · ngày tái khám cuối · ngày được phép bay
  - Bước 4 KHÔNG được chỉ viết "Safety is our priority" — đó là tính từ đúng
    chỗ cần bằng chứng nhất. Thay bằng: ai mổ · phòng mổ gì · theo dõi bao lâu
    · ai trực

B09 · AFTER YOU FLY HOME
  - ai là người liên hệ (tên bộ phận, không phải inbox chung)
  - kênh gì · ngôn ngữ gì · TRONG BAO LÂU
  - lịch tái khám từ xa
  - nếu phải chỉnh sửa: ai trả chi phí, ai trả vé
    ⛔ Không dùng chữ "lifetime" khi chưa có T&C bằng văn bản

Phép thử trước khi giao: "Đọc trang này xong, khách có đủ thông tin để mở
app hàng không và chọn ngày bay chưa?" Chưa → trang chưa xong.
```

---

## 5 · PROMPT RÀ SOÁT — trước khi đẩy traffic

```
Rà landing này theo scorecard kn-khung-landing-qt.md §9. Kiểm 10 điểm:

1. Khung có đúng chặng × tầng không? (L4 cho từ khoá S2 là lỗi phổ biến nhất)
2. Message-match: 3 yếu tố của ad có xuất hiện ở hero không?
3. Rào cản XA: có SỐ NGÀY Ở LẠI và có nói AI LO SAU KHI VỀ chưa? (15 điểm)
4. Bộ bằng chứng có đúng luật của market này không?
   (AU/UK/EU/GCC: không testimonial kết quả, không before-after)
5. Bảng giá có đủ 3 dòng bắt buộc? Có nêu phụ phí quốc tế 10%?
6. Form có preferred contact time + time zone? Có consent nêu chuyển dữ liệu
   sang VN?
7. tel: có đủ +84? WhatsApp link có hoạt động?
8. Bảy rào tương phản có bị phá chỗ nào?
9. Có ảnh stock / ảnh AI / <img> trỏ URL không tồn tại không?
10. Có sao chép gì từ trang tham chiếu không được phép?
    (câu FAQ có tên Dr. Granzow · số 0+ · superlative · lifetime/permanent)

Chấm điểm từng tiêu chí + tổng. Liệt kê lỗi theo mức ưu tiên.
Viết lại phần yếu nhất.
```

---

## 6 · PROMPT CHUYỂN BIẾN THỂ sang market khác

```
Tôi có landing này cho market [X]. Chuyển sang market [Y].

Trước khi viết, trả lời 3 câu:
① [Y] có cùng nhóm luật quảng cáo với [X] không? Không → nêu rõ khối nào
   phải gỡ và vì sao (luật, không phải hiệu quả).
② Khác tầng không? Khác tầng thì khác rào cản chính → có thể phải đổi khung.
③ Ngôn ngữ, múi giờ, kênh nhắn tin đổi thế nào?

Rồi mới: giữ gì · gỡ gì · viết mới gì. Chấm lại scorecard cho market mới.
```

---

## Checklist giao hàng

☐ Dòng khai `Market · Tier · Stage · Language · Ad-risk` ở đầu
☐ Khung L1–L6 + **lý do chọn theo chặng × tầng**
☐ Bản đồ 14 khối đúng thứ tự của khung
☐ Hero có **3 phương án headline**
☐ **B08 có số ngày ở lại** (hoặc `[PENDING]` đúng vị trí)
☐ **B09 nói rõ ai liên hệ · kênh gì · trong bao lâu**
☐ Bộ bằng chứng **đúng luật market** — tầng C không dựa vào before–after/testimonial
☐ Bảng giá đủ **3 dòng bắt buộc** + cột gồm gì / không gồm gì
☐ Form đủ trường, có **`preferred contact time + time zone`**
☐ Thank-you page **quy đổi múi giờ** của khách
☐ `tel:+84…` đủ mã quốc gia · WhatsApp deep-link kiểm thật
☐ **Bảng kê ảnh cần cấp** có cột phạm vi đồng ý quốc tế
☐ Danh sách **`[PENDING]`** nêu rõ ai cấp
☐ **Scorecard ≥ 80**, và không gian lận điểm rào cản XA
