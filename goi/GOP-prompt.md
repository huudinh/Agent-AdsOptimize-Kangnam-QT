# PROMPT MẪU KN-QT — Ads Optimize Kangnam Quốc tế
> File này gộp **5 prompt mẫu** từ `prompts/`. Sinh tự động ngày 2026-10-22 bằng `python tools/gop-tham-khao.py`.
> ⛔ **Không sửa file này** — sửa ở bản rời trong thư mục nguồn rồi chạy lại lệnh trên.

**Cách đọc:** mỗi phần bắt đầu bằng dòng `===== tên file =====` và là **một đơn vị tri thức riêng**. Tham chiếu dạng `[[tên-file]]` trong văn bản trỏ tới **phần cùng tên ngay trong file này**, không phải file bên ngoài.

## MỤC LỤC

| # | File | Cỡ |
|---|---|---|
| 1 | `prompt-build-ad-set.md` | 5.5 KB |
| 2 | `prompt-build-landing-page.md` | 8.9 KB |
| 3 | `prompt-geo-answer.md` | 6.5 KB |
| 4 | `prompt-nghien-cuu-tu-khoa.md` | 6.4 KB |
| 5 | `prompt-quy-trinh-tron-goi.md` | 7.0 KB |


===== prompt-build-ad-set.md =====

# PROMPT MẪU — MODE 2 · WIN-AD (mẫu quảng cáo tiếng Anh)

> Dùng khi: đã có từ khoá **qua cổng WIN 3/4**.
> Đầu ra: Google RSA (15 headline + 4 description) + Meta (3–5 biến thể) + bảng chấm 14 điểm + kế hoạch test.

---

## 1 · PROMPT ĐẦY ĐỦ

```
MODE 2 — WIN-AD.

Nhóm từ khoá: [dán 3–8 từ khoá cùng một nhóm]
Market:       [vd AU]
Tầng:         [vd C]
Dịch vụ:      [vd Rhinoplasty]
Chặng:        [vd S4 — nếu biết; không biết thì tự suy và nói rõ]

Chạy B1→B7 đầy đủ, không bỏ bước:

B1 · Insight. Suy đủ 6 thứ, trong đó bắt buộc có market + tầng + ngôn ngữ
     + múi giờ, và ràng buộc chuyến đi.
     Rút 3–5 câu khách nói NGUYÊN VĂN, từ nguồn của ĐÚNG market này:
       - tầng C → RealSelf, r/PlasticSurgery, r/MedicalTourism
       - tầng B → group "Người Việt tại [nước]"
       - tầng D → group expat tại Hà Nội / TP.HCM
       - mọi tầng → Google autocomplete + People Also Ask, tra RIÊNG theo market
     Ghi kèm nguồn từng câu. Không tìm được → ghi "no voice of customer yet",
     KHÔNG bịa câu nói.

B2 · Chọn góc: A khát khao / B nỗi đau / C khả thi của chuyến đi.
     Chặng S4 thì ưu tiên góc C. 1 nội dung = 1 góc chính.

B3 · Viết ≥ 3 hook khác archetype. Mỗi hook = 1 insight + 1 bằng chứng
     ĐƯỢC PHÉP DÙNG Ở MARKET NÀY.
     Market AU/UK/EU/GCC: KHÔNG dùng archetype testimonial kết quả,
     KHÔNG dùng FOMO khan hiếm giả.

B4 · Dựng body theo tầng, CTA gắn ĐÚNG 1 KÊNH của market này.

B5 · Xuất mẫu:
     Google RSA — 15 headline ≤ 30 ký tự, phủ đủ 5 nhóm:
       dịch vụ+từ khoá (4) · USP/bằng chứng (3) · gỡ nỗi sợ (3)
       · giá/CTA (3) · logistics chuyến đi (2)
     4 description ≤ 90 ký tự + display path.
     ĐẾM KÝ TỰ TỪNG DÒNG và in số bên cạnh. Không ước lượng.
     Meta — 3–5 biến thể: hook + bằng chứng mạnh nhất nằm TRONG 125 KÝ TỰ ĐẦU,
     headline ≤ 40, description ≤ 30, gợi ý visual bằng chữ.
     Tầng C: visual chỉ được là cơ sở · phòng mổ · bác sĩ · bộ phận quốc tế
     · sơ đồ quy trình 5 bước. KHÔNG before-after, KHÔNG testimonial kết quả.

B6 · Ma trận A/B T1→T6. Nêu rõ lô nào chạy trước.

B7 · Bảng chấm WIN 7 tiêu chí, tổng __/14. Dưới 12 thì sửa rồi chấm lại,
     đừng xuất mẫu chưa đạt.

Cuối cùng: danh sách [PENDING] + nêu rõ CẦN PHÁP CHẾ THỊ TRƯỜNG NÀO duyệt.
```

---

## 2 · PROMPT NGẮN

```
MODE 2 — từ khoá "[từ khoá]", market [X], tầng [Y].
Chấm cổng WIN trước; qua cổng thì sinh RSA + Meta, đếm ký tự, chấm 14 điểm.
```

---

## 3 · PROMPT CHỈ CẦN HOOK

```
Viết 5 hook cho [dịch vụ], market [X], chặng [S?].
Mỗi hook: 1 câu khách nói thật + 1 bằng chứng được phép dùng ở market này.
Ghi rõ archetype và vì sao hook đó phù hợp với chặng này.
Market AU/UK/EU/GCC: nhớ không dùng testimonial kết quả.
```

---

## 4 · PROMPT CHO CHẶNG S4 — ngách tốt nhất

```
MODE 2 cho chặng S4 (kế hoạch chuyến đi), market [X], dịch vụ [Y].

Đây là ngách cạnh tranh gần bằng 0 và gần như không đối thủ nào dùng.
Viết mẫu quảng cáo theo GÓC C (khả thi của chuyến đi):
- 2 headline về số ngày ở lại (dùng [PENDING] nếu chưa có số từ Khoa Chuyên môn)
- 2 headline về phiên dịch / chăm sóc sau khi về nước
- 2 headline về đưa đón + khách sạn
- 1 description nói rõ "ai liên hệ với bạn, qua kênh gì, trong bao lâu"

⛔ KHÔNG tự suy số ngày ở lại. Đó là mốc y khoa.
```

---

## 5 · PROMPT RÀ SOÁT mẫu quảng cáo đã có

```
Rà bộ mẫu quảng cáo này trước khi tôi bật. Kiểm 8 điểm:

1. Có khai market + geo_mode + tầng chưa?
2. Headline nào vượt 30 ký tự? Description nào vượt 90? (đếm thật)
3. Meta: hook + bằng chứng có nằm trong 125 ký tự đầu không?
4. Còn từ cấm tiếng Anh nào? (best · #1 · top-rated · leading · guaranteed
   · permanent · lifetime warranty · painless · no scars · risk-free · cheapest)
5. Có dùng testimonial kết quả hoặc before-after cho market rủi ro cao không?
6. Có hứa số ngày ở lại hoặc mốc hồi phục cứng không?
7. Có so giá với quốc gia hoặc cơ sở CÓ TÊN không?
8. CTA có gắn đúng 1 kênh của market, hay gắn cả 5 kênh một lúc?

Chấm lại 14 điểm. Xuất bảng: mẫu nào · lỗi gì · sửa thành gì.
```

---

## Checklist nghiệm thu

☐ Dòng khai `Market · Tier · Stage · Language · Ad-risk` ở đầu
☐ **Phiếu cổng WIN x/4** xuất trước, kể cả khi loại
☐ 3–5 câu voice of customer **có nguồn, từ đúng market**
☐ 15 headline, **mỗi dòng có số ký tự in kèm**, không dòng nào > 30
☐ 4 description, không dòng nào > 90
☐ Có đủ **2 headline nhóm logistics chuyến đi**
☐ Meta: hook + bằng chứng **trong 125 ký tự đầu**
☐ CTA gắn **đúng 1 kênh** theo market
☐ Tầng C: **không** before–after, **không** testimonial kết quả trong gợi ý visual
☐ Bảng chấm **14 điểm**, tổng ≥ 12
☐ Tiêu chí ⑥ và ⑦ **không bị 0 điểm**
☐ Ghi rõ **cần Pháp chế thị trường nào** duyệt


===== prompt-build-landing-page.md =====

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


===== prompt-geo-answer.md =====

# PROMPT MẪU — MODE 5 · GEO-ANSWER (nội dung để AI trích dẫn)

> Dùng khi: muốn **AI trích dẫn Kangnam** khi khách nước ngoài hỏi ChatGPT · Gemini · AI Overview bằng tiếng Anh.
> Nguồn: [`knowledge/kn-truy-van-geo-qt.md`](../knowledge/kn-truy-van-geo-qt.md) — **83 truy vấn · 15 cụm · 53 CORE**.
> Đo bằng **Share of Voice**, không bằng CPL. Mục tiêu quý: **SoV ≥ 30%** ở cụm Tầng A.

## ⚠️ Đây là kênh khác, không phải quảng cáo

| | Ads (MODE 1–4) | **GEO (MODE 5)** |
|---|---|---|
| Đo bằng | CPL · chi phí/khách đến khám | **Share of Voice** |
| Nhịp | Tuần · cohort 8 tuần | **Quý** |
| Khung viết | **AIDA** (L1–L6) | **PAS** |
| `market` / `geo_mode` | ✅ bắt buộc | ⛔ **không có** |
| Cổng WIN 3/4 | ✅ | ⛔ không áp |

⛔ Đừng hỏi Agent chấm cổng WIN hay gắn `market` cho nội dung GEO — AI không có geo-targeting và không có CPC.

---

## 1 · PROMPT CHÍNH — làm một cụm

```
MODE 5 — GEO-ANSWER.

Cụm: [vd Q13 · Medical tourism logistics]
     (hoặc chỉ nói tên dịch vụ, Agent tự map sang cụm và nói rõ đã map vào đâu)

Làm theo G1→G7:

G1 · Xác nhận cụm + tầng ưu tiên. Nếu cụm này KHÔNG thuộc Tầng A mà 4 cụm
     Tầng A (Q10 · Q12 · Q11 · Q13) chưa làm xong → NÓI RÕ là đang đi sai thứ tự,
     và cho tôi biết vì sao thứ tự đó quan trọng.
G2 · Liệt kê các truy vấn CORE của cụm, nguyên văn tiếng Anh.
G3 · Với từng truy vấn, đọc cột "Khối trả lời cần có" — đó là brief, không phải
     gợi ý. Nêu luôn từ khoá ưu tiên và trang đích.
G4 · Rà mã rào R# của TỪNG truy vấn TRƯỚC KHI VIẾT. Nêu rõ: rào nào chạm,
     không được viết gì, thay bằng gì. (Rà sau là phải viết lại.)
G5 · Viết nội dung EN cho trang đích, khung PAS. Mỗi truy vấn là một H2/H3
     dùng ĐÚNG câu khách gõ, và trả lời ngay trong 2–3 câu đầu.
G6 · Tự soát R1 (cam kết kết quả) + R2 (DMKT) + R3 (pháp nhân) + R7 (thiết bị/
     số lưu hành) + R8 (KCB cho người nước ngoài) + R9 (bản EN vẫn cần GXNNDQC).
G7 · Ghi lại prompt đo SoV tương ứng và tháng sẽ đo lại.

Cuối cùng: danh sách [PENDING] nêu rõ AI CẤP.
```

---

## 2 · PROMPT NGẮN

```
MODE 5 cho cụm [Qxx]. Rà rào pháp lý trước khi viết.
```

---

## 3 · PROMPT SÓNG 1 — bốn cụm Tầng A

```
MODE 5 — Sóng 1, 90 ngày, 70% ngân sách EN.

Làm kế hoạch cho đúng 4 cụm Tầng A, theo thứ tự ưu tiên:
  Q10 · Choosing a hospital & surgeon   (15,5% điểm)
  Q12 · Safety, accreditation & licensing (12,8%)
  Q11 · Cost & price transparency (USD)   (11,7%)
  Q13 · Medical tourism logistics         (6,9%)

Với mỗi cụm cho tôi: số truy vấn CORE · trang đích · dạng nội dung cần sản xuất
· rào pháp lý phải qua · dữ liệu còn thiếu.

Nói rõ cụm nào BỊ CHẶN vì thiếu dữ liệu, và ai phải cấp dữ liệu đó.
⛔ Chưa cần viết nội dung ở bước này — tôi cần kế hoạch và danh sách chặn trước.
```

> Trang `/medical-tourism-guide` (Q13) cần **số ngày ở lại** — vẫn `[CHỜ CẬP NHẬT]`. Agent phải nêu điều này, không được viết bằng số tự suy.

---

## 4 · PROMPT ĐO SoV hằng tháng

```
MODE 5 — đo Share of Voice tháng [MM/YYYY].

Cho tôi 20 prompt đo ở dạng danh sách để tôi dán lần lượt, kèm hướng dẫn:
chế độ ẩn danh · ngôn ngữ giao diện EN · VPN/IP thị trường mục tiêu.

Rồi cho tôi khuôn bảng ghi kết quả: ChatGPT / Gemini / AI Overview
+ cột "đối thủ được AI nhắc".

Nhắc tôi vì sao cột đối thủ là cột quan trọng nhất.
```

**Bảng ghi kết quả:**

| # | Prompt | Cụm | ChatGPT | Gemini | AI Overview | Số nền tảng nhắc | Đối thủ AI nhắc |
|---|---|---|---|---|---|---|---|

`SoV = (số prompt có nhắc Kangnam) / (tổng số prompt)` — tính riêng từng nền tảng.

---

## 5 · PROMPT RÀ NỘI DUNG EN ĐÃ CÓ

```
Rà bài EN này theo bộ truy vấn GEO. Kiểm 7 điểm:

1. Bài trả lời truy vấn nào trong 83 truy vấn? Nếu không khớp cái nào →
   nói thẳng là bài này không phục vụ cụm nào.
2. Tiêu đề H2/H3 có dùng ĐÚNG câu khách gõ không, hay đang viết kiểu marketing?
3. Câu trả lời có nằm trong 2–3 câu đầu sau tiêu đề không?
4. Có đoạn nào là tính từ rỗng (AI không bao giờ trích) thay vì dữ kiện
   kiểm chứng được?
5. Rào R1 — còn "permanent" / "lifetime" / "100% safe" / "no scars"?
6. Rào R2/R3/R7 — có nêu kỹ thuật ngoài DMKT · gộp pháp nhân · thiết bị không
   rõ số lưu hành?
7. Bài có dùng khung AIDA (sai) thay vì PAS (đúng cho GEO)?

Xuất bảng: lỗi · vị trí · sửa thành gì. Rồi viết lại đoạn yếu nhất.
```

---

## 6 · PROMPT HỎI ĐÁP

```
Vì sao Tầng A là 4 cụm ngang dịch vụ, không phải trang dịch vụ?
```
```
Cụm nào đang bị chặn vì chưa chốt được điều kiện pháp lý, và chốt với ai?
```
*(Đáp án đúng: **Q08 Dental** — pháp nhân RHM · **Q09 BBL** — kỹ thuật có trong DMKT không + phải nói thật rủi ro thuyên tắc mỡ.)*
```
Rào R8 là gì và vì sao nó khác các rào còn lại?
```
*(Đáp án đúng: R2/R3/R7 nói về **câu chữ**; R8 nói về **điều kiện hoạt động** — có được tiếp nhận khách quốc tế hay không.)*

---

## Checklist nghiệm thu

☐ Mở đầu bằng `Cụm · Tầng · Giai đoạn GEO · Rào R#` *(không phải `Market · geo_mode` — đó là của kênh ads)*
☐ Nếu làm cụm Tầng B/C/D trước khi xong Tầng A → Agent **đã cảnh báo**
☐ Mỗi truy vấn có **mã rào R#**, và rà rào **trước khi viết**
☐ Tiêu đề `H2`/`H3` dùng **đúng câu khách gõ**, không nhồi từ khoá
☐ Câu trả lời nằm trong **2–3 câu đầu** sau tiêu đề
☐ Khung **PAS**, không phải AIDA
☐ Nội dung là **dữ kiện kiểm chứng được**, không phải tính từ
☐ Đã soát **R1 · R2 · R3 · R7 · R8 · R9**
☐ Có **prompt đo SoV** tương ứng + tháng sẽ đo lại
☐ Danh sách `[PENDING]` nêu rõ **ai cấp**
☐ ⛔ Không chấm cổng WIN, không gắn `market`/`geo_mode`, không đo bằng CPL


===== prompt-nghien-cuu-tu-khoa.md =====

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


===== prompt-quy-trinh-tron-goi.md =====

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

