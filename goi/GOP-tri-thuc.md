# TRI THỨC KN-QT — Ads Optimize Kangnam Quốc tế
> File này gộp **10 module tri thức** từ `knowledge/`. Sinh tự động ngày 2026-10-22 bằng `python tools/gop-tham-khao.py`.
> ⛔ **Không sửa file này** — sửa ở bản rời trong thư mục nguồn rồi chạy lại lệnh trên.

**Cách đọc:** mỗi phần bắt đầu bằng dòng `===== tên file =====` và là **một đơn vị tri thức riêng**. Tham chiếu dạng `[[tên-file]]` trong văn bản trỏ tới **phần cùng tên ngay trong file này**, không phải file bên ngoài.

## MỤC LỤC

| # | File | Cỡ |
|---|---|---|
| 1 | `kn-chan-doan-chi-so-qt.md` | 10.4 KB |
| 2 | `kn-chan-dung-hanh-trinh-qt.md` | 14.5 KB |
| 3 | `kn-cong-win-tu-khoa-qt.md` | 12.0 KB |
| 4 | `kn-engine-win-ad-qt.md` | 12.1 KB |
| 5 | `kn-ho-so-thuong-hieu-qt.md` | 22.5 KB |
| 6 | `kn-khung-landing-qt.md` | 27.8 KB |
| 7 | `kn-quy-trinh-tuan-qt.md` | 12.1 KB |
| 8 | `kn-rao-phap-ly-qt.md` | 19.3 KB |
| 9 | `kn-thi-truong-quoc-te.md` | 19.3 KB |
| 10 | `kn-truy-van-geo-qt.md` | 78.6 KB |


===== kn-chan-doan-chi-so-qt.md =====

# CHẨN ĐOÁN CHỈ SỐ QUỐC TẾ → QUYẾT ĐỊNH (MODE 4)
Version: 1.0 — 2026-10-21

---

## §1. PHỄU ĐO LƯỜNG QUỐC TẾ — 8 BƯỚC, KHÔNG PHẢI 3

Gói nội địa đo: `click → lead → booking`. Gói QT có **8 bước**, và chỗ rụng nằm ở những bước gói nội địa không có.

```
① click
② lead (form / WhatsApp)
③ phản hồi được  ← múi giờ + kênh
④ gửi ảnh đánh giá sơ bộ
⑤ nhận báo giá
⑥ ĐẶT CỌC        ← điểm chuyển trạng thái thật
⑦ đặt vé / xác nhận ngày
⑧ ĐẾN KHÁM (arrival)  ← chỉ số duy nhất đáng tin
```

**Chỉ số bắc đẩu: `chi phí trên một khách ĐẾN KHÁM` (cost per arrival).**

⛔ **CPL là chỉ số gây nhầm lẫn nhất của gói này.** Lead ở Campuchia rẻ gấp nhiều lần lead ở Úc, nhưng tỷ lệ đến khám khác hoàn toàn. So CPL giữa hai market là **so hai thứ khác nhau**.

**Hai chỉ số trung gian phải đo, nếu không thì mù:**
- **Tỷ lệ phản hồi được (bước ③)** — chẩn đoán vấn đề **múi giờ và kênh**, không phải vấn đề từ khoá.
- **Tỷ lệ đặt cọc (bước ⑥)** — đây là **điểm chuyển trạng thái thật** của du lịch y tế. Khách đặt cọc rồi gần như luôn đến. Chưa đặt cọc thì mọi thứ phía trước chỉ là ý định.

---

## §2. ⚠️ ĐỘ TRỄ — LUẬT CHẶN KẾT LUẬN SỚM

Độ trễ `lead → đến khám` của gói QT là **4–12 tuần** *(tầng B có thể tới 6 tháng nếu chờ dịp Tết)*.

**Hệ quả, không được bỏ qua:**

| Luật | Vì sao |
|---|---|
| ⛔ **Không kết luận chiến dịch tầng B/C trong cửa sổ < 8 tuần** | Lead tháng này thành ca tháng sau nữa. Cắt sớm là cắt đúng lúc nó bắt đầu chạy |
| ⛔ **Không so chi phí/arrival của tháng này với lead của tháng này** | Phải so **cohort**: lead tháng 1 → arrival của cohort tháng 1, đo ở tháng 3 |
| ✅ Tầng **D (expat)** đo được trong **1–2 tuần** | Không có rào cản đi lại → độ trễ gần như gói nội địa |
| ✅ Dùng **tỷ lệ đặt cọc** làm chỉ số sớm | Đặt cọc xảy ra sớm hơn arrival nhiều tuần, và tương quan chặt |

> **Đây là luật bị phá nhiều nhất.** Áp lực báo cáo hằng tuần làm team cắt chiến dịch tầng C ở tuần thứ 3 vì "CPL cao, chưa ra ca". Ca của nó đang trên đường — **theo nghĩa đúng của từ**.

**Agent bắt buộc:** nhận số liệu có cửa sổ < 8 tuần cho tầng B/C → **nói rõ ngay dòng đầu** rằng chưa kết luận được về hiệu quả cuối, chỉ đọc được các chỉ số sớm (CTR · tỷ lệ phản hồi · tỷ lệ đặt cọc).

---

## §3. SỐ LIỆU CẦN CÓ ĐỂ CHẨN ĐOÁN

| Nguồn | Chỉ số |
|---|---|
| **Google / Meta Ads** | CTR · CPC · CPL · chi phí · impression · từ khoá · **`market`** · **`geo_mode`** · search terms |
| **GA4** | scroll depth · time-on-page · form view → submit · click WhatsApp · tải cẩm nang · **phân tách theo country** |
| **CRM** | lead → phản hồi được → ảnh → báo giá → **đặt cọc** → vé → **arrival** · tag `market` + tầng + chặng · **thời gian phản hồi đầu tiên** |
| ★ **Vận hành quốc tế** | thời gian phản hồi theo múi giờ · kênh nào được trả lời · ngôn ngữ nào thiếu người |

**Ba tag bắt buộc trên mọi lead trong CRM:** `market` · `tier` · `stage`. Thiếu một tag → lead về CRM là **lead mù**, và mọi chẩn đoán phía sau là đoán.

Thiếu chỉ số nào → nói rõ **thiếu gì** và **kết luận nào chưa đưa ra được**, không suy đoán bù.

---

## §4. BẢNG TRIỆU CHỨNG → CHẨN ĐOÁN → QUYẾT ĐỊNH

| Triệu chứng | Chẩn đoán | Quyết định |
|---|---|---|
| CTR thấp + impression cao | Hook yếu hoặc sai đối tượng | Sửa mẫu QC (MODE 2) — **chưa đụng landing** |
| CTR cao + CVR thấp + scroll nông | Traffic vào nhưng landing không chốt | **Làm lại landing** — hero → khối gỡ rào cản → CTA |
| **Lead nhiều, không ai đến khám** ★ | **Trượt tiêu chí ④ travel intent**, hoặc **sai `geo_mode`** | **Quay cổng WIN §2/§4** — kiểm travel intent và `geo_mode` **trước** khi nghĩ tới landing |
| **Lead hỏi *"các bạn ở đâu"*** | `geo_mode` sai: traffic nước ngoài vào chiến dịch expat, hoặc ngược lại | **Sửa `geo_mode` ngay** — đây là lỗi cấu hình, sửa trong 5 phút |
| **Tỷ lệ phản hồi được thấp** ★ | **Múi giờ hoặc kênh**, không phải từ khoá | Thu trường *preferred contact time + timezone* (§7 `kn-khung-landing-qt.md`) · xếp ca trực theo market · đổi kênh sang WhatsApp |
| **Phản hồi được nhưng không gửi ảnh** | Luồng ảnh có ma sát hoặc khách lo riêng tư | Làm rõ: ai xem ảnh · lưu bao lâu · có dùng cho marketing không *(mặc định: không)* |
| **Báo giá rồi mất khách** ★ | **Giá bị sốc ở khâu phụ phí**, hoặc không trả lời được rào cản XA | Kiểm trang có nêu **phụ phí 10%** chưa · kiểm **B08/B09** có số ngày ở lại và ai lo sau khi về chưa |
| **Đặt cọc rồi không đến** | Vấn đề lịch bay / visa / không ai nhắc | Luồng nurture sau đặt cọc · hỗ trợ giấy tờ · nhắc theo mốc |
| CPC cao + cạnh tranh cao + CPL xấu | Từ khoá đắt / sai intent | Thu hẹp — vào **3 ngách §8** của cổng WIN |
| CVR ổn nhưng CPL vẫn cao | Bid / phân bổ ngân sách | **Giữ landing**, tối ưu bidding theo `market` |
| **CPL một market rẻ bất thường** | Thường là **tràn geo**: traffic từ market rẻ hơn lọt vào | Kiểm báo cáo theo country · siết `geo_mode` |

★ = triệu chứng riêng của gói QT.

**Mỗi dòng khi xuất phải kèm đủ 4 thứ:**
① ngưỡng cụ thể đang vi phạm · ② lý do dựa trên số · ③ action tiếp theo · ④ chỉ số cần theo dõi sau khi sửa.

---

## §5. BỐN QUYẾT ĐỊNH CỦA MODE 4

**① Đổi từ khoá?**
Khi intent lệch landing, hoặc CTR thấp + CPC cao, **hoặc lead không ra arrival** → quay `kn-cong-win-tu-khoa-qt.md`, chấm lại 4 tiêu chí với từ khoá hẹp hơn. **Kiểm tiêu chí ④ trước tiên.**

**② Làm lại landing?**
Khi CTR ổn nhưng CVR / scroll / form thấp. Sửa theo thứ tự: hero → **khối gỡ rào cản XA (B08/B09)** → CTA → form.

**③ Đổi mẫu QC hoặc đổi khung landing?**
Khi hook yếu, hoặc khung không khớp chặng. Chuyển L1↔L2↔L3↔L4 theo `kn-khung-landing-qt.md` §1.

**④ ★ Sửa cấu hình hoặc sửa vận hành?**
Quyết định riêng của gói QT, và **phải kiểm trước ba quyết định kia** vì nó rẻ nhất và nhanh nhất:
- `geo_mode` sai → sửa cấu hình.
- Tỷ lệ phản hồi thấp → **vấn đề vận hành** (ca trực, múi giờ, kênh, ngôn ngữ), **không phải vấn đề quảng cáo**.
- Thiếu người nói được ngôn ngữ của market → **tạm dừng market đó**, không đổ thêm tiền.

> **Luật thứ tự chẩn đoán:** ④ → ① → ② → ③. Làm lại landing trước khi kiểm `geo_mode` là tốn một tuần để sửa cái không hỏng.

---

## §6. ĐỊNH NGHĨA WIN BẰNG SỐ

Chưa có benchmark team → lấy **control hiện tại trong CÙNG market** làm mốc.

→ Mẫu nào **CTR cao hơn + tỷ lệ đặt cọc cao hơn control**, trong **cùng market, cùng chặng, cùng mùa** = winner.

**Ba điều kiện để được kết luận:**
① đủ lượng hiển thị/chi tiêu tối thiểu;
② **cửa sổ ≥ 8 tuần** cho tầng B/C (§2);
③ **cùng market** — ⛔ không bao giờ so winner giữa hai market.

Mẫu nhỏ hoặc cửa sổ ngắn → nói rõ *"chưa đủ dữ liệu để kết luận"*. Đây là lỗi tốn tiền nhất trong tối ưu ads: **scale một mẫu thắng nhờ may mắn**.

---

## §7. QUẢN TRỊ CREATIVE

- **Winner → scale** ngân sách, và nhân bản sang market **cùng nhóm luật quảng cáo**.
  ⛔ **Không nhân bản sang market khác nhóm luật.** Hook dùng testimonial thắng ở tầng A **không chuyển sang AU được** — không phải vì hiệu quả, mà vì **luật** (`kn-rao-phap-ly-qt.md` §2).
- Luôn giữ **1–2 challenger mới mỗi lô** — chống ad fatigue.
- Lưu **thư viện hook thắng theo market**, kèm dòng `Portable to` (`kn-engine-win-ad-qt.md` §8).
- **Theo mùa:** winner của mùa trước Tết (tầng B) không suy ra winner của mùa hè. Ghi `Conditions` gồm cả mùa.

---

## §7b. HAI TẦNG CHỈ SỐ — đọc ở hai nhịp khác nhau

| Tầng | Đo gì | Nguồn | Nhịp | Dùng để |
|---|---|---|---|---|
| **Sớm** | xem trang · time on site · tỷ lệ tương tác · thoát | **GA4** | hằng ngày/tuần | **sửa trang · sửa mẫu QC** |
| **Thật** | đặt cọc · đến khám · chi phí/đến khám | Ads + CRM | **cohort ≥ 8 tuần** | **quyết ngân sách** |

⛔ Không quyết ngân sách bằng chỉ số sớm — trang có time-on-site đẹp mà không ai đặt cọc vẫn là trang hỏng.
⛔ Không chờ chỉ số thật mới sửa trang — đợi 8 tuần mới biết hero sai là mất 8 tuần.

Trường GA4 cụ thể và khuôn báo cáo tuần: [`kn-quy-trinh-tuan-qt.md`](kn-quy-trinh-tuan-qt.md) §5.

---

## §8. BÁO CÁO — PHẢI CẮT THEO BỐN CHIỀU

Báo cáo theo chiến dịch là **không đủ** cho gói này. Luôn cắt theo:

① **`market`** — khác luật, khác giá, khác múi giờ.
② **Tầng (A/B/C/D)** — khác động cơ, khác độ trễ.
③ **Chặng (S1–S7)** — để thấy S4 đang làm việc hay không.
④ **Cohort theo tháng nhận lead** — để độ trễ không làm méo số.

**Bảng tối thiểu của mọi báo cáo MODE 4:**

| Market | Tầng | Chặng | Lead | % phản hồi | % đặt cọc | Arrival | **Chi phí/arrival** | Cohort |
|---|---|---|---|---|---|---|---|---|

Thiếu cột **Chi phí/arrival** và cột **Cohort** thì báo cáo không dùng được để ra quyết định — nó chỉ đẹp.


===== kn-chan-dung-hanh-trinh-qt.md =====

# CHÂN DUNG & HÀNH TRÌNH — KHÁCH THẨM MỸ QUỐC TẾ
Version: 1.0 — 2026-10-21

> Gói nội địa dùng **3 rào cản** và **phễu 6 giai đoạn**. Gói QT dùng **4 rào cản** và **phễu 7 chặng**.
> Hai phần thêm vào không phải để cho khác — chúng là chỗ mất khách thật của du lịch y tế.

---

## §1. INSIGHT NỀN — khách quốc tế mua gì

- Khách mua **kết quả cảm xúc** (tự tin · trẻ ra · được công nhận) — giống khách nội địa.
- Nhưng khách quốc tế đang mua thêm một thứ nữa: **một chuyến đi có thể kiểm soát được**. Họ không chỉ quyết định *"có mổ không"*, họ quyết định *"có bay không"*.
- → Nội dung phải trả lời **hai câu hỏi song song**: *"nơi này có an toàn không"* **và** *"chuyến đi này có chạy được không"*. Trả lời một câu mà bỏ câu kia là mất khách — và câu bị bỏ gần như luôn là câu thứ hai.

**Phép thử trước khi xuất bất kỳ landing nào:** *"Đọc trang này xong, khách có đủ thông tin để mở app hàng không và chọn ngày bay chưa?"* Chưa → trang chưa xong.

---

## §2. BỐN RÀO CẢN CHỐT

| Rào cản | Khách đang nghĩ gì | Bằng chứng gỡ | Nặng nhất ở tầng |
|---|---|---|---|
| **① SỢ** (Fear) | Đau không? Biến chứng không? Hỏng thì sao? Mổ ở nước ngoài có an toàn? | Giấy phép Bộ Y tế · quy trình mổ có văn bản · phòng mổ vô khuẩn · hội đồng chuyên môn · gây mê do bác sĩ chỉ định | **C** |
| **② NGỜ** (Doubt) | Cơ sở này có thật không? Có phép không? Bác sĩ có bằng gì? Giá có đúng như trang web? | Giấy phép · hồ sơ bác sĩ (bằng cấp, trường, năm) · **bảng giá công khai + phụ phí 10% nói trước** · International Patient Department | **A · D** |
| **③ NGẠI** (Reluctance) | Nghỉ bao lâu? Ai biết? Về nhà sưng thì giải thích thế nào? | Mốc hồi phục dạng khoảng · **kênh nhắn tin riêng tư** (WhatsApp/Telegram) · cam kết bảo mật | A · B · C |
| **④ XA ★** (Distance) | **Tôi bay về rồi thì ai lo cho tôi?** Phải ở lại bao nhiêu ngày? Nếu cần sửa lại thì ai trả tiền vé? Có ai nói được tiếng tôi không? | **Quy trình 5 bước cho khách ở xa** · phiên dịch tiếp tục sau khi về · **số ngày ở lại cụ thể** · T&C bảo hành/chỉnh sửa · lịch tái khám từ xa · ai là người liên hệ | **B · C ★** |

### 2.1 Rào cản ④ XA — vì sao nó là rào cản quyết định của gói này

Ba rào cản đầu, khách nội địa cũng có. Rào cản XA **chỉ có ở khách quốc tế**, và nó là rào cản **cuối cùng** — nghĩa là khách đã vượt qua Sợ, Ngờ, Ngại rồi mới chạm vào nó. Mất khách ở đây là mất khách **đắt nhất**: họ đã đọc hết trang, đã so giá, đã tin bác sĩ.

**Bốn câu hỏi của rào cản XA, theo thứ tự khách nghĩ:**

| # | Câu khách nghĩ | Trang phải trả lời bằng |
|---|---|---|
| 1 | *"Tôi phải ở Việt Nam bao nhiêu ngày?"* | **Một con số khoảng** + mốc nào (cắt chỉ · tái khám cuối · được phép bay) |
| 2 | *"Về nhà rồi có vấn đề thì liên hệ ai?"* | Tên bộ phận · kênh · ngôn ngữ · **trong bao lâu** |
| 3 | *"Nếu phải chỉnh sửa lại thì ai trả chi phí và chi phí bay?"* | **T&C bảo hành bằng văn bản** — không có thì không viết |
| 4 | *"Có ai nói được tiếng của tôi không, cả lúc mổ và sau khi về?"* | Phiên dịch: ngôn ngữ nào · có tính phí không · kéo dài bao lâu |

⛔ **Không trả lời được câu 1 thì khách không đặt vé** — và không đặt vé thì lead không bao giờ thành ca. Đây là lý do `kn-thi-truong-quoc-te.md` §8 là trường dữ liệu quan trọng nhất chưa có.

> **Luật gỡ rào cản:** mọi nội dung chốt phải gỡ **đúng rào cản của tầng + chặng đang nhắm**, không gỡ chung chung cả bốn. Gỡ sai rào cản = nói lạc đề với người đang lo chuyện khác.

---

## §3. BẢY CHÂN DUNG MẪU — dùng làm điểm khởi đầu, không dùng thay nghiên cứu

Mỗi chân dung thật phải trả lời đủ **7 câu** ở §4. Bảy chân dung dưới đây là khung mẫu theo tầng.

| Mã | Chân dung | Tầng | Nỗi đau thật | Rào cản chính | Giá trị ca |
|---|---|---|---|---|---|
| **QT1** | Phụ nữ 25–40, Phnom Penh / Jakarta / Manila, đã tìm hiểu clinic trong nước nhưng không tin tay nghề | A | *"Trong nước làm thì tôi không dám. Thái Lan thì đắt quá."* | **NGỜ** — cơ sở có thật, có phép không | Trung bình–Cao |
| **QT2** | Việt kiều nữ 35–55, Sydney / California, về VN dịp Tết hoặc hè | **B** | *"Mỗi lần về nhà tôi lại định làm, rồi lại thôi vì không biết sắp lịch thế nào."* | **XA** + NGẠI (họ hàng biết) | **Cao–Rất cao** |
| **QT3** | Việt kiều nam 30–50, về thăm nhà, hair transplant | **B** | *"Tôi không muốn ai ở công ty biết. Về VN làm thì không ai thấy quá trình."* | **NGẠI (riêng tư)** + XA | Cao |
| **QT4** | Nữ 30–50, Úc / NZ / Canada, đã báo giá ở nước mình và thấy không trả được | **C** | *"Ở Úc báo tôi 20.000 đô. Tôi không có số tiền đó, nhưng tôi vẫn muốn làm."* | **SỢ** + **XA** | **Rất cao** |
| **QT5** | Nữ/nam 28–45, GCC (UAE · Saudi · Kuwait) | **C** | *"Tôi cần nơi tôn trọng điều kiện của tôi, và không ai ở đây biết tôi đi đâu."* | NGẠI (riêng tư) + NGỜ (có đáp ứng được điều kiện không) | **Rất cao** |
| **QT6** | Expat 28–45 đang sống & làm việc tại HN / TP.HCM | **D** | *"Tôi sống ở đây rồi. Tôi chỉ cần một bác sĩ nói được tiếng Anh và một cuộc hẹn tuần này."* | **NGỜ** (giao tiếp · tiêu chuẩn) | Trung bình–Cao |
| **QT7** ★ | **Khách đã làm ở nơi khác và cần sửa lại** — bất kể tầng | A · B · C | *"Tôi đã làm một lần ở [nơi khác] và nó hỏng. Giờ tôi không tin ai nữa."* | **NGỜ, ở mức mất niềng tin vào cả ngành** | **Cao nhất** |

### 3.1 Hai chân dung không được gộp vào nhóm khác

**QT7 (khách sửa lại)** — tách hẳn, như gói nội địa. Nhóm này **đã mất niềm tin**, cần bộ bằng chứng khác (hồ sơ bác sĩ ca khó · quy trình đánh giá lại · chính sách rõ về trường hợp phức tạp) và **trả được CPC cao nhất**. Gộp họ vào nhóm khách lần đầu là mất nhóm sẵn sàng trả nhiều nhất.

**QT2/QT3 (kiều bào)** — tách khỏi tầng C dù cùng sống ở Úc/Mỹ. Họ tìm bằng **tiếng Việt**, đã tin thương hiệu Việt, và **đã có vé máy bay**. Gộp vào chiến dịch tiếng Anh là không bao giờ gặp họ.

---

## §4. BẢY CÂU MỖI CHÂN DUNG PHẢI TRẢ LỜI

Năm câu đầu giống gói nội địa. Câu 6 và 7 là của gói QT.

1. **Ai** — tuổi, nghề, tình huống (lần đầu / sửa lại / trước cưới / sau sinh).
2. **Nỗi đau thật** — không phải *"muốn đẹp"*, mà câu họ tự nói.
3. **Rào cản chốt chính** — đúng **1** trong SỢ / NGỜ / NGẠI / **XA**.
4. **Người gõ có phải người điều trị không** — chồng tìm cho vợ, con tìm cho mẹ. Nếu không → viết cho **người mua hộ**.
5. **Giá trị ca** — quyết định được phép trả CPC bao nhiêu.
6. ★ **`market` + ngôn ngữ + múi giờ** — ở đâu, tìm bằng ngôn ngữ nào, gọi lại được vào giờ nào theo giờ của họ.
7. ★ **Ràng buộc chuyến đi** — bay được bao nhiêu ngày · đi một mình hay có người đi cùng · cửa sổ thời gian nào (Tết · hè · trước cưới · ngoài Ramadan) · có cần visa không.

Không viết được câu 6 hoặc câu 7 thì **chưa đủ dữ liệu để dựng chiến dịch**.

---

## §5. PHỄU 7 CHẶNG — S1 → S7

Gói nội địa có 6 chặng. Gói QT chèn thêm **S4 · LÊN KẾ HOẠCH CHUYẾN ĐI** giữa *cân nhắc* và *thực hiện*. Đây là chặng khách rụng nhiều nhất mà **không ai đo**, vì nó xảy ra sau khi lead đã vào CRM.

| Chặng | Nhiệt | Tâm lý | Dấu hiệu trong từ khoá (EN) | Rào cản | Landing |
|---|---|---|---|---|---|
| **S1 NHẬN BIẾT** | Cold | Chưa nghĩ tới đi nước ngoài | *"what is rhinoplasty"* · *"should I get"* | — | ❌ Không chạy landing chốt |
| **S2 SO SÁNH ĐIỂM ĐẾN ★** | Cold→Warm | **Chọn nước, chưa chọn bệnh viện** | *"plastic surgery in vietnam"* · *"vietnam vs thailand plastic surgery"* · *"is vietnam safe for plastic surgery"* · *"cheaper than korea"* | NGỜ | **L1 — Destination** |
| **S3 CÂN NHẮC & NỖI SỢ ★** | Warm→Hot | Đã chọn VN, đang sợ | *"is rhinoplasty in vietnam safe"* · *"vietnam plastic surgery horror"* · *"reviews"* · *"revision"* | **SỢ** | **L2 — Answer-first** |
| **S4 LÊN KẾ HOẠCH CHUYẾN ĐI ★★** | Hot | **Đã muốn làm, đang tính có đi được không** | *"how many days"* · *"recovery before flying"* · *"hospital hanoi english speaking"* · *"visa"* · *"hotel near"* · *"interpreter"* | **XA** | **L3 — Trip-planning** |
| **S5 THỰC HIỆN** | Hot | Sẵn sàng, cần giá và đặt lịch | *"cost"* · *"price"* · *"package"* · *"book consultation"* | NGẠI (chi phí) | **L4 — Price & Book** |
| **S6 HẬU PHẪU TỪ XA ★** | Existing | **Đã về nước, đang lo** | *"swelling after"* · *"when can I fly"* · *"aftercare"* | XA | Trang hướng dẫn / CRM — ❌ không chạy ads chốt |
| **S7 GẮN BÓ & GIỚI THIỆU** | LTV | Hài lòng → kể lại | *"other procedures"* · *"second trip"* | — | L4 cho dịch vụ mới |

★ = chặng không có tương đương trực tiếp ở gói nội địa. ★★ = **chặng quyết định của gói QT**.

### 5.1 S4 là chặng quyết định — và là chặng bị bỏ ngân sách

Gói nội địa dồn ngân sách vào S3 (nỗi sợ). Gói QT phải dồn vào **S3 và S4**.

**Vì sao S4 là nơi mất khách đắt nhất:**
- Khách đến S4 đã **vượt qua cả Sợ và Ngờ**. Họ muốn làm. Họ chỉ đang tính xem **chuyến đi có chạy được không**.
- Từ khoá S4 (*"how many days in vietnam after rhinoplasty"* · *"english speaking plastic surgeon hanoi"*) có **cạnh tranh thấp nhất** trong cả phễu, vì đối thủ đổ tiền vào từ khoá giá.
- Nhưng trang trả lời được S4 thì **hầu như không ai làm**, nên ai làm trước thì chiếm.

→ **Luật ngân sách: S4 tối thiểu 15%.** S3 tối thiểu 10%. Chi tiết ở `kn-cong-win-tu-khoa-qt.md`.

### 5.2 S2 — chặng chọn điểm đến, không phải chọn bệnh viện

Khách tầng C vào phễu ở **S2**, không ở S3: họ đang hỏi *"nước nào"* trước khi hỏi *"bệnh viện nào"*. Landing S2 vì vậy **không bán Kangnam trước** — nó trả lời câu hỏi về **Việt Nam** (giấy phép · đào tạo của bác sĩ · tiêu chuẩn bệnh viện · chi phí · logistics), rồi mới đặt Kangnam vào như câu trả lời.

⛔ Dùng landing bán dịch vụ cho từ khoá S2 là nguyên nhân phổ biến nhất của **CTR tốt, bounce cao** ở tầng C.

### 5.3 S6 không chạy ads — nhưng phải có trang

Khách S6 **đã là bệnh nhân** và đang ở nước họ, lo lắng, lệch múi giờ. Họ sẽ google thay vì chờ phiên dịch trả lời.
→ Cần trang hướng dẫn hậu phẫu bằng tiếng Anh, **không chạy ads**, dùng trong CRM và tin nhắn WhatsApp. Trang này là **tài sản giữ review tốt** và là nguồn của S7.

---

## §6. NHẬN DIỆN CHẶNG TỪ MỘT TỪ KHOÁ LẠ

Chạy theo thứ tự, dừng ở dòng khớp đầu tiên:

1. Có **`how many days` · `before flying` · `visa` · `interpreter` · `hotel` · `english speaking` · `airport pickup`** → **S4**.
2. Có **`cost` · `price` · `how much` · `package` · `book`** → **S5**.
3. Có **`safe` · `safety` · `risk` · `pain` · `review` · `horror` · `revision` · `gone wrong`** → **S3**.
4. Có **tên nước khác** (`vs thailand` · `vs korea` · `vs turkey`) hoặc **`in vietnam` mà không có dịch vụ cụ thể** → **S2**.
5. Có **`what is` · `should I` · `types of`** → **S1**.
6. Có **`after` · `swelling` · `aftercare` · `recovery tips`** → **S6**.
7. Không khớp → **hỏi lại người dùng, không đoán bừa.**

> ⚠️ Bước 1 đặt **trước** bước 2 là có chủ ý. Từ khoá S4 thường chứa cả chữ về chi phí (*"how many days and how much"*) — nhưng intent chính là **kế hoạch**, và landing giá không trả lời được nó.

---

## §7. BẢN ĐỒ THÔNG ĐIỆP — chặng × rào cản × bằng chứng

| Chặng | Rào cản phải gỡ | Bằng chứng bắt buộc có trên trang | CTA đúng nấc |
|---|---|---|---|
| **S2** | NGỜ | Giấy phép Bộ Y tế · bác sĩ đào tạo Hàn · tiêu chuẩn bệnh viện · bảng giá công khai · International Patient Dept | **Micro** — nhận bảng giá / cẩm nang điểm đến |
| **S3** | **SỢ** | Giấy phép · hồ sơ bác sĩ · quy trình mổ có văn bản · phòng mổ vô khuẩn · hội đồng chuyên môn · *(tầng C: **không** dựa vào testimonial/before-after)* | **Mid** — chat WhatsApp với bộ phận quốc tế |
| **S4** ★ | **XA** | **Số ngày ở lại** · quy trình 5 bước · phiên dịch sau khi về · T&C bảo hành · đưa đón + khách sạn · ai liên hệ, trong bao lâu | **Mid** — gửi ảnh nhận đánh giá sơ bộ *(bác sĩ thực hiện)* |
| **S5** | NGẠI (chi phí) | Bảng giá + **phụ phí 10%** + cái gì có trong giá + giá cuối do bác sĩ chốt | **Macro** — đặt lịch tư vấn / giữ suất |
| **S6** | XA | Hướng dẫn hậu phẫu · mốc tái khám từ xa · khi nào được bay · kênh liên hệ | — *(không bán)* |
| **S7** | — | Dịch vụ tiếp theo · ưu đãi khách cũ | Macro |

**Luật:** chặng S1 và S6 **không chạy landing chốt**. Ép bán ở đây là đốt ngân sách và làm hỏng niềm tin.


===== kn-cong-win-tu-khoa-qt.md =====

# CỔNG WIN QUỐC TẾ — Nghiên cứu, chấm & gom nhóm từ khoá
Version: 1.0 — 2026-10-21

> Cổng này chạy **trước mọi việc sản xuất nội dung**. Từ khoá không qua cổng thì không viết mẫu quảng cáo, không dựng landing.
> Gói nội địa dùng **3 tiêu chí, qua 2/3**. Gói QT dùng **4 tiêu chí, qua 3/4** — tiêu chí thứ tư là của du lịch y tế.

---

## §1. BƯỚC 0 — TIỀN LỌC (bắt buộc)

Từ khoá phải nêu được **≥ 2 trong 4 thứ**: dịch vụ · điểm đến (Vietnam / Hanoi / HCMC) · intent · ngữ cảnh quốc tế.

| Loại | Ví dụ | Phán quyết |
|---|---|---|
| Quá rộng | `plastic surgery` · `beauty` · `cosmetic` | ⛔ Loại |
| Không intent | `aesthetic hospital` | ⛔ Loại |
| Lệch lĩnh vực | `korean skincare routine` | ⛔ Loại |
| **Lệch điểm đến** | `plastic surgery korea` · `rhinoplasty turkey` | ⛔ **Loại — và đưa vào phủ định** |
| Qua cổng | `rhinoplasty cost vietnam` · `is plastic surgery in vietnam safe` · `how many days in vietnam after nose surgery` · `english speaking plastic surgeon hanoi` | ✅ Chấm tiếp |

> ⚠️ **Từ khoá tên nước khác** (`korea` · `thailand` · `turkey` · `mexico`) chia làm hai loại, xử lý khác nhau:
> - `rhinoplasty korea` — người tìm **muốn đi Hàn**, không muốn đi VN → **phủ định**.
> - `vietnam vs korea plastic surgery` · `cheaper than korea` — người tìm **đang so sánh**, chưa quyết → **S2, giữ lại, giá trị cao**.
>
> Phân biệt bằng: có chữ `vs` · `compare` · `or` · `cheaper than` · `instead of` → giữ. Chỉ có tên nước khác → phủ định.

---

## §2. BỐN TIÊU CHÍ LÕI — đạt ≥ 3/4 mới được sản xuất nội dung

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---|---|---|---|
| ① | **Sát chuyển đổi (CR)** | Intent mua hoặc intent kế hoạch: `cost` · `price` · `how many days` · `book` · `best hospital for` · tên dịch vụ cụ thể | Thông tin thuần: `what is` · `types of` · `how does it work` |
| ② | **Cạnh tranh ít → bid thấp** | Ngách · dài · **tiếng Việt cho tầng B** · **từ khoá S4 (kế hoạch chuyến đi)** | Từ khoá đầu ngành ở thị trường tiếng Anh — nơi clinic Thái/Hàn/Thổ đổ tiền |
| ③ | **Giá trị ca lớn ($)** | breast augmentation · rib-cartilage rhinoplasty · V-line · facelift · Lipo 360 · hair transplant | Dịch vụ giá thấp đứng **đơn lẻ**: mí mắt · da liễu · spa (xem §3) |
| ④ ★ | **Ý chí đi lại (travel intent)** | Từ khoá cho thấy người này **chấp nhận đi nước ngoài**: có `vietnam` / `hanoi` / `ho chi minh` / `abroad` / `overseas` / `medical tourism`, **hoặc** thuộc tầng **B/D** (vé đã có / đã ở VN) | Từ khoá thuần địa phương nước họ: `rhinoplasty sydney` · `nose job near me` — người này **không có ý định bay** |

### 2.1 Vì sao tiêu chí ④ tồn tại

Ba tiêu chí của gói nội địa đo *"người này có mua không"*. Với khách quốc tế còn một câu nữa: **"người này có bay không"**.

> `rhinoplasty cost` gõ từ Sydney — intent mua rõ, giá trị ca cao, nhưng người này đang hỏi giá **ở Sydney**. Họ đạt ①②③ và **trượt ④**. Chạy từ khoá này là trả tiền để gặp người sẽ không bao giờ bay.

→ Tiêu chí ④ là tiêu chí **cắt tiền** của gói này. Bỏ nó là nguyên nhân chính của *"CTR tốt, lead có, không ai đến khám"*.

### 2.2 Quyết định

- **< 3/4 → KHÔNG làm nội dung.** Thu hẹp (thêm `vietnam` · thêm dịch vụ cụ thể · thêm intent kế hoạch) rồi chấm lại.
- **≥ 3/4 → chuyển MODE 2 (WIN-AD).**
- **Trượt riêng tiêu chí ④ → không thu hẹp được bằng cách thêm chữ.** Phải đổi từ khoá hoặc đổi `market`.

**Luôn xuất phiếu chấm, kể cả khi loại:**

```
WIN GATE SCORECARD
Keyword:        "rhinoplasty cost vietnam"
Market:         AU (Tier C) · geo_mode: Presence+Interest
Pre-filter:     PASS (service + destination + intent)
① CR intent:        PASS — "cost", intent mua rõ
② Low competition:  FAIL — từ khoá đầu ngành ở thị trường EN
③ High case value:  PASS — rhinoplasty, nhóm biên cao
④ Travel intent:    PASS — có "vietnam"
→ 3/4 · PASSES GATE → MODE 2
Stage:          S5 (price intent)
Note:           Thêm biến thể S4 hẹp hơn để kéo CPC xuống:
                "how many days in vietnam after rhinoplasty"
```

---

## §3. LUẬT COMBO — dịch vụ giá thấp cho khách quốc tế

Không ai bay 6 giờ để cắt mí.

| Dịch vụ | Tầng A/B/C | Tầng D |
|---|---|---|
| Eyelid · da liễu · clinic · spa đơn lẻ | **`win` tối đa 2/4** → không dựng landing riêng. Chỉ dùng làm **cụm combo / cross-sell** | ✅ chấm bình thường |

→ `ghi_chu` phải khai: *"combo/cross-sell only — no dedicated landing"*.
→ Cách đúng để bán dịch vụ giá thấp cho tầng A/B/C: **ghép vào gói** với một ca lớn, và nói rõ *"performed in the same trip"* — đó chính là lợi thế thật của du lịch y tế.

---

## §4. ⚠️ CỔNG GEO — chặn trước khi chấm điểm

Mọi dòng từ khoá phải khai **hai trường**. Thiếu → không chấm, không xuất.

| Trường | Nghĩa |
|---|---|
| `market` | **Người gõ đang ở đâu** — không phải thành phố trong từ khoá |
| `geo_mode` | `Presence` hoặc `Presence+Interest` |

**Bẫy:** từ khoá có tên thành phố Việt Nam là **hai người khác nhau**.

| Từ khoá | `market` | `geo_mode` | Chân dung | Landing |
|---|---|---|---|---|
| `plastic surgery hanoi` | `AU` | `Presence+Interest` | QT4 — khách Úc sắp bay | **L3 Trip-planning** |
| `plastic surgery hanoi` | `VN-EXPAT` | **`Presence`** | QT6 — expat đang sống ở HN | **L5 Expat** — ⛔ không có khối du lịch |

→ **Cùng chuỗi ký tự, hai dòng từ khoá, hai chiến dịch, hai landing.** Đây là cách đúng, không phải trùng lặp.

⛔ Để Google tự chọn kiểu nhắm (mặc định `Presence or interest`) cho chiến dịch expat → tràn traffic quốc tế, CPL trông rẻ, không ai đến khám. **Lỗi này im lặng** — Google Ads không cảnh báo.

**Cổng tự động:** generator chặn build nếu dòng từ khoá có tên thành phố VN mà thiếu `market` hoặc `geo_mode`.

---

## §5. GOM NHÓM

**1 nhóm = 1 dịch vụ × 1 chặng (S1–S7) × 1 intent × 1 tầng thị trường.**
→ 1 nhóm = **1 landing page + 1 bộ mẫu quảng cáo**.

Chiều **tầng thị trường** là chiều thêm vào so với gói nội địa, và **không được lược bỏ**: cùng dịch vụ, cùng chặng, cùng intent, nhưng khách Campuchia và khách Úc cần hai trang khác nhau vì **luật quảng cáo khác, bộ bằng chứng được phép dùng khác, ngôn ngữ khác**.

⛔ **Không trộn:**
- hai chặng vào một landing (người hỏi *"có an toàn không"* và người hỏi *"bao nhiêu tiền"* cần hai trang);
- hai tầng vào một chiến dịch (khác luật quảng cáo → khác creative được phép dùng);
- tầng B (tiếng Việt) vào chiến dịch tiếng Anh;
- tầng D (expat, `Presence`) vào chiến dịch du lịch y tế.

**Quy ước tên chiến dịch:**
```
KN-QT | <tầng> | <market> | <chặng> | <cụm truy vấn>

KN-QT | C | AU | S5 | Price & Package
KN-QT | B | VN-DIASPORA-AU | S4 | Lịch trình về nước
KN-QT | D | VN-EXPAT | S5 | Book - English speaking
```
Tên này là **khoá nối** sang sheet từ khoá và sheet tối ưu. Sửa một nơi phải sửa cả hai.

---

## §6. PHÂN BỔ NGÂN SÁCH — theo ý định × giá trị ca, KHÔNG theo lượng tìm kiếm

| Chặng | Tỷ trọng tối thiểu | Vì sao |
|---|---|---|
| S2 · So sánh điểm đến | — | Cold, dùng để nuôi phễu tầng C |
| **S3 · Nỗi sợ** | **≥ 10%** | Chặng rụng khách, cạnh tranh thấp |
| **S4 · Kế hoạch chuyến đi ★** | **≥ 15%** | **Chặng rụng khách đắt nhất, cạnh tranh thấp nhất, gần như không đối thủ nào làm** |
| S5 · Giá & đặt lịch | — | Hot nhưng đắt nhất — không dồn hết vào đây |
| **Tầng B (kiều bào)** | **≥ 15%** | Tầng dễ chốt nhất và rẻ nhất, thường bị bỏ |

Tổng đúng **100%**.

⛔ **Không chia ngân sách theo lượng tìm kiếm.** `plastic surgery vietnam` có volume lớn nhất và giá trị thấp nhất.
⛔ **Không cắt S4 vì CPL cao hơn S5** — S4 có CPL cao hơn nhưng **tỷ lệ đến khám cao hơn nhiều**, và đó là chỉ số thật (xem `kn-chan-doan-chi-so-qt.md`).

---

## §7. KIỂU KHỚP & HAI CỘT ĐỂ TRỐNG

- Chỉ **Exact / Phrase**. **Không Broad** cho tới khi đã import được chuyển đổi offline (đặt cọc / đến khám).
- **Để TRỐNG `volume` và `cpc`** — hai số đó lấy từ Keyword Planner, **không ước lượng, không bịa**.
  → Quan trọng hơn ở gói QT: Keyword Planner phải chạy **theo từng `market`**, vì volume và CPC của `rhinoplasty vietnam` ở Úc và ở Campuchia khác nhau hoàn toàn.
- Từ khoá đầu ngành chấm `1/4` hoặc `2/4`: **vẫn giữ để hứng volume**, nhưng để P3/P4, **không sản xuất nội dung riêng**, và ghi rõ quy tắc cắt trong `ghi_chu`.

---

## §8. BA NGÁCH ƯU TIÊN CỦA GÓI QT

Xếp theo tỷ lệ *(giá trị / cạnh tranh)*, cao nhất trước:

**① Từ khoá kế hoạch chuyến đi (S4).** `how many days in vietnam after rhinoplasty` · `english speaking plastic surgeon hanoi` · `airport pickup hospital vietnam` · `interpreter plastic surgery vietnam` · `can i fly after rhinoplasty`.
→ Cạnh tranh gần như bằng không. Người gõ đã quyết định làm. **Ngách tốt nhất của cả gói.**

**② Từ khoá tiếng Việt từ nước ngoài (tầng B).** `nâng mũi ở việt nam cho việt kiều` · `về việt nam thẩm mỹ dịp tết` · `bệnh viện thẩm mỹ cho việt kiều`.
→ Không đối thủ quốc tế nào đấu. Khách đã tin thương hiệu Việt và đã có vé.

**③ Từ khoá sửa lại (QT7).** `revision rhinoplasty vietnam` · `fix bad nose job abroad` · `botched surgery revision`.
→ Giá trị ca cao nhất, nhưng cần bộ bằng chứng riêng và **giọng khác hẳn**: không bán kết quả, bán **đánh giá lại**.

**Ba ngách này cộng lại nên chiếm ≥ 40% ngân sách** ở giai đoạn đầu, trước khi đấu vào từ khoá giá.

---

## §8b. BA NGUỒN LẤY TỪ KHOÁ — theo thứ tự

| # | Nguồn | Lấy gì |
|---|---|---|
| ① | **Bộ truy vấn GEO** (`kn-truy-van-geo-qt.md`) | 83 truy vấn đã phân tầng, đã gắn rào pháp lý — **câu khách thật sự gõ** |
| ② | **Landing đang chạy** | GA4 `sessionGoogleAdsQuery` · `sessionGoogleAdsKeyword` + Search terms — khách **đang** gõ gì |
| ③ | **Keyword Planner** | Chỉ để **điền 2 cột trống** `volume` · `cpc`, chạy riêng theo từng market |

⛔ **Không bắt đầu từ Keyword Planner.** Volume lớn nhất gần như luôn là từ khoá giá trị thấp nhất. Bắt đầu từ ① và ②, dùng ③ để định giá.

Vòng lặp tuần đầy đủ: [`kn-quy-trinh-tuan-qt.md`](kn-quy-trinh-tuan-qt.md).

---

## §9. KHI NÀO QUAY LẠI CỔNG NÀY

MODE 4 (OPTIMIZE) chẩn đoán ra **"đổi từ khoá"** → quay về đây. Ba triệu chứng dẫn về cổng này:
- CTR thấp + CPC cao + cạnh tranh cao → thu hẹp, tìm ngách §8.
- **Lead nhiều, không ai đến khám** → kiểm tiêu chí ④ (travel intent) và cổng GEO-TARGET §4. Gần như luôn là một trong hai.
- Lead toàn hỏi *"các bạn ở đâu"* → sai `geo_mode`.


===== kn-engine-win-ad-qt.md =====

# ENGINE WIN-AD QUỐC TẾ — B1→B7 & template mẫu quảng cáo tiếng Anh
Version: 1.0 — 2026-10-21

Chạy tuần tự **sau khi** từ khoá đã qua cổng 3/4 (`kn-cong-win-tu-khoa-qt.md`). Đọc kết quả & lặp ở MODE 4.

---

## B1 · INSIGHT TỪ TỪ KHOÁ

Từ từ khoá, suy ra đủ **6 thứ** (bốn thứ đầu giống gói nội địa, hai thứ sau là của gói QT):

1. **Khách là ai** — tuổi, giới, hoàn cảnh.
2. **Chặng phễu** — S1→S7, tra `kn-chan-dung-hanh-trinh-qt.md` §6.
3. **Nỗi đau / khát khao.**
4. **Job-to-be-done.**
5. ★ **`market` + tầng + ngôn ngữ + múi giờ** — quyết định luật quảng cáo nào áp và viết bằng ngôn ngữ nào.
6. ★ **Ràng buộc chuyến đi** — cửa sổ thời gian, đi cùng ai, bay được mấy ngày.

**Bắt buộc rút 3–5 câu nói nguyên văn của khách**, và với gói QT phải **rút từ nguồn của đúng thị trường đó**:

| Nguồn | Dùng cho tầng |
|---|---|
| RealSelf · r/PlasticSurgery · r/MedicalTourism (Reddit) | **C** — nguồn tốt nhất, khách viết dài và thật |
| Facebook group *"Vietnamese in Australia"*, *"Người Việt tại Mỹ"* | **B** — nguồn tiếng Việt |
| Google autocomplete + People Also Ask **theo từng market** | A · C · D |
| Review Google Maps của Kangnam và của đối thủ VN/Thái | A · C |
| Group expat (*"Hanoi Massive"*, *"Expats in HCMC"*) | **D** |
| Bình luận dưới ads của clinic Thái Lan / Thổ Nhĩ Kỳ | **C** — thấy đúng phản đối thật |

⛔ Autocomplete phải tra **theo đúng market** — gợi ý ở Úc và ở Campuchia khác nhau hoàn toàn.
⛔ Không tìm được câu thật → ghi rõ **"no voice of customer yet"**, không bịa câu nói.

**Voice of customer luôn win hơn văn marketing.** Với gói QT còn mạnh hơn, vì khách viết rất cụ thể về logistics — đó là chỗ lấy được hook mà đối thủ không có.

---

## B2 · CHỌN GÓC

| Góc | Dùng khi |
|---|---|
| **A — khát khao kết quả** | Khách đã muốn làm, đang chọn nơi |
| **B — nỗi đau / khiếm khuyết** | Intent xuất phát từ khiếm khuyết hoặc nỗi sợ |
| **C ★ — khả thi của chuyến đi** | ★ **Góc riêng của gói QT.** Khách đã muốn làm, đang tính *"đi được không"*. Nói về số ngày · phiên dịch · đưa đón · chăm sóc sau khi về |

**1 nội dung = 1 góc chính.** Trộn hai góc làm loãng cả hai.

**Góc C là góc thắng ở chặng S4** và gần như không đối thủ nào dùng. Hook góc C:
> *"7 days in Vietnam. Interpreter from arrival to flight home."* *(số ngày là ví dụ — phải lấy số thật từ Khoa Chuyên môn)*

> ⚠️ **GÓC ≠ KHUNG LANDING.** Góc quyết định *quảng cáo nói về cái gì*. Khung landing chọn theo **chặng + tầng** — xem `kn-khung-landing-qt.md`.

---

## B3 · HOOK — quyết định ~80% hiệu quả

Hook = **3 giây đầu / dòng 1 / headline**. Viết **≥ 3 hook khác archetype** cho mỗi nhóm. Mỗi hook = **1 insight (B1) + 1 bằng chứng được phép dùng ở market đó**.

| # | Archetype | Khung | Dùng tốt ở |
|---|---|---|---|
| 1 | Câu hỏi chốt intent | *"Considering [service] in Vietnam?"* | S2 · S3 |
| 2 | **Trả lời trước** | *"[Fear]? Here is the answer."* | **S3** |
| 3 | **Logistics cụ thể ★** | *"[N] days in Vietnam. Interpreter included."* | **S4 ★** |
| 4 | Minh bạch giá | *"Full price list published. 10% international service charge."* | **S5** |
| 5 | Bằng chứng giấy phép | *"MOH-licensed hospital. Licence 287/BYT-GPHĐ."* | Mọi chặng |
| 6 | Hồ sơ bác sĩ | *"Operated by a surgeon with 20+ years — Hanoi Medical University."* | S3 · S5 |
| 7 | So sánh điểm đến | *"Vietnam or Thailand? Compare on the things that matter."* | **S2** |
| 8 | Phá vỡ hiểu lầm | *"Think surgery abroad means no aftercare? Read this."* | S3 · S4 |
| 9 | Ngách sửa lại | *"Previous surgery did not go well? Start with an assessment."* | **QT7** |
| 10 | Kiều bào *(tiếng Việt)* | *"Về Việt Nam dịp Tết? Sắp lịch thẩm mỹ gọn trong chuyến đi."* | **Tầng B** |

⛔ **Archetype cấm ở tầng C:** social proof dạng testimonial kết quả, và FOMO khan hiếm giả. Xem `kn-rao-phap-ly-qt.md` §2.
⛔ Archetype cần **số thật** (3 · 4 · 6): không có số đã duyệt → đổi archetype, **không bịa số**.

---

## B4 · DỰNG BODY THEO TẦNG THÔNG ĐIỆP

```
HOOK
 → gọi đúng nỗi đau / khát khao / lo lắng về chuyến đi
 → giải pháp + USP
 → bằng chứng (gỡ đúng rào cản của chặng: SỢ · NGỜ · NGẠI · XA)
 → minh bạch chi phí (nếu S5)
 → CTA + kênh liên hệ đúng market
```

**Mỗi câu một nhiệm vụ.** Bằng chứng phải khớp **chặng đang nhắm**:

| Chặng | Dồn bằng chứng vào |
|---|---|
| S2 | Giấy phép · tiêu chuẩn bệnh viện · bảng giá công khai |
| S3 | Giấy phép · hồ sơ bác sĩ · quy trình mổ · phòng mổ vô khuẩn |
| **S4** | **Số ngày ở lại · quy trình 5 bước · phiên dịch sau khi về · ai liên hệ trong bao lâu** |
| S5 | Bảng giá + phụ phí 10% + cái gì có trong giá + giá cuối do bác sĩ chốt |

**Kênh liên hệ theo market** — gắn đúng kênh, không gắn tất cả:

| Market | Kênh chính |
|---|---|
| AU · US · UK · CA · NZ · EU | **WhatsApp** |
| GCC | WhatsApp |
| KH · LA · MM | WhatsApp · Telegram |
| ID · PH · MY · IN | WhatsApp |
| JP · TW · TH | **Line** |
| KR | **KakaoTalk** |
| **Tầng B (kiều bào)** | **Zalo** + WhatsApp |
| **Tầng D (expat tại VN)** | Zalo + WhatsApp + gọi trực tiếp |

---

## B5 · XUẤT MẪU QUẢNG CÁO

### Google Responsive Search Ad — giới hạn ký tự

| Thành phần | Giới hạn | Số lượng |
|---|---|---|
| Headline | **≤ 30 ký tự** | **15** |
| Description | **≤ 90 ký tự** | **4** |
| Display path | ≤ 15 ký tự / ô | 2 ô |

> ⚠️ **Tiếng Anh đếm ký tự khác tiếng Việt.** 30 ký tự tiếng Anh ngắn hơn cảm giác: `"MOH-Licensed Hospital VN"` = 24. `"Rhinoplasty in Vietnam"` = 22. **Luôn đếm, không ước lượng.**

**15 headline phải phủ đủ 5 nhóm** *(gói nội địa có 4 — nhóm ⑤ là của gói QT)*:

| Nhóm | Số lượng | Ví dụ |
|---|---|---|
| ① Dịch vụ + từ khoá | 4 | `Rhinoplasty in Vietnam` · `Nose Surgery Hanoi` |
| ② USP / bằng chứng | 3 | `MOH-Licensed Hospital` · `Korean-Trained Surgeons` |
| ③ Gỡ nỗi sợ | 3 | `Sterile Operating Theatre` · `Surgeon With 20+ Years` |
| ④ Giá / CTA | 3 | `See Full Price List` · `Book a Consultation` |
| ⑤ ★ **Logistics chuyến đi** | **2** | `Interpreter Included` · `Airport Pickup Provided` |

**Display path:** `/[service]/[market-or-intent]` — vd `/rhinoplasty/vietnam` · `/breast-surgery/price`.

### Meta Ad — 3–5 biến thể mỗi nhóm

| Thành phần | Giới hạn khuyến nghị |
|---|---|
| Primary text | 125 ký tự hiện trước nút *See more* — **đặt hook và bằng chứng mạnh nhất trong 125 ký tự đầu** |
| Headline | **≤ 40 ký tự** |
| Description | **≤ 30 ký tự** |

**Cấu trúc primary text:** hook (dòng 1) → bằng chứng được phép dùng ở market đó → logistics (nếu S4) → CTA + kênh đúng market.

**Gợi ý visual:** mô tả bằng chữ. ⛔ Không chèn ảnh bịa, không mô tả ảnh kết quả không có thật.
⛔ **Tầng C:** gợi ý visual **không được** là before–after hay testimonial kết quả. Visual hợp lệ cho tầng C: cơ sở · phòng mổ · bác sĩ · bộ phận quốc tế · sơ đồ quy trình 5 bước.

**Mỗi mẫu gắn nhãn:**
```
Keyword group | Market | Tier | Stage | Angle A/B/C | Test hypothesis
```

### Mẫu cho tầng B — viết bằng tiếng Việt

Tầng B **không dùng lại mẫu tiếng Anh dịch sang**. Viết mới, giọng nói với người Việt ở xa:
- Nhắc **cửa sổ chuyến đi**: *"Về dịp Tết"* · *"Về hè này"*.
- Nhắc **sắp lịch gọn trong chuyến**: đây là nỗi lo thật của họ, không phải giá.
- ⛔ Không nhắc phiên dịch, không nhắc đưa đón sân bay như bán cho người nước ngoài — họ là người Việt.

---

## B6 · MA TRẬN A/B — đổi đúng 1 biến mỗi lô

| Lô | Biến đổi | Giữ nguyên | Đọc chỉ số |
|---|---|---|---|
| T1 | Hook (3 archetype) | body · offer · visual | CTR |
| T2 | Góc A ↔ B ↔ **C** | hook thắng T1 | CTR + CVR |
| T3 | Bằng chứng (giấy phép / bác sĩ / quy trình) | hook + góc thắng | CVR |
| T4 | **Logistics: có / không nêu số ngày ở lại** ★ | thân thắng | **CVR + tỷ lệ reply** |
| T5 | Kênh CTA (WhatsApp ↔ form ↔ gọi) | copy thắng | **Tỷ lệ kết nối được** |
| T6 | Minh bạch giá: có / không nêu giá trong ad | copy thắng | CTR + chất lượng lead |

★ **Lô T4 là lô có đòn bẩy cao nhất của gói QT** và nên chạy sớm — nó trả lời câu *"nêu số ngày ở lại có làm tăng chuyển đổi không"*, và câu trả lời quyết định cả cấu trúc landing.

Đổi nhiều biến cùng lúc → thắng cũng **không biết nhờ cái gì**.

---

## B7 · CHẤM ĐIỂM WIN — ≥ 12/14 mới được duyệt

Gói nội địa chấm 6 tiêu chí / 12 điểm. Gói QT chấm **7 tiêu chí / 14 điểm** — tiêu chí ⑦ là của gói QT.

| # | Tiêu chí | 0 điểm | 2 điểm |
|---|---|---|---|
| 1 | Hook chạm trong 3 giây | Chung chung | Đúng câu khách tự nói, lấy từ nguồn đúng market |
| 2 | Đúng intent + chặng | Lệch chặng | Khớp đúng nỗi lo của chặng |
| 3 | Bằng chứng thật | Toàn tính từ | Giấy phép · hồ sơ bác sĩ · quy trình cụ thể |
| 4 | Gỡ ≥ 1 rào cản | Không chạm Sợ–Ngờ–Ngại–Xa | Gỡ thẳng rào cản chính của chặng |
| 5 | CTA rõ 1 hành động + **đúng kênh của market** | Mơ hồ, hoặc gắn 5 kênh một lúc | Một hành động, một kênh đúng market |
| 6 | **Tuân thủ:** luật VN + luật market + policy Google/Meta | Có từ cấm (§1 `kn-rao-phap-ly-qt.md`) · dùng testimonial kết quả cho AU · before–after cho tầng C chưa duyệt · hứa số ngày cứng | Sạch, đã rà theo **đúng market** |
| 7 ★ | **Khai đủ `market` + `geo_mode` + tầng** | Thiếu bất kỳ trường nào | Khai đủ, và creative khớp với luật của market đó |

**Tổng < 12/14 → sửa rồi chấm lại. Không xuất mẫu chưa đạt.**

> ⛔ **Tiêu chí 6 hoặc 7 bị 0 điểm = LOẠI THẲNG**, bất kể tổng điểm.
> Năm lỗi tự động cho 0 điểm:
> ① có từ cấm tiếng Anh (`best` · `guaranteed` · `permanent` · `painless` · `lifetime warranty` · `no scars` · `risk-free`);
> ② dùng **testimonial kết quả lâm sàng** hoặc **before–after** cho market AU/UK/EU/GCC chưa qua Pháp chế;
> ③ **hứa số ngày ở lại hoặc mốc hồi phục cứng**;
> ④ **thiếu `market` hoặc `geo_mode`**;
> ⑤ so sánh giá với một quốc gia hoặc cơ sở **có tên**.

---

## §8. THƯ VIỆN HOOK THẮNG — ghi theo market, không ghi chung

Một hook thắng ở Campuchia **không suy ra** thắng ở Úc. Lưu riêng:

```
Service:     Rhinoplasty
Market:      AU  ·  Tier C  ·  geo_mode: Presence+Interest
Stage:       S4 · Trip planning
Archetype:   3 · Logistics cụ thể
Hook:        "[nguyên văn hook thắng]"
Result:      CTR __% (control __%) · CPL __ · reply rate __% · arrival rate __%
Conditions:  [thời gian chạy · ngân sách · nhóm từ khoá · mùa]
Portable to: [market nào dùng lại được — và market nào KHÔNG, vì sao]
```

Dòng `Portable to` là dòng quan trọng nhất và hay bị bỏ. Hook dùng testimonial thắng ở tầng A **không chuyển sang AU được** — không phải vì hiệu quả, mà vì **luật**.


===== kn-ho-so-thuong-hieu-qt.md =====

# HỒ SƠ THƯƠNG HIỆU — KANGNAM QUỐC TẾ *(module swappable)*
Version: 1.0 — 2026-10-21 · đối chiếu trực tiếp với `kangnamaesthetichospital.com`

> Đây là **module thương hiệu** của gói QT. Đổi sang brand khác = thay file này + `kn-rao-phap-ly-qt.md`, giữ nguyên bộ não.
> Khác biệt với `Agent-AdsOptimize-Kangnam` (nội địa): site khác, ngôn ngữ khác, **chỉ 2 cơ sở**, giá **hiện công khai**, và bộ trust **có claim hội–hiệp hội** (xem §4 — điểm xung đột phải xử lý).

---

## §0. NGUỒN DỮ LIỆU — tra tại thời điểm chạy

| Dữ liệu | Nguồn duy nhất | Dùng cho |
|---|---|---|
| Dịch vụ · định vị · trust | `kangnamaesthetichospital.com` (trang chủ + menu) | mọi output |
| **Giá** | `/price-list/` | landing màn Giá · ad có giá |
| Bác sĩ | trang bác sĩ của **site quốc tế** | landing màn Bác sĩ |
| Trang tham chiếu style | `/top-plastic-surgery-in-vietnam/` (bản lưu `template/`) | Design System |
| Số ngày ở lại VN | **chưa có trên site** → Khoa Chuyên môn | mọi landing tầng A/B/C |

**Site mới hơn file này → tin site**, rồi báo người dùng cập nhật file. Bản chụp dưới đây: **2026-10-21**.

---

## §1. ĐỊNH VỊ

Tên quốc tế: **Kangnam Korean Aesthetic Hospital** (viết tắt nội bộ: **KN-QT**).
Định vị site đang dùng: *"Korean Quality, Affordable Price"* — **chất lượng Hàn, chi phí hợp lý**.

**Trục định vị đúng cho thị trường quốc tế:** không bán "rẻ", bán **tỷ lệ chất lượng / chi phí có bằng chứng**.
- Khách tầng C vào trang vì giá, nhưng **chốt vì an toàn**. Trang chỉ nói giá là trang thu hút người săn giá rồi mất họ ở khúc so sánh an toàn.
- Khách tầng A chốt vì **có thật và có phép** — cơ sở bệnh viện có giấy phép Bộ Y tế là bằng chứng mạnh nhất với họ.

⛔ **Hai câu định vị hiện có trên site là superlative và không dùng được trong quảng cáo:**
> *"The Leading Aesthetic Hospital in Vietnam"* · *"Top-Rated Aesthetic Hospital in Vietnam"*

Hai câu này vi phạm luật quảng cáo y tế VN (so sánh tuyệt đối) **và** rủi ro ở AU/UK (claim không có bằng chứng). Dùng trong **tiêu đề SEO của site** là chuyện của SEO; **đưa vào mẫu quảng cáo hoặc headline landing là không được**. Thay bằng câu mô tả kiểm chứng được: *"Licensed aesthetic hospital in Vietnam — Ministry of Health"*.

---

## §2. CƠ SỞ — CHỈ HAI, VÀ CẢ HAI LÀ TUYẾN BỆNH VIỆN

| Cơ sở | Địa chỉ *(nguyên văn site EN)* | Giấy phép | Đại phẫu |
|---|---|---|---|
| **Kangnam Hanoi** | No. 190 Truong Chinh St., Kim Lien Ward, Hanoi, Vietnam | 194/BYT-GPHĐ | ✅ |
| **Kangnam Ho Chi Minh City** | No. 666 Cach Mang Thang 8 St., Tan Son Nhat Ward, Ho Chi Minh City, Vietnam | 287/BYT-GPHĐ | ✅ |

> ✅ **Gói QT không có bẫy TUYẾN của gói nội địa.** Site quốc tế chỉ công bố 2 cơ sở, **cả hai đều là tuyến bệnh viện** → mời đại phẫu là hợp lệ ở cả hai.
> ⛔ **Nhưng không được giới thiệu 5 viện thẩm mỹ tỉnh** (Hải Phòng · Nghệ An · Đà Nẵng · Cần Thơ · Thanh Hoá) cho khách quốc tế: các cơ sở đó **không làm đại phẫu**, và đưa chúng vào nội dung quốc tế tạo ra đúng cái bẫy mà gói này tránh được. Khách quốc tế → **chỉ Hà Nội và TP.HCM**.

**Pháp nhân của site EN:** **Công ty TNHH Bệnh viện Thẩm mỹ Kangnam Sài Gòn** — MST **0312155633**.
Giấy phép hoạt động KCB **287/BYT-GPHĐ**, Bộ Y tế cấp **03/12/2020**.
Tên hiển thị trên site EN: **Kangnam Aesthetic Hospital**. *(Xác nhận 2026-10-21, đối chiếu footer site nội địa.)*

> ⚠️ **Một trang dịch vụ trên site KHÔNG phải là văn bản phạm vi giấy phép.** Rào **R3** đòi hai thứ, và chúng được xác minh bằng hai loại bằng chứng khác nhau:
> ① *pháp nhân nào* — ✅ chốt bằng footer site: Công ty TNHH BVTM Kangnam Sài Gòn.
> ② *dịch vụ có trong phạm vi hoạt động chuyên môn của giấy phép đó không* — chỉ **phụ lục phạm vi của giấy phép** mới trả lời được, không phải trang web.
>
> ⚠️ **Hai cơ sở, hai số giấy phép khác nhau** (194/BYT-GPHĐ Hà Nội · 287/BYT-GPHĐ TP.HCM). Mọi bằng chứng tra được từ footer site nội địa đều thuộc **287 — TP.HCM**. Vì vậy mỗi trang phải ghi **đúng số giấy phép của cơ sở mà trang đó nhắm tới**; ⛔ không dùng chung một số cho cả hai, không chỉ ghi tên thương hiệu rồi bỏ số.

**Liên hệ (nguyên văn site EN):**
- Hotline: **(+84) 981 615 151**
- Giờ làm việc: **Monday to Sunday, 8am – 5pm** *(giờ Việt Nam — UTC+7)*
- Kênh nhắn tin: **WhatsApp · Telegram · Viber · Line · KakaoTalk · Zalo · Messenger**

> ⚠️ **Giờ làm việc 8am–5pm ICT là một rào cản vận hành thật, không phải chi tiết nhỏ.**
> 5pm Việt Nam = 8pm Sydney · 10am London · 6am Los Angeles. Lead tầng C gửi form lúc tối ở nước họ sẽ **không có ai trả lời trong nhiều giờ**.
> → Mọi landing tầng B/C **phải** có ô *preferred contact time + time zone* trong form (xem `kn-khung-landing-qt.md`), và trang thank-you phải nói rõ **khi nào** sẽ được liên hệ theo giờ của khách. Thiếu điều này là nguyên nhân số 1 của lead không kết nối được.

---

## §3. DỊCH VỤ — TAXONOMY QUỐC TẾ

Tên dùng khi viết nội dung hiển thị là **tên quốc tế**, không dịch nguyên văn từ tiếng Việt.

| Nhóm | Dịch vụ (tên EN dùng để viết nội dung & gom từ khoá) |
|---|---|
| **Facial Aesthetic** | Rhinoplasty · Eyelid surgery (double eyelid, canthoplasty, ptosis correction) · Facelift · Neck lift · Forehead lift · Fat grafting |
| **Jaw & Facial Contouring** | V-line surgery · Jaw correction (protrusion / recession) · Zygoma reduction · Chin augmentation · Lip surgery |
| **Body Aesthetic** | Breast augmentation · Breast lift · Liposuction / Lipo 360 · Tummy tuck |
| **ICEFUE Hair Transplant** | Hair transplant |
| **Reconstructive Aesthetic** | Facial paralysis treatment · reconstructive surgery |
| **Dentistry (KDT)** ✅ | Braces · Porcelain crowns · Dental implants · Veneers — **có trong hệ dịch vụ của pháp nhân**, xem ghi chú dưới bảng |
| **Skin & Clinic** | Pigmentation · acne · scar · laser · spa *(⚠️ chỉ bán cho tầng D — xem `kn-thi-truong-quoc-te.md` §3)* |

> ✅ **Nha khoa (2026-10-21):** Kangnam **có chuyên khoa Nha khoa thẩm mỹ**, vận hành dưới chính pháp nhân Công ty TNHH BVTM Kangnam Sài Gòn (giấy phép **287/BYT-GPHĐ**), với 4 dịch vụ: niềng răng · bọc răng sứ · cấy ghép Implant · dán mặt sứ Veneer.
> Nguồn: `benhvienthammykangnam.com.vn/chuyen-khoa/chuyen-khoa-nha-khoa-tham-my/`
> ⚠️ Bằng chứng này thuộc **cơ sở TP.HCM (287)**. **Chưa có bằng chứng cho cơ sở Hà Nội (194)** → landing nha khoa cho khách quốc tế **mặc định trỏ về TP.HCM**, trừ khi Pháp chế xác nhận 194 cũng có RHM trong phạm vi.
> ⚠️ *"Kangnam Dental"* xuất hiện như một nhánh trong hệ sinh thái, nhưng nha khoa **vận hành dưới pháp nhân chính**, không phải một pháp nhân riêng.

**Dịch vụ giá trị lớn** (ưu tiên khi chấm tiêu chí ③ của cổng WIN): breast augmentation · rib-cartilage rhinoplasty · V-line · facelift · Lipo 360 · hair transplant.

---

## §4. ⚠️ TRUST — VÀ ĐIỂM XUNG ĐỘT PHẢI XỬ LÝ TRƯỚC KHI CHẠY

### 4.1 Bằng chứng được phép dùng — theo thứ tự ưu tiên

Dùng **đúng thứ tự này**. Ở thị trường quốc tế, bằng chứng về **giấy phép và quy trình** thắng bằng chứng về **kết quả**, vì kết quả bị chặn bởi luật quảng cáo nhiều thị trường (§5 của `kn-thi-truong-quoc-te.md`).

| # | Bằng chứng | Dùng được ở | Nguyên văn site |
|---|---|---|---|
| ① | **Giấy phép Bộ Y tế Việt Nam** | **Mọi thị trường** | *"MOH Vietnam Licensed"* · 194/BYT-GPHĐ (HN) · 287/BYT-GPHĐ (HCMC) |
| ② | **Hồ sơ bác sĩ** — bằng cấp, trường, số năm | **Mọi thị trường** | xem §5 |
| ③ | **Korean-Trained Surgeons** | Mọi thị trường | *"Korean-Trained Surgeons"* — ⚠️ cần hồ sơ đào tạo kèm theo |
| ④ | **Quy trình an toàn + phòng mổ vô khuẩn + hội đồng chuyên môn** | Mọi thị trường | — |
| ⑤ | **International Patient Department** + phiên dịch | **Mọi thị trường** ★ | *"International Patient Department"* |
| ⑥ | **Quy trình 5 bước cho khách ở xa** (pre-consult → reservation → consult → operation → post-op care) | **Mọi thị trường** ★ | xem §7 |
| ⑦ | **3D Simulation System** | Mọi thị trường | *"3D Simulation System"* |
| ⑧ | **Muslim-Friendly Care** | **GCC · MY · ID ★** | *"Muslim-Friendly Care"* — ⚠️ cần khai rõ gồm những gì |
| ⑨ | **Chính sách bảo hành / chỉnh sửa** | Mọi thị trường — **chỉ khi có văn bản T&C** | xem 4.3 |
| ⑩ | Testimonial · success story · before–after | ⛔ **Giới hạn theo thị trường** — xem `kn-thi-truong-quoc-te.md` §5.2 | — |

★ = **bằng chứng gỡ rào cản XA**, đặc trưng của gói QT, không có ở gói nội địa. Đây là nhóm bằng chứng có đòn bẩy cao nhất và đang bị dùng ít nhất.

### 4.2 🔴 XUNG ĐỘT ① — claim hội–hiệp hội

Site quốc tế **đang hiển thị** các hội: **VSAPS · ASPS · ASAPS · ISAPS · AAFPRS**.
Gói nội địa **cấm thẳng** mọi claim hội–hiệp hội (luật ③ của `Agent-AdsOptimize-Kangnam/knowledge/kn-rao-phap-ly.md`), vì tư cách hội là **của từng cá nhân**, không phải của thương hiệu.

**Hai site đang nói hai điều khác nhau về cùng một đội ngũ.** Đây là rủi ro thật, không phải chuyện câu chữ.

**Luật của gói QT — ba điều kiện, phải đủ cả ba:**
① Gắn với **tên một người cụ thể**, không gắn ở mức thương hiệu / ekip / nhóm quảng cáo.
② Có **hồ sơ thành viên còn hiệu lực** lưu tại Pháp chế cho đúng người đó, đúng hội đó.
③ **Không** trình bày như *board certification* hay như giấy phép hành nghề — đó là hai thứ khác nhau, và nhầm lẫn này là điểm bị chất vấn nhiều nhất ở thị trường US/AU.

→ Thiếu bất kỳ điều kiện nào → **bỏ claim**, thay bằng bằng chứng ① ② ③ ở bảng 4.1.
→ **Việc phải làm ngoài repo:** Pháp chế chốt **một dòng dùng chung cho cả hai site**. Ghi vào `doc/CHANGELOG.md` → *Việc còn treo*.

### 4.3 🔴 XUNG ĐỘT ② — "Lifetime warranty"

Site đang ghi trong khối *Clients Specialized Benefits*: **"Lifetime warranty"**.

Đây là **cam kết mạnh nhất trên toàn site** và cũng là claim rủi ro nhất:
- Không có T&C công bố → là **hứa không kiểm chứng được**, vi phạm nguyên tắc "bằng chứng, không tính từ".
- Ở AU/UK/US, cam kết dạng này cần **điều khoản rõ ràng** về phạm vi, thời hạn, điều kiện loại trừ.
- Với khách tầng C, đây **đồng thời là bằng chứng gỡ rào cản XA mạnh nhất** — nên không thể chỉ bỏ đi, phải **làm cho nó dùng được**.

**Luật:** Agent chỉ được viết về bảo hành khi có **văn bản T&C** nêu đủ:
`phạm vi bảo hành · thời hạn · điều kiện loại trừ · ai chi trả chi phí bay nếu phải chỉnh sửa · xử lý từ xa thế nào`.
→ Chưa có → viết `[PENDING: warranty T&C — Legal]` và **không dùng chữ "lifetime"**. Dùng mô tả trung tính đã có bằng chứng: *"follow-up and warranty policy — see terms"*.

### 4.4 🔴 BA LỖI ĐANG CÓ TRÊN TRANG THAM CHIẾU — đã phát hiện 2026-10-21

Trang `/top-plastic-surgery-in-vietnam/` là **mẫu style** của gói này. Nó **không phải mẫu nội dung**. Ba lỗi dưới đây có trên bản live và **không được sao chép lại**:

| # | Lỗi | Nguyên văn trên trang | Vì sao nghiêm trọng |
|---|---|---|---|
| ① | **Tên bác sĩ của cơ sở khác** trong FAQ | *"**Dr. Granzow** will be able to provide a good estimate for the length of your procedure during your consultation."* | Đây là nội dung FAQ **copy từ website một bác sĩ Mỹ khác**. Không có bác sĩ nào tên Granzow ở Kangnam. Một khách tầng C tra tên này sẽ thấy ngay — mất toàn bộ niềm tin |
| ② | **Bộ đếm hỏng** | *"Trusted by **0+** clients"* | Khối social proof đang hiển thị số 0. Tệ hơn là không có khối nào |
| ③ | **Cam kết kết quả vĩnh viễn** | *"Is rhinoplasty a permanent procedure? **Yes**, … the results are permanent."* | Cam kết kết quả y khoa — vi phạm luật VN, rủi ro FTC/ASA/AHPRA. Phải viết dạng *"long-lasting; ageing or trauma can change nasal structure over time"* |

→ **Luật:** khi đối chiếu trang tham chiếu, Agent lấy **token màu · khung trang · nhịp section · spec form · khối 5 bước cho khách ở xa**. Agent **không lấy**: câu FAQ · con số social proof · câu định vị superlative · claim "lifetime" / "permanent".
→ Báo lại ba lỗi này cho người dùng ở lần đầu mỗi phiên làm việc với trang tham chiếu.

---

## §5. BÁC SĨ — nguồn: site quốc tế

Bản chụp từ `/top-plastic-surgery-in-vietnam/` ngày **2026-10-21**. Nguyên văn credential:

| Bác sĩ | Chức danh *(nguyên văn)* | Bằng cấp | Kinh nghiệm | Cơ sở |
|---|---|---|---|---|
| **Dr. PhD Richard Huy** | Medical Director of Kangnam Aesthetic Hospital – Hanoi | Doctor of Medicine (PhD) – Hanoi Medical University | Over 20 years in Aesthetic Surgery | Hanoi |
| **Dr. Felix Tran** | Medical Director of Kangnam Aesthetic Hospital – Ho Chi Minh City | Doctor of Medicine (M.D.) – Thai Nguyen University of Medicine and Pharmacy | Over 20 years in Aesthetic Surgery | HCMC |
| **Dr. Frankie Vu** | Deputy Head of the Facial Plastic and Aesthetic Surgery – HCMC | Doctor of Medicine (M.D.) – Military Medical Academy, Hanoi | Over 10 years in Aesthetic Surgery | HCMC |
| **Dr. Victor Vu** | Head of the Maxillofacial Surgery Department – Hanoi | Specialist Level I in Oral and Maxillofacial Surgery | Nearly 20 years in Oral and Maxillofacial Surgery | Hanoi |
| **Dr. Henry Nguyen** | Head of the Facial Plastic and Aesthetic Surgery Department – Hanoi | Specialist Level I in General Surgery – Hanoi Medical University | Over 12 years in aesthetics surgery | Hanoi |

### Bốn cổng trước khi gắn tên bác sĩ vào bất kỳ nội dung nào

① **Có trên site quốc tế** không — site nội địa và site quốc tế **không trùng danh sách**, và trang hồ sơ còn sống **không** đồng nghĩa được dùng.
② **Đúng chuyên khoa VÀ đúng cơ sở** của nội dung — bác sĩ HCMC không gắn vào landing Hanoi.
③ **Có số CCHN** — site quốc tế **không công bố số CCHN**, chỉ công bố bằng cấp. → Cần lấy từ hồ sơ nội bộ. Chưa có → **không nêu claim tay nghề ở mức cá nhân**.
④ **Có trong danh sách nội bộ "được duyệt quảng bá"** — cổng quyết định, do Pháp chế giữ.

> ⚠️ **Hai danh sách lệch nhau.** Site nội địa có 16 bác sĩ; site quốc tế công bố 5 trên trang tham chiếu. Nhân sự có mặt ở site nội địa **không tự động** dùng được cho nội dung quốc tế, và ngược lại. Lệch → **dừng, hỏi Pháp chế**, không tự chọn bên.
> Số năm kinh nghiệm: chép **đúng** chữ trên site (*"Over 20 years"*, *"Nearly 20 years"*). ⛔ Không làm tròn lên, không đổi "nearly 20" thành "20+".

---

## §6. GIÁ — bản chụp `/price-list/` 2026-10-21

> ⚠️ **Bản chụp để đối chiếu, KHÔNG để đăng.** Lấy lại tại `/price-list/` ở thời điểm chạy. Quy tắc hiện giá: `kn-thi-truong-quoc-te.md` §7.

| Nhóm | Dịch vụ | VND | ≈ USD *(site tự quy đổi)* |
|---|---|---|---|
| **Eyelid** | 6D Eyelid Surgery | 12.000.000 | 461 |
| | VIP Eyelid Surgery | 20.800.000 | 800 |
| | Fat Removal | 5.600.000 | 215 |
| | Comprehensive Package | 18.400.000 | 707 |
| **Rhinoplasty** | Idol Structure (Nanoform) | 35.200.000 | 1.353 |
| | Surgiform Technique | 48.000.000 | 1.846 |
| | 6D VIP | 56.800.000 | 2.184 |
| | Rib Cartilage (100%) | 88.200.000 | 3.392 |
| **Facial Rejuvenation** | Facelift | 51.200.000 | 1.969 |
| | Facelift + Neck Lift | 71.200.000 | 2.738 |
| | Forehead Lift | 40.000.000 | 1.538 |
| **Jaw & Contouring** | Chin Augmentation | 24.000.000 | 923 |
| | V-line 3D | 54.400.000 | 2.092 |
| | Zygoma Reduction | 54.400.000 | 2.092 |
| **Liposuction** | Advanced Lipo | 40.500.000 – 65.800.000 | 1.557 – 2.530 |
| | Mini Lipo (1 vùng) | 18.000.000 | 692 |
| **Breast** | 6D Basic | 67.000.000 | 2.576 |
| | 6D VIP | 84.000.000 | 3.230 |

**Ba dòng bắt buộc đi kèm mọi bảng giá** *(nguyên văn site)*:
- *"The price shown does not include 10% international service charge."*
- *"USD figures are approximate conversions, for reference only; they will change depending on exchange rates on payment day."*
- *"Final costs will be confirmed by the doctor after examination."*

**Gói giá bao gồm** *(nguyên văn site)*: consultation · comprehensive health screening · pre-operative assessment · standard medical techniques · professional post-operative care · follow-up appointments · long-term warranty policy *(⚠️ xem §4.3 về chữ "warranty")*.

---

## §7. QUY TRÌNH 5 BƯỚC CHO KHÁCH Ở XA — *"Out of Town Patients"*

Khối này là **bằng chứng gỡ rào cản XA** và là tài sản mạnh nhất của gói QT. Nguyên văn site:

| Bước | Tên | Nội dung *(nguyên văn)* |
|---|---|---|
| **1** | Pre-Consultation | *"Recommendable surgery, estimated cost, and the detailed information regarding surgery will be provided based on the pictures"* |
| **2** | Reservation | *"Schedule a date on the desired date. Hotel recommendation and Airport pick up will be provided"* |
| **3** | Consultation in Person | *"Meet the specialized surgeon for each surgery area and get more accurate surgery plan"* |
| **4** | Operation | *"Safety is our priority"* |
| **5** | Post Operative Care | *"Communicating with the interpreter will be continued after departure"* |

**Ba chỗ khối này đang yếu — vá được ngay và có đòn bẩy cao:**
① **Bước 2 không nói số ngày phải ở lại** → khách không đặt được vé (xem `kn-thi-truong-quoc-te.md` §8).
② **Bước 4 chỉ có một câu** *"Safety is our priority"* — đây là **tính từ**, đúng chỗ cần bằng chứng nhất. Thay bằng: ai mổ · ở đâu · phòng mổ gì · theo dõi hậu phẫu bao lâu · ai trực.
③ **Bước 5 không nói thời hạn và kênh** → *"continued after departure"* trong bao lâu, qua kênh nào, ai là người liên hệ. Đây đúng là câu khách tầng C muốn biết nhất.

→ Khi dựng landing, Agent **phải** đề xuất vá ba chỗ này, và để `[PENDING]` nếu chưa có dữ liệu.

---

## §8. DỊCH VỤ HỖ TRỢ KHÁCH QUỐC TẾ — kiểm kê

| Hạng mục | Trạng thái trên site | Cần khai thêm |
|---|---|---|
| International Patient Department | ✅ có nêu | Giờ trực · ngôn ngữ · kênh |
| Phiên dịch | ✅ có nêu (trong/sau điều trị) | Ngôn ngữ nào · có tính phí không |
| Đưa đón sân bay | ✅ có nêu | Miễn phí hay tính phí |
| Gợi ý khách sạn | ✅ có nêu | Có giá đối tác không |
| Ngôn ngữ site | English · Vietnamese · **Khmer** | Arabic cho GCC — chưa có |
| Kênh nhắn tin | WhatsApp · Telegram · Viber · Line · KakaoTalk · Zalo · Messenger | Thời gian phản hồi cam kết |
| Muslim-Friendly Care | ✅ có nêu | **Gồm những gì** — chưa khai. Claim này vô nghĩa nếu không nêu cụ thể (đồ ăn halal? nhân viên nữ? phòng cầu nguyện?) |
| Visa / thư mời | ❌ **không thấy trên site** | Có hỗ trợ không — câu hỏi thường gặp của tầng A |
| Thanh toán quốc tế | ❌ **không thấy trên site** | Thẻ quốc tế? chuyển khoản? đặt cọc bao nhiêu? — **rào cản chốt thật** |

→ Bốn dòng `❌` và các ô "cần khai thêm" là **danh sách đặt hàng dữ liệu**. Agent liệt kê chúng ở cuối mỗi output có liên quan, không tự điền.

---

## §9. GIỌNG — thị trường quốc tế

**Register:** y khoa cao cấp, điềm tĩnh, nhiều số liệu, ít cảm xúc. Gần với một bệnh viện quốc tế hơn là một thẩm mỹ viện.

| Nên | Không nên |
|---|---|
| *"Licensed by the Vietnamese Ministry of Health. Licence No. 287/BYT-GPHĐ."* | *"The leading hospital in Vietnam"* |
| *"Over 20 years in aesthetic surgery — Hanoi Medical University."* | *"World-class surgeons"* |
| *"Interpreter support continues after you fly home."* | *"We care about you like family"* |
| *"Published price list. 10% international service charge applies."* | *"Unbeatable prices"* |

⛔ **Không dùng giọng "khoe"** (xem `kn-thi-truong-quoc-te.md` §6). ⛔ Không emoji trong ad và landing tầng C.

---

## §10. RANH GIỚI

- **Nha khoa (KDT)** thuộc sub-brand Kangnam Dental — nằm trong hệ sinh thái nên **được cross-sell**, nhưng rào cản chốt khác (NGỜ về vật liệu nặng nhất). Gợi ý được, **không dựng bộ từ khoá hay landing nha khoa bằng bộ não này**.
- **Cơ xương khớp / bảo tồn khớp** là thương hiệu riêng, có agent riêng (CXK-CPW) — không viết bằng giọng thẩm mỹ.
- **Nội dung tiếng Việt cho khách trong nước** thuộc gói nội địa [`Agent-AdsOptimize-Kangnam`](../../Agent-AdsOptimize-Kangnam/) — site khác, giá ẩn, 7 cơ sở, có bẫy TUYẾN. **Không trộn hai gói.**
  → Ngoại lệ duy nhất: **tầng B (kiều bào)** viết bằng tiếng Việt nhưng **thuộc gói QT**, vì rào cản là XA và cơ sở chỉ có 2.


===== kn-khung-landing-qt.md =====

# KHUNG LANDING QUỐC TẾ & DESIGN SYSTEM KANGNAM INTERNATIONAL v1.0
Version: 1.0 — 2026-10-21 · token lấy từ trang production `/top-plastic-surgery-in-vietnam/`

---

## §1. CHỌN KHUNG — THEO CHẶNG × TẦNG, KHÔNG THEO NGUỒN TRAFFIC

Gói nội địa chọn khung theo **nguồn traffic** (Ads → AIDA · SEO → PAS). Gói QT chọn theo **chặng phễu × tầng thị trường**, vì khách quốc tế vào phễu ở **chặng khác nhau**: tầng C vào ở S2 (*"nước nào"*), tầng D vào ở S5 (*"đặt lịch tuần này"*).

| Khung | Dùng cho | Hero trả lời câu gì | Rào cản gỡ |
|---|---|---|---|
| **L1 · DESTINATION** | **S2** · tầng A · C | *"Tại sao là Việt Nam?"* — ⛔ **chưa bán Kangnam** | NGỜ |
| **L2 · ANSWER-FIRST** | **S3** · mọi tầng | Gọi đúng nỗi lo rồi **trả lời ngay** | **SỢ** |
| **L3 · TRIP-PLAN ★** | **S4** · tầng A · B · C | *"Chuyến đi này chạy được không?"* | **XA ★** |
| **L4 · PRICE & BOOK** | **S5** · mọi tầng | *"Bao nhiêu, và đặt lịch thế nào?"* | NGẠI (chi phí) |
| **L5 · EXPAT** | tầng **D** | *"Có bác sĩ nói tiếng Anh, tuần này đặt được không?"* | NGỜ (giao tiếp) |
| **L6 · DIASPORA** | tầng **B** · tiếng Việt | *"Về nhà dịp này, sắp lịch gọn trong chuyến được không?"* | XA + NGẠI |

### 1.1 Ba luật chọn khung

**① ⛔ Không dùng L4 (giá) cho từ khoá S2.** Người đang hỏi *"nước nào"* chưa sẵn sàng xem bảng giá của một bệnh viện họ chưa tin. Đây là nguyên nhân phổ biến nhất của **CTR tốt + bounce cao** ở tầng C.

**② ⛔ Không dùng L3 (trip-plan) cho tầng D.** Expat đang sống ở Hà Nội — khối đưa đón sân bay và khách sạn là vô nghĩa, và làm trang trông như không hiểu họ là ai.

**③ ⛔ Không khoét sâu nỗi sợ ở L2.** Hai lý do, lý do sau nặng hơn: ① click đã trả tiền và từ khoá đã khai intent → trì hoãn câu trả lời làm tăng bounce; ② quảng cáo dịch vụ KCB **không được gây hoang mang**, và với khách sắp bay nửa vòng trái đất thì khoét sâu biến chứng là **rủi ro tuân thủ**, không chỉ là copy dở. Gọi tên nỗi lo rồi **trả lời ngay** — đó là tất cả.

---

## §2. THƯ VIỆN 14 KHỐI — dùng lại, không dựng khối mới

| # | Khối | Trả lời câu hỏi nào | Ghi chú bắt buộc |
|---|---|---|---|
| **B01** | **Hero** | *"Có đúng thứ tôi tìm không?"* | Message-match với ad trong **3 giây** · 2–3 badge trust · 1 CTA chính |
| **B02** | **Credential bar** | *"Nơi này có thật, có phép không?"* | Giấy phép Bộ Y tế + số · Korean-Trained · 3D Simulation · International Patient Dept · *(GCC: Muslim-Friendly)* |
| **B03** | **Why Vietnam** | *"Tại sao không làm ở nước tôi hoặc ở Hàn/Thái?"* | ⛔ **Không hạ thấp nước khác.** Nêu tiêu chí khách quan, để khách tự so |
| **B04** | **The worry, answered** | *"[Nỗi lo] thì sao?"* | Gọi tên → **trả lời ngay** → bằng chứng. ⛔ Không khoét sâu |
| **B05** | **Procedure & technique** | *"Làm bằng cách nào? Khác gì?"* | Chỉ nêu kỹ thuật/thiết bị cơ sở **thực sự có** |
| **B06** | **Your surgeon** | *"Ai mổ cho tôi?"* | Ảnh thật · bằng cấp · trường · số năm **chép đúng site** · qua đủ 4 cổng bác sĩ |
| **B07** | **Safety protocol** | *"Có an toàn không?"* | Phòng mổ vô khuẩn · hội đồng chuyên môn · gây mê do bác sĩ chỉ định · theo dõi hậu phẫu. ⛔ **Không viết "Safety is our priority"** — đó là tính từ |
| **B08** ★ | **Your trip, step by step** | *"Chuyến đi diễn ra thế nào?"* | Quy trình 5 bước + **số ngày ở lại** + phiên dịch + đưa đón + khách sạn |
| **B09** ★ | **After you fly home** | *"Về nhà rồi ai lo cho tôi?"* | Ai liên hệ · kênh · ngôn ngữ · **trong bao lâu** · lịch tái khám từ xa · T&C bảo hành |
| **B10** | **Price & what's included** | *"Bao nhiêu? Có đáng không?"* | Bảng giá + **3 dòng bắt buộc** (§6) + gồm gì / không gồm gì |
| **B11** | **Proof** | *"Người giống tôi ra sao?"* | ⚠️ **Theo market** — tầng C mặc định **không** dùng testimonial kết quả / before–after |
| **B12** | **FAQ** | *"Tôi còn lo gì?"* | 6–8 câu, **ưu tiên câu logistics**. ⛔ Không copy FAQ từ site khác |
| **B13** | **Consultation form** | *"Giờ làm gì?"* | Spec §7 — có `timezone` + `preferred contact time` |
| **B14** | **Footer** | — | Logo · **số giấy phép đúng cơ sở** · 2 địa chỉ · hotline · giờ làm việc **kèm múi giờ** · disclaimer *"Results vary by individual"* |

★ = khối riêng của gói QT. **B08 và B09 là hai khối có đòn bẩy cao nhất** và đang bị làm sơ sài nhất trên trang production.

---

## §3. BẢN ĐỒ KHUNG → THỨ TỰ KHỐI

| Khung | Thứ tự khối |
|---|---|
| **L1 · DESTINATION** | B01 → B02 → **B03** → B07 → B06 → **B08** → B10 → B12 → B13 → B14 |
| **L2 · ANSWER-FIRST** | B01 → **B04** → B02 → B07 → B06 → B09 → B05 → B11 → B12 → B13 → B14 |
| **L3 · TRIP-PLAN ★** | B01 → B02 → **B08** → **B09** → B06 → B07 → B10 → B12 → B13 → B14 |
| **L4 · PRICE & BOOK** | B01 → B02 → **B10** → B06 → B07 → B08 → B09 → B11 → B12 → B13 → B14 |
| **L5 · EXPAT** | B01 → B02 → B06 → B05 → B07 → B10 → B11 → B12 → B13 → B14 — ⛔ **không B08, không B09** |
| **L6 · DIASPORA** *(tiếng Việt)* | B01 → B02 → **B08 rút gọn** (lịch trình trong chuyến về) → B06 → B07 → B10 → B09 → B12 → B13 → B14 |

**Độ dài theo nhiệt độ:**
- **Tầng D / S5 (nóng)** → ngắn: B01 → B02 → B06 → B10 → B13.
- **Tầng C / S2 (lạnh)** → đủ khối, thêm nội dung giáo dục ở B03.
- **Tầng B** → trung bình, dồn vào cửa sổ chuyến đi.

---

## §4. MICRO-CONVERSION — hạ rào cản trước khi xin số

Khách quốc tế càng không sẵn sàng để lại số cho một ca đại phẫu ở nước khác. **Đặt một bước trung gian trước form.**

| Micro-conversion | Dùng cho chặng | Rào cản hạ |
|---|---|---|
| **Nhận bảng giá đầy đủ qua email** | S2 · S5 | NGỜ (minh bạch) |
| **Tải cẩm nang chuyến đi** — số ngày · chuẩn bị · giấy tờ | **S4 ★** | **XA** |
| **Gửi ảnh nhận đánh giá sơ bộ** *(bác sĩ thực hiện, không phải Agent)* | S3 · S4 | SỢ |
| **Chat WhatsApp với bộ phận quốc tế** | mọi chặng | XA |
| **Chọn dịch vụ quan tâm** — bottom sheet | mọi chặng, trong form | — |

**Vị trí:** ngay **trước** B13 (form), hoặc sau B09.
⛔ Không bắt điền số ngay ở hero cho ca đại phẫu — hero chỉ cần CTA cuộn xuống hoặc nút WhatsApp.

> **Trục riêng tư.** Rào cản NGẠI ở gói QT có hai trục: *"không muốn người thân biết"* **và** *"không muốn đồng nghiệp ở nước tôi biết"* (rõ nhất ở QT3 hair transplant và QT5 GCC). Mọi landing phải có **kênh nhắn tin riêng tư song song form** và dòng cam kết bảo mật dưới nút submit.

---

## §5. DESIGN SYSTEM KANGNAM INTERNATIONAL v1.0

**Nguồn token:** trang production `https://kangnamaesthetichospital.com/top-plastic-surgery-in-vietnam/`
(bản lưu: `template/lp-reference-top-plastic-surgery.html` + `template/lp-reference-style.css`).

> ⚠️ **Trang mẫu dùng để lấy gì — và KHÔNG lấy gì.**
> ✅ Lấy: **token màu** · nhịp section · spec form quốc tế · **khối 5 bước cho khách ở xa**.
> ❌ **Không lấy nội dung:** câu FAQ (có tên bác sĩ của cơ sở khác) · con số social proof (`0+`) · câu định vị superlative · claim `lifetime` / `permanent`. Chi tiết 3 lỗi: `kn-ho-so-thuong-hieu-qt.md` §4.4.

### 5.1 Token màu

```css
:root{
  /* ---- primary: lấy từ production --primary-color / --second-color ---- */
  --teal:#005F88;        --teal-900:#00394F;      --teal-400:#00BAC3;
  --navy:#003C77;        /* navy nhận diện thương hiệu */

  /* ---- luxury accent: gold ---- */
  --gold:#B08D4F;        --gold-dk:#8C6E36;       --gold-lt:#C9A86A;
  --gold-wash:#F3EADA;

  /* ---- action ---- */
  --cta:#E15A01;         --cta-press:#C44D00;

  /* ---- surface: trắng + champagne ấm = register sang trọng ---- */
  --bg:#FFFFFF;          --surface:#FFFFFF;
  --champagne:#FAF7F2;   /* khối ấm, xen giữa các khối trắng */
  --surface-alt:#F7F9FA; /* khối mát */

  /* ---- ink & line ---- */
  --ink:#14212B;         --ink-2:#4A5C6A;         --ink-3:#7A8B98;
  --line:#E3E8EC;        --line-gold:#E0D2B6;

  /* ---- trạng thái ---- */
  --ok:#147D56;          --err:#B3261E;           --err-t:#FDECEA;

  /* ---- hình khối ---- */
  --r-sm:6px;  --r:10px;  --r-lg:16px;  --r-pill:999px;
  --sh:0 1px 2px rgba(20,33,43,.04), 0 8px 24px rgba(20,33,43,.06);
  --sh-lg:0 2px 4px rgba(20,33,43,.05), 0 24px 48px rgba(20,33,43,.10);

  /* ---- nhịp: thang 8px ---- */
  --s1:8px; --s2:16px; --s3:24px; --s4:32px; --s5:48px; --s6:64px; --s7:96px;
  --maxw:1140px;  --maxw-text:68ch;  --hdr-h:72px;
}
```

### 5.2 ⚠️ BẢY RÀO TƯƠNG PHẢN — đã đo, không phải ước lượng

| Luật | Số đo |
|---|---|
| ✅ `--teal` **an toàn ở mọi cỡ**, cả chữ trên trắng và trắng trên nền teal | **7,02:1 AA/AAA** cả hai chiều |
| ✅ `--teal-900` cho heading lớn và khối tối | 12,37 AAA trên trắng |
| ✅ `--navy` an toàn mọi cỡ | 10,98 AAA trên trắng |
| ⛔ **`--teal-400` KHÔNG làm chữ trên trắng** | **2,38:1 — fail.** Chỉ dùng làm vạch, viền, icon trang trí |
| ⛔ **`--gold` KHÔNG làm chữ nhỏ trên trắng** | **3,10:1** → chỉ đạt ngưỡng large-text: **≥ 24px thường hoặc ≥ 19px/700**. Chữ gold nhỏ hơn → dùng **`--gold-dk` (4,77 AA)** |
| ⛔ **`--cta` là màu NỀN NÚT, không phải màu chữ** | Trắng trên `--cta` = **3,71:1** → nhãn nút phải **≥ 19px/700**. Nút nhỏ hơn → dùng **`--cta-press` (4,76 AA)** hoặc `--teal` |
| ⛔ **`--ink-3` KHÔNG dùng cho chữ thân** | **3,52:1 — fail.** Chữ phụ dùng `--ink-2` (**6,93 AA**) |

**Gold trên nền tối — dùng được:** `--gold-lt` trên `--teal-900` = **5,47 AA** · `#FEC465` trên `--teal-900` = **7,83 AAA**.
**Trên `--champagne`:** `--ink` 15,33 · `--ink-2` 6,49 · `--teal` 6,57 · `--navy` 10,27 — tất cả an toàn.

### 5.3 Tỷ lệ màu — luật "sạch & sang"

```
78%  trắng / champagne / surface-alt     ← khoảng trắng là vật liệu chính
15%  teal + teal-900                      ← nền tin cậy, khối tối có chủ ý
 5%  gold                                 ← chỉ eyebrow, vạch, số thứ tự, viền
 2%  cta cam                              ← CHỈ hành động
```

⛔ **Không nền tối toàn trang.** ⛔ Không quá 3 màu chính. ⛔ Không gradient/neon. ⛔ Không nhiều style icon lẫn lộn. ⛔ Không chồng shadow.

> **"Sang trọng" ở đây đến từ ba thứ, không đến từ màu:** ① **khoảng trắng lớn** (section padding 96px desktop) · ② **serif hiển thị ở cỡ lớn** · ③ **gold dùng rất ít, chỉ ở vạch mảnh và eyebrow**. Dùng nhiều gold làm trang trông rẻ đi, không sang hơn.

### 5.4 Typography — hai font

| Vai trò | Font | Weight | Cỡ |
|---|---|---|---|
| **Display** — h1 · h2 · số lớn · câu nhấn | **Cormorant Garamond** | 600 | **≥ 28px** — không bao giờ nhỏ hơn |
| **Body · UI · nút · form · h3 · bảng** | **Inter** | 400 · 500 · 600 · 700 | body 17px/1.65 · input **16px** |

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@600&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

```css
--f:'Inter',system-ui,-apple-system,'Segoe UI',Roboto,Arial,sans-serif;
--f-d:'Cormorant Garamond','Georgia','Times New Roman',serif;
```

**Thang chữ** *(desktop → mobile)*:
`h1` 56→34px · `h2` 40→27px · `h3` 21→19px (Inter 600) · body 17→16px · caption 14px (`--ink-2`) · eyebrow 13px/600 letter-spacing `.14em` uppercase (`--gold-dk`).

**Luật:**
- Cormorant Garamond là serif **tương phản cao, nét mảnh** — dưới 28px nó mỏng và khó đọc. **Không dùng cho body, không dùng cho nút, không dùng cho form.**
- Body **17px** là cố ý: nhiều khách đọc tiếng Anh như ngôn ngữ thứ hai, và tầng B/C có độ tuổi cao hơn.
- **Input bắt buộc 16px** — nhỏ hơn thì iOS tự zoom khi chạm.
- Đoạn văn giới hạn **`--maxw-text` 68ch**. Dòng dài hơn là lỗi đọc, không phải lỗi thẩm mỹ.
- **Không nạp font thứ ba.** Cần nhấn thì đổi weight.

> ⚠️ **Lệch với production.** Trang production đang chạy **Roboto** cho toàn bộ. Cặp Cormorant + Inter là **register quốc tế của gói này** (yêu cầu "sạch, sang trọng"), và là **thay đổi cần brand chốt một lần** — ghi vào `doc/CHANGELOG.md` → *Việc còn treo*. Chưa chốt thì dùng Inter cho cả display (weight 600, letter-spacing `-.02em`) và **nói rõ với người dùng** đang dùng bản dự phòng.

### 5.5 Khung trang — **responsive full-width, không phải thẻ 480px**

Đây là khác biệt cấu trúc lớn nhất so với gói nội địa. Gói nội địa dựng thẻ khổ điện thoại `max-width:480px` căn giữa. **Gói QT không dùng kiểu đó**, vì:
- Khách tầng C **nghiên cứu trên desktop** (so giá, đọc hồ sơ bác sĩ, mở nhiều tab) rồi mới chuyển sang mobile để nhắn tin.
- Bảng giá và bảng so sánh điểm đến **cần chiều ngang**.
- Một thẻ 480px trên màn 1440px đọc như một trang quảng cáo địa phương, không như một bệnh viện quốc tế.

```css
*{box-sizing:border-box}
html{scroll-behavior:smooth;-webkit-text-size-adjust:100%}
body{margin:0;font:400 17px/1.65 var(--f);color:var(--ink);background:var(--bg)}
img{max-width:100%;display:block}
:focus-visible{outline:3px solid var(--gold);outline-offset:2px;border-radius:4px}
@media (prefers-reduced-motion:reduce){
  html{scroll-behavior:auto} *{transition:none!important;animation:none!important}}

/* container */
.wrap{max-width:var(--maxw);margin-inline:auto;padding-inline:var(--s3)}
@media (max-width:640px){.wrap{padding-inline:var(--s2)}}   /* gutter 16px mobile */
section{padding-block:var(--s7)}
@media (max-width:860px){section{padding-block:var(--s5)}}
.band-warm{background:var(--champagne)}
.band-cool{background:var(--surface-alt)}
.band-dark{background:var(--teal-900);color:#fff}

/* header: sticky, nền mờ, logo + 1 CTA */
.hdr{position:sticky;top:0;z-index:60;min-height:var(--hdr-h);
  display:flex;align-items:center;gap:var(--s3);
  padding:12px clamp(16px,4vw,40px);
  background:rgba(255,255,255,.92);backdrop-filter:blur(12px);
  -webkit-backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.hdr__nav{display:flex;gap:var(--s3);margin-inline-start:auto;font-size:15px;font-weight:500}
.hdr__nav a{color:var(--ink-2);text-decoration:none}
.hdr__nav a:hover{color:var(--teal)}
@media (max-width:860px){.hdr__nav{display:none}}

/* tiêu đề section: eyebrow gold + display serif + vạch gold mảnh */
.sec-head{max-width:var(--maxw-text);margin-bottom:var(--s5)}
.sec-head--center{margin-inline:auto;text-align:center}
.sec-head .eyebrow{display:block;font:600 13px/1.4 var(--f);letter-spacing:.14em;
  text-transform:uppercase;color:var(--gold-dk)}          /* gold-dk: 4,77 AA */
.sec-head h2{margin:10px 0 0;font:600 clamp(27px,3.4vw,40px)/1.18 var(--f-d);
  color:var(--teal-900);letter-spacing:-.01em}
.sec-head .rule{display:block;width:56px;height:1px;background:var(--line-gold);
  margin-top:var(--s3)}
.sec-head--center .rule{margin-inline:auto}

/* nút */
.btn{display:inline-flex;align-items:center;justify-content:center;gap:10px;
  min-height:54px;padding:14px 34px;border:0;border-radius:var(--r-pill);
  font-family:var(--f);text-decoration:none;cursor:pointer;
  transition:background-color .16s,transform .12s}
.btn-cta{background:var(--cta);color:#fff;font-size:19px;font-weight:700}  /* 19/700 = ngưỡng */
.btn-cta:hover{background:var(--cta-press)}
.btn-cta:active{transform:translateY(1px)}
.btn-ghost{background:transparent;color:var(--teal);font-size:16px;font-weight:600;
  box-shadow:inset 0 0 0 1.5px var(--teal);min-height:48px}
.btn-wa{background:#fff;color:var(--teal-900);font-size:16px;font-weight:600;
  box-shadow:inset 0 0 0 1.5px var(--line)}
@media (max-width:640px){.btn{width:100%}}

/* card */
.card{background:var(--surface);border:1px solid var(--line);
  border-radius:var(--r-lg);padding:var(--s4);box-shadow:var(--sh)}
.card--gold{border-color:var(--line-gold)}
.grid{display:grid;gap:var(--s3)}
.grid-2{grid-template-columns:repeat(2,1fr)}
.grid-3{grid-template-columns:repeat(3,1fr)}
.grid-4{grid-template-columns:repeat(4,1fr)}
@media (max-width:980px){.grid-3,.grid-4{grid-template-columns:repeat(2,1fr)}}
@media (max-width:640px){.grid-2,.grid-3,.grid-4{grid-template-columns:1fr}}

/* số thứ tự gold — dùng cho B08 quy trình 5 bước */
.step__n{font:600 40px/1 var(--f-d);color:var(--gold);     /* 40px > 24px: đạt ngưỡng */
  border-bottom:1px solid var(--line-gold);padding-bottom:10px;margin-bottom:14px}

/* sticky action bar — mobile */
.sticky{position:fixed;inset-inline:0;bottom:0;z-index:70;display:none;gap:8px;
  padding:10px 12px calc(10px + env(safe-area-inset-bottom,0px));
  background:rgba(255,255,255,.96);backdrop-filter:blur(12px);
  border-top:1px solid var(--line)}
@media (max-width:860px){.sticky{display:flex}}
.sticky .btn{min-height:48px;padding:12px 16px;font-size:15px;flex:1}
```

### 5.6 Nhịp khối — luật "sạch"

- Xen khối: `trắng → champagne → trắng → surface-alt → trắng`. **Tối đa một `band-dark` trên toàn trang** (thường là B09 hoặc B02).
- Section padding **96px** desktop / **48px** mobile. Đây là nguồn chính của cảm giác "sang" — cắt padding là cắt đúng thứ đang mua.
- Mỗi khối **1 ý chính + 1 điểm nhìn chính**.
- CTA lặp lại sau mỗi **2–3 khối** + sticky bar mobile.
- ⛔ Không popup chặn màn đầu. ⛔ Không autoplay video có tiếng. ⛔ Không đếm ngược tự reset.

### 5.7 Ô ảnh tạm — bắt buộc khi chưa có ảnh thật

⛔ **Không bao giờ** chèn ảnh stock, ảnh AI, hay `<img>` trỏ tới URL không tồn tại.

```css
.ph{display:grid;place-content:center;gap:6px;text-align:center;margin:0;padding:20px;
    aspect-ratio:var(--ar,16/9);background:var(--surface-alt);
    border:1px dashed var(--line-gold);border-radius:var(--r-lg);
    color:var(--ink-2);font-size:14px;line-height:1.5}
.ph b{display:block;font-weight:600;color:var(--teal-900)}
```

```html
<figure class="ph" style="--ar:3/4">
  <b>Photo 3:4</b>
  Dr. [name] portrait, Hanoi hospital · needs: real photo, 4 doctor gates passed, Legal approval
</figure>
```

| Vị trí | `--ar` | Ghi chú |
|---|---|---|
| Hero | `16/9` desktop · `4/5` mobile | Ảnh **duy nhất** không lazy-load · `fetchpriority="high"` |
| Chân dung bác sĩ | `3/4` | Chỉ bác sĩ qua đủ 4 cổng |
| Cơ sở · phòng mổ · thiết bị · bộ phận quốc tế | `16/9` | Ảnh thật của hệ thống — **nhóm ảnh dùng được ở mọi market** |
| Before–after | `1/1` | ⚠️ **Theo market** — tầng C mặc định không dùng |
| Icon | `1/1` | 24px, **một bộ icon duy nhất**, stroke 1.5px |

**Cuối mỗi landing bắt buộc kèm BẢNG KÊ ẢNH CẦN CẤP** — vị trí · tỉ lệ · nội dung cần · **đồng ý có phạm vi quốc tế hay không** · ai duyệt. Thiếu bảng này thì trang **chưa giao xong**.

> ⚠️ Cột *"đồng ý có phạm vi quốc tế hay không"* là cột riêng của gói QT: một văn bản đồng ý cho phép dùng ảnh ở Việt Nam **không tự động** cho phép dùng ở Úc hay EU.

---

## §6. KHỐI GIÁ (B10) — ba dòng bắt buộc

Mọi bảng giá **phải** kèm đủ ba dòng, nguyên văn:

```
The price shown does not include 10% international service charge.
USD figures are approximate and depend on the exchange rate on the day of payment.
Final cost is confirmed by the doctor after in-person examination.
```

Và **hai cột** *(cái gì có trong giá / cái gì không)*:

| ✅ Included | ❌ Not included |
|---|---|
| Consultation · health screening · pre-operative assessment · post-operative care · follow-up appointments · warranty policy *(⚠️ chỉ ghi khi có T&C — xem `kn-rao-phap-ly-qt.md` §4 luật ④)* | Flights · hotel · **10% international service charge** · *(phiên dịch — nếu tính phí riêng)* |

⛔ **Không so sánh giá với quốc gia/cơ sở có tên.** Công bố bảng giá đầy đủ và để khách tự so.

---

## §7. FORM QUỐC TẾ (B13) — SPEC

Form nội địa 3 trường. **Form quốc tế không thể 3 trường** — thiếu trường là lead không kết nối được.

### 7.1 Trường

| # | Trường | Bắt buộc | Ghi chú |
|---|---|---|---|
| 1 | Full name | ✅ | |
| 2 | **Country code + phone** | ✅ | Hai ô riêng. Bàn phím số. `inputmode="tel"` |
| 3 | **Email** | ✅ | **Bắt buộc ở gói QT** — lệch múi giờ nên email là kênh chắc chắn nhất |
| 4 | **Country / market** | ✅ | Quyết định luật áp dụng và kênh liên hệ |
| 5 | Service of interest | ✅ | Bottom sheet, không `<select>` thường |
| 6 | **Preferred messaging channel** | ✅ | WhatsApp · Telegram · Viber · Line · KakaoTalk · Zalo — **chọn 1**, không chọn nhiều |
| 7 | ★ **Preferred contact time + time zone** | ✅ | **Trường quan trọng nhất của form này** — xem 7.2 |
| 8 | Planned travel window | — | Tháng/khoảng tháng. Giúp bộ phận quốc tế xếp lịch |
| 9 | Note | — | |
| 10 | **Consent checkbox** | ✅ | Không tick sẵn · nêu rõ **chuyển dữ liệu sang Việt Nam** · link privacy policy mở được |

⛔ **Không** hỏi giới tính nếu không có lý do vận hành. ⛔ Không hỏi hộ chiếu, ngày sinh, tình trạng bệnh trên form công khai.
⛔ **Không** bắt upload ảnh ở form đầu tiên — ảnh là dữ liệu sức khoẻ, cần luồng riêng có thông báo riêng (`kn-rao-phap-ly-qt.md` §3).

### 7.2 Vì sao trường ⑦ quyết định tỷ lệ kết nối

Bệnh viện mở **8am–5pm giờ Việt Nam (UTC+7)**. Nghĩa là:

| Giờ VN 8am–5pm | = giờ khách |
|---|---|
| Sydney | 11am – 8pm ✅ |
| Dubai | 5am – 2pm ⚠️ |
| London | 1am – 10am ⚠️ |
| Los Angeles | **5pm – 2am** 🔴 |

→ Lead từ California gửi form buổi tối ở họ sẽ **không có ai trả lời trong ~12 giờ**, và cuộc gọi lại sẽ đến vào lúc 2 giờ sáng giờ họ.
→ Không thu trường ⑦ thì lead tầng C **mất phần lớn ở khâu kết nối**, và báo cáo sẽ hiển thị như "lead chất lượng kém" trong khi vấn đề là **múi giờ**.

**Trang thank-you phải nói rõ:** *"Our international patient team will contact you on [channel] within [N] working hours, between 8am and 5pm Vietnam time (UTC+7) — that is [giờ quy đổi theo country đã chọn]."*

### 7.3 Spec UI form

- `.input` / `.select-btn`: `min-height:52px` · `border:1px solid var(--line)` · `border-radius:var(--r)` · **`font:400 16px var(--f)`**.
- Focus: `border-color:var(--teal)` + `box-shadow:0 0 0 3px rgba(0,95,136,.16)`.
- Lỗi: viền `--err` + nền `--err-t` + `.err` 14px/600, `aria-describedby` trỏ tới ô lỗi.
- **Honeypot** input ẩn + `aria-hidden="true"`.
- `aria-live="polite"` cho vùng trạng thái submit · spinner trong nút khi đang gửi.
- `.privacy` 14px dưới nút submit, `--ink-2`.
- Màn **thank-you là một view riêng**, không phải `alert()`.
- **Nhãn hiện rõ phía trên ô** — ⛔ không dùng placeholder làm nhãn (khách đọc tiếng Anh ngôn ngữ thứ hai cần nhãn ở lại trên màn).
- ⛔ Không CAPTCHA chữ méo. Dùng honeypot + rate-limit phía server.

> ⚠️ Form production hiện có CAPTCHA kiểu *"Please fill in the result before sending"* — đây là rào ma sát làm mất lead, nhất là trên mobile. Đề xuất thay bằng honeypot.

---

## §8. MOBILE-FIRST & HIỆU NĂNG — CHECKLIST BẮT BUỘC

☐ Thiết kế **375–430px trước**, desktop sau — nhưng **desktop phải đẹp thật**, không phải phóng to mobile
☐ **Sticky bar mobile: WhatsApp | Call | Book**
☐ Body ≥ 16px · nút ≥ 48px cao · vùng chạm ≥ 44px
☐ Hero đọc hiểu trong **3 giây**, CTA thấy ngay không cần cuộn
☐ **LCP < 2,5s** — ⚠️ gói QT khắt khe hơn: khách ở Úc/GCC tải từ xa, **dùng CDN hoặc đo từ đúng thị trường đó**, không đo từ Hà Nội
☐ Ảnh WebP/AVIF · video lazy · ảnh hero **không** lazy
☐ Click-to-call có **mã quốc gia đầy đủ** `tel:+84981615151` — thiếu `+84` là số không gọi được từ nước ngoài
☐ **WhatsApp deep-link** `https://wa.me/84981615151?text=...` — kiểm thật
☐ Không bảng ngang tràn màn · không phải zoom để đọc
☐ `lang="en"` đúng · `hreflang` nếu có nhiều phiên bản ngôn ngữ
☐ Giờ làm việc **luôn kèm múi giờ**
☐ Market RTL (Arabic) → kiểm `dir="rtl"`, dùng thuộc tính logic (`margin-inline`, `inset-inline`) — CSS ở §5 đã dùng sẵn

---

## §9. SCORECARD — chấm trước khi giao

| Tiêu chí | Điểm |
|---|---|
| Message-match với ad / keyword / `market` | 18 |
| Đúng khung theo **chặng × tầng** (§1) | 12 |
| Trust: đủ mật độ và **đúng bộ bằng chứng được phép dùng ở market đó** | 18 |
| ★ **Gỡ rào cản XA: B08 + B09 có số ngày ở lại, ai liên hệ, trong bao lâu** | **15** |
| CTA: đủ 4 câu hỏi · đúng nấc · **đúng kênh của market** · form đạt §7 | 15 |
| Mobile-first + hiệu năng (§8) | 12 |
| UI: nhất quán §5, rõ thứ bậc thị giác, đạt 7 rào tương phản | 10 |
| **Cổng pháp lý `kn-rao-phap-ly-qt.md`** | **Fail = 0 điểm toàn bài** |

**≥ 80** → giao · **65–79** → sửa theo danh sách lỗi · **< 65** → làm lại từ bước chọn khung.

Tự chấm thật. Cho điểm cao một trang yếu là làm hỏng vòng học.

> Tiêu chí **rào cản XA 15 điểm** là tiêu chí riêng của gói QT. Một trang English rất đẹp, trust rất đầy, nhưng không nói **số ngày ở lại** và **ai lo sau khi về** thì **không thể đạt 80** — và đúng như vậy, vì trang đó sẽ không ra ca.

---

## §10. LUỒNG LÀM VIỆC MODE 3 (LDP-BUILD)

1. Nhận cụm từ khoá + `market` + tầng → xác định **chặng**, chốt khung **L1–L6**, **nói rõ vì sao**.
2. Lấy trust/bác sĩ/quy trình từ `kn-ho-so-thuong-hieu-qt.md`; giá lấy từ `/price-list/` tại thời điểm chạy.
3. **Rà bộ bằng chứng theo market** — tầng C thì loại testimonial kết quả và before–after ra khỏi kế hoạch **trước khi viết**, không loại sau.
4. Kiểm **B08 + B09**: có số ngày ở lại chưa? Chưa → `[PENDING: minimum stay — Medical Dept]`, **không bịa**.
5. **Mặc định hỏi:** *"Xuất copy-deck trước, hay dựng thẳng HTML?"*
6. Dựng HTML thì tuân §5 + §7, kèm **bảng kê ảnh cần cấp** và **danh sách `[PENDING]`** cuối trang.
7. Tự chấm §9 và in bảng điểm.


===== kn-quy-trinh-tuan-qt.md =====

# QUY TRÌNH TUẦN & BỘ CHỈ SỐ BÁO CÁO — GÓI QUỐC TẾ
Version: 1.0 — 2026-10-21 · dựng theo quy trình vận hành do người phụ trách khai

> File này nối **bốn bước rời** của gói thành **một vòng lặp hằng tuần**: chọn từ khoá → gom cụm → kế hoạch sản xuất landing → đo và báo cáo → quay lại bước 1.
> Khác với các file kia (mô tả *cách làm từng việc*), file này mô tả **nhịp làm việc** và **cái gì chảy từ bước này sang bước kia**.

---

## §1. BỐN BƯỚC — VÀ THỨ CHẢY GIỮA CHÚNG

```
BƯỚC 1 · CHỌN TỪ KHOÁ                    BƯỚC 2 · GOM CỤM
nguồn: GEO · LDP đang chạy · Planner  →  1 cụm = 1 landing
         ↓                                        ↓
BƯỚC 4 · ĐO & BÁO CÁO                    BƯỚC 3 · KẾ HOẠCH SẢN XUẤT
bộ chỉ số tuần này → tuần tới         ←  landing nào làm trước, ngân sách bao nhiêu
```

**Luật nối:** mỗi bước chỉ được bắt đầu khi bước trước đã giao đủ **thứ bắt buộc chảy xuống** (§6). Thiếu thì bước sau phải **đoán**, và đoán sai ở gói này là rủi ro pháp lý chứ không chỉ là lãng phí.

---

## §2. BƯỚC 1 — CHỌN TỪ KHOÁ

### 2.1 Ba nguồn từ khoá, theo thứ tự ưu tiên

| # | Nguồn | Lấy gì | Vì sao đứng ở vị trí này |
|---|---|---|---|
| ① | **Bộ truy vấn GEO** (`kn-truy-van-geo-qt.md`) | 83 truy vấn tiếng Anh, 15 cụm, đã chấm 80/20 | **Đây là câu khách thật sự gõ**, đã phân tầng và đã gắn rào pháp lý. Không phải suy đoán |
| ② | **Landing đang chạy** | Truy vấn thực tế đổ vào trang: GA4 `sessionGoogleAdsQuery` · `sessionGoogleAdsKeyword` · Search terms report | Dữ liệu của chính mình, nói đúng khách **đang** gõ gì, không phải khách lẽ ra gõ gì |
| ③ | **Keyword Planner** | Volume · CPC | Chỉ để **điền hai cột trống**, không phải để chọn từ khoá. Chạy **riêng theo từng market** |

⛔ **Không bắt đầu từ Keyword Planner.** Volume lớn nhất gần như luôn là từ khoá giá trị thấp nhất (`plastic surgery vietnam`). Bắt đầu từ ① và ②, rồi dùng ③ để định giá.

### 2.2 Ba nhóm người tìm — phân biệt trước khi gom cụm

Ba nhóm này gõ **gần giống nhau** nhưng là ba người khác nhau. Nhầm là hỏng cả cụm lẫn landing.

| Nhóm | Là ai | Tìm bằng | Ở đâu | `market` · `geo_mode` |
|---|---|---|---|---|
| **Khách quốc tế** | Người nước ngoài ở nước họ | English | Nước họ | `AU`/`US`/… · `Presence+Interest` |
| **Kiều bào** | Người Việt sống ở nước ngoài | **Tiếng Việt** | Nước họ | `VN-DIASPORA-*` · `Presence+Interest` |
| **Expat** | Người nước ngoài **đang ở VN**, lưu trú quanh **Hà Nội · TP.HCM** | English | **Trong VN** | `VN-EXPAT` · **`Presence`** |

> ⚠️ **Người Việt nói tiếng Anh** cũng xuất hiện trong dữ liệu tìm kiếm tiếng Anh. Họ **không phải** khách quốc tế: họ ở trong nước, không có rào cản XA, không cần phiên dịch. Nếu không tách, họ sẽ kéo CPL xuống trông đẹp mà không ra ca quốc tế nào. Tách bằng `geo_mode` + báo cáo cắt theo `country`.

### 2.3 Mục đích của bước này: **XUẤT HIỆN**

Khách quốc tế tìm qua **hai cửa**, và cả hai đều phải có mặt:

| Cửa | Là gì | Đo bằng |
|---|---|---|
| **AI Search** | ChatGPT · Gemini · AI Overview | **Share of Voice** — 20 prompt ở `kn-truy-van-geo-qt.md` §6 |
| **Google Search** | Kết quả tìm kiếm trả tiền + tự nhiên | Impression share · thứ hạng · CTR |

→ Một cụm từ khoá chỉ coi là "đã phủ" khi **có mặt ở cả hai cửa**. Chạy ads mà AI không nhắc tên là mất một nửa lượt tìm, và ngược lại.

---

## §3. BƯỚC 2 — GOM CỤM TỪ KHOÁ ⟹ MỖI CỤM MỘT LANDING

**Luật gom:** `1 dịch vụ × 1 chặng × 1 intent × 1 tầng thị trường = 1 cụm = 1 landing page`.

Chi tiết và lý do: `kn-cong-win-tu-khoa-qt.md` §5.

**Đầu ra bắt buộc của bước này** — bảng cụm, mỗi dòng đủ:

| Cột | Ví dụ |
|---|---|
| Mã cụm | `C-S4-AU-RHINO` |
| Dịch vụ · chặng · intent · tầng | Rhinoplasty · S4 · kế hoạch · C |
| `market` · `geo_mode` | AU · Presence+Interest |
| Số từ khoá · điểm WIN trung bình | 12 dòng · 3,4/4 |
| **Khung landing** | L3 Trip-plan |
| **Rào cản phải gỡ** | XA |
| Rào pháp lý chạm | R1 · R8 |

⛔ Cụm nào chưa khai được **khung landing** và **rào cản phải gỡ** thì **chưa gom xong** — bước 3 sẽ phải đoán.

---

## §4. BƯỚC 3 — KẾ HOẠCH SẢN XUẤT LANDING + NGÂN SÁCH TUẦN

### 4.1 Xếp thứ tự sản xuất

Không làm theo thứ tự cụm được nghĩ ra. Xếp theo **điểm sản xuất**:

```
Điểm = (ý định mua × giá trị ca × khả năng chốt) ÷ công sức sản xuất
```

**Ba thứ đẩy một cụm lên đầu hàng:**
① Thuộc **3 ngách ưu tiên** (từ khoá S4 · tiếng Việt kiều bào · sửa lại) — `kn-cong-win-tu-khoa-qt.md` §8.
② **Không bị chặn dữ liệu** — cụm cần số ngày ở lại mà chưa có số thì **không xếp đầu hàng**, dù điểm cao.
③ **Dùng lại được khối** đã làm ở landing trước.

### 4.2 Ngân sách tuần

| Ràng buộc | Mức |
|---|---|
| Chặng S3 · nỗi sợ | ≥ 10% |
| **Chặng S4 · kế hoạch chuyến đi** | **≥ 15%** |
| **Tầng B · kiều bào** | **≥ 15%** |
| Tổng | đúng 100% |

Chia theo **ý định mua × giá trị ca**, ⛔ không theo lượng tìm kiếm.

### 4.3 Bảng kế hoạch tuần — đầu ra của bước 3

| Cụm | Landing | Khung | Trạng thái | Ngân sách tuần | Chặn bởi | Ai làm | Xong khi nào |
|---|---|---|---|---|---|---|---|

**Trạng thái** dùng đúng 5 giá trị: `chưa làm` · `đang viết` · `chờ duyệt` · `chờ ảnh` · `đang chạy`.
Cột **Chặn bởi** để trống nếu không vướng; có vướng thì ghi tên dữ liệu và **ai phải cấp**.

---

## §5. BƯỚC 4 — BỘ CHỈ SỐ ĐO LƯỜNG & BÁO CÁO

### 5.1 ⚠️ Hai tầng chỉ số — đừng trộn

| Tầng | Đo cái gì | Nhịp đọc | Dùng để |
|---|---|---|---|
| **Chỉ số sớm** | Trang có giữ được người không | **Hằng ngày / hằng tuần** | Sửa trang, sửa mẫu QC |
| **Chỉ số thật** | Có ra ca không | **Theo cohort, ≥ 8 tuần** | Quyết định ngân sách |

⛔ **Không dùng chỉ số sớm để quyết định ngân sách.** Trang có time-on-site đẹp mà không ai đặt cọc vẫn là trang hỏng. Và ngược lại: ⛔ **không chờ chỉ số thật mới sửa trang** — đợi 8 tuần mới biết hero sai là mất 8 tuần.

### 5.2 Chỉ số sớm — đọc hằng ngày, nguồn GA4

| Chỉ số | Trường GA4 | Ngưỡng cảnh báo |
|---|---|---|
| Lượt xem trang | `screenPageViews` | — |
| Phiên | `sessions` · `engagedSessions` | — |
| **Thời gian trên trang** | `averageSessionDuration` · `avgUserEngagementDuration` | **< 45 giây** → hero sai hoặc sai khung |
| Tỷ lệ tương tác | `engagementRate` | < 40% → message-match hỏng |
| Tỷ lệ thoát | `bounceRate` | > 70% → landing không khớp từ khoá |
| Chuyển đổi trên trang | `conversions` · `sessionConversionRate` | — |

**Cắt theo:** `landingPage` · `country` · `sessionDefaultChannelGrouping` · `deviceCategory` · `sessionGoogleAdsQuery`.

> Hai chỉ số **xem trang** và **time on site** là bộ đôi của bước 1 — chúng trả lời câu *"từ khoá này có kéo đúng người không"*, không trả lời câu *"có ra ca không"*.

### 5.3 Chỉ số thật — đọc theo cohort, nguồn Google Ads + CRM

Phễu 8 bước và luật độ trễ 4–12 tuần: `kn-chan-doan-chi-so-qt.md`.

| Chỉ số | Nguồn | Vai trò |
|---|---|---|
| Chi phí · click · CTR · CPC | Google Ads | Đầu vào |
| Lead | GA4 `conversions` + CRM | — |
| **Tỷ lệ phản hồi được** | CRM | Chẩn đoán **múi giờ + kênh**, không phải từ khoá |
| **Tỷ lệ đặt cọc** | CRM | **Điểm chuyển trạng thái thật** |
| **Chi phí / khách ĐẾN KHÁM** | Ads + CRM | **⭐ Chỉ số bắc đẩu** |

### 5.4 Khuôn báo cáo tuần

Báo cáo gồm **đúng hai bảng và một danh sách**:

**Bảng A — tuần này, cắt 4 chiều**

| Landing | market | Tầng | Chặng | Xem trang | Time on site | Phiên | Tỷ lệ tương tác | Lead | Đặt cọc | Đến khám | Chi phí/đến khám | Cohort |
|---|---|---|---|---|---|---|---|---|---|---|---|---|

**Bảng B — tuần tới**

| Việc | Vì số nào | Ai làm | Đo lại bằng gì |
|---|---|---|---|

**Danh sách C — đang bị chặn**: dữ liệu còn thiếu, ai phải cấp, chặn landing nào.

⛔ **Báo cáo thiếu cột `market` hoặc cột `cohort` là báo cáo không dùng được để ra quyết định** — nó chỉ đẹp. Gộp AU với KH vào một dòng là gộp hai thị trường khác luật, khác giá, khác múi giờ.

---

## §6. THỨ BẮT BUỘC CHẢY GIỮA CÁC BƯỚC

| Trường | B1→B2 | B2→B3 | B3→B4 |
|---|---|---|---|
| `market` · `geo_mode` | ✅ | ✅ | ✅ |
| Tầng (A/B/C/D) | ✅ | ✅ | ✅ |
| Chặng S1–S7 | ✅ | ✅ | ✅ |
| **Rào cản phải gỡ** | ✅ | ✅ | ✅ |
| Khung landing L1–L6 | — | ✅ | ✅ |
| Rào pháp lý chạm (R#) | ✅ | ✅ | ✅ |
| Danh sách `[PENDING]` tích luỹ | ✅ | ✅ | ✅ |

> Dòng hay rơi nhất là **rào pháp lý chạm**. Rơi nó thì tới bước duyệt mới phát hiện phải bỏ cả khối, và trang phải làm lại từ bước chọn bằng chứng.

---

## §7. ⚠️ TRẠNG THÁI KẾT NỐI DỮ LIỆU — tra 2026-10-21

| Nguồn | Trạng thái | Ghi chú |
|---|---|---|
| **GA4 — site quốc tế** | ✅ **đã kết nối** | Property **`417341092`** = `kangnamaesthetichospital.com` |
| GA4 — site nội địa | ✅ đã kết nối | Property `253218410` = `benhvienthammykangnam.com.vn` *(gói nội địa dùng)* |
| **Google Ads** | ❌ **chưa có tài khoản nào được nối** | Phải nối trước khi có bất kỳ chỉ số chi phí nào |
| Google Ads Keyword Planner | ⚠️ đã xác thực nhưng chưa kéo được | Dùng để điền 2 cột `volume` · `cpc` |
| **Trình kéo dữ liệu (Supermetrics)** | 🔴 **trial hết hạn 24/07/2026** | **Chặn mọi truy vấn số liệu tự động** |

**Hệ quả:** bước 4 hiện **chạy tay** — đọc số trực tiếp trên GA4 và Google Ads, điền vào khuôn §5.4. Khuôn và tên trường ở §5.2 đã khai đúng theo GA4 nên khi nối lại được thì dùng ngay, không phải dựng lại.

**Ba việc cần làm để bước 4 tự động:**
① Gia hạn hoặc đổi gói trình kéo dữ liệu.
② **Nối tài khoản Google Ads** — hiện chưa có tài khoản nào.
③ Khai **3 tag CRM** `market` · `tier` · `stage` cho mọi lead, từ Pha 1. Thiếu tag thì mọi cột phía sau của bảng A là lead mù.

---

## §8. NHỊP TUẦN

| Khi nào | Làm gì | Mất bao lâu |
|---|---|---|
| **Thứ 2** | Đọc chỉ số sớm tuần trước → chốt bảng B (việc tuần này) | 30 phút |
| Trong tuần | Sản xuất theo bảng kế hoạch §4.3 | — |
| **Thứ 6** | Cập nhật trạng thái landing · ghi `[PENDING]` mới phát sinh | 15 phút |
| **Đầu tháng** | Chạy 20 prompt đo **Share of Voice** (`kn-truy-van-geo-qt.md` §6) | 1 giờ |
| **Mỗi 8 tuần** | Đọc cohort → quyết định ngân sách | 1 buổi |

⛔ **Không ra quyết định ngân sách ở nhịp tuần.** Nhịp tuần để sửa trang và sửa mẫu quảng cáo; ngân sách đi theo nhịp cohort 8 tuần (`kn-chan-doan-chi-so-qt.md` §2).


===== kn-rao-phap-ly-qt.md =====

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

> ✅ **Chốt 2026-10-21 — pháp nhân:** **Công ty TNHH Bệnh viện Thẩm mỹ Kangnam Sài Gòn**, MST 0312155633, giấy phép KCB **287/BYT-GPHĐ** (03/12/2020).
> ✅ **Chốt 2026-10-21 — nha khoa:** Kangnam **có chuyên khoa Nha khoa thẩm mỹ** vận hành dưới chính pháp nhân này (4 dịch vụ: niềng răng · bọc sứ · Implant · Veneer). Nguồn: trang chuyên khoa trên site nội địa. → **Cụm Q08 không còn bị chặn vì câu hỏi pháp nhân.**
> ⚠️ **Hai điều vẫn phải giữ:**
> ① **Bằng chứng trên chỉ thuộc cơ sở TP.HCM (287).** Chưa có bằng chứng cho **Hà Nội (194)** → nội dung nha khoa cho khách quốc tế **mặc định trỏ về TP.HCM**, trừ khi Pháp chế xác nhận 194 cũng có RHM trong phạm vi.
> ② **Trang web không phải văn bản phạm vi giấy phép.** Chỉ **phụ lục phạm vi hoạt động chuyên môn** của giấy phép mới chứng minh được một kỹ thuật nằm trong phạm vi. Trước khi phát hành, Pháp chế vẫn rà phụ lục đó cùng lúc với **GXNNDQC (R9)** — đây là bước có sẵn trong quy trình, không phải việc phát sinh.
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
| ~~**Nha khoa** *(Q08)*~~ ✅ | **Đã gỡ chặn 2026-10-21** — nha khoa vận hành dưới chính pháp nhân BVTM Kangnam Sài Gòn (287/BYT-GPHĐ). Điều kiện còn lại khi viết: **trỏ về cơ sở TP.HCM**, và ghi đúng số **287** | R3 phần pháp nhân đã xong. Nếu muốn nội dung nha khoa cho **Hà Nội** thì phải xác nhận 194 trước |
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
| 14 | ~~R3 — pháp nhân cho site EN~~ | ✅ **ĐÃ CHỐT 2026-10-21: Bệnh viện Thẩm mỹ Kangnam** |
| 14b | ~~R3 — nha khoa có thuộc pháp nhân BVTM Kangnam không~~ | ✅ **ĐÃ CHỐT 2026-10-21: có, chuyên khoa Nha khoa thẩm mỹ, giấy phép 287** |
| 14c | **R3 — cơ sở Hà Nội (194/BYT-GPHĐ)** có RHM trong phạm vi không *(chỉ cần nếu muốn làm nội dung nha khoa cho Hà Nội)* | `[CHỜ CẬP NHẬT]` |
| 14d | **Phụ lục phạm vi hoạt động chuyên môn** của 287 và 194 — rà cùng lúc với GXNNDQC trước khi phát hành | `[CHỜ CẬP NHẬT]` |
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


===== kn-thi-truong-quoc-te.md =====

# THỊ TRƯỜNG QUỐC TẾ — PHÂN TẦNG & LUẬT CHỌN THỊ TRƯỜNG
Version: 1.0 — 2026-10-21 · file **lõi** của gói QT, không có tương đương ở gói nội địa

> Gói nội địa chia việc theo **ZONE dịch vụ** (Mũi · Mắt · Hàm mặt…). Gói quốc tế chia theo **THỊ TRƯỜNG × DỊCH VỤ**.
> Lý do: cùng một ca nâng mũi, khách Campuchia và khách Úc có **động cơ khác nhau, rào cản khác nhau, ngôn ngữ khác nhau, giá chấp nhận được khác nhau và luật quảng cáo khác nhau**. Gộp họ vào một chiến dịch là lỗi nền tảng của gói này.

---

## §1. BỐN TẦNG THỊ TRƯỜNG

Phân tầng theo **logic ra quyết định**, không theo khoảng cách địa lý hay GDP.

| Tầng | Ai | Động cơ chính | Rào cản nặng nhất | Ngôn ngữ tìm kiếm | Giá trị ca |
|---|---|---|---|---|---|
| **A · Khu vực lân cận** | Campuchia · Lào · Myanmar · Indonesia · Philippines · Malaysia · Ấn Độ | Gần + rẻ hơn Thái/Hàn + kỹ thuật Hàn | **NGỜ** (cơ sở có thật không, có phép không) | English · Khmer · Bahasa · mix bản địa | Trung bình–Cao |
| **B · Kiều bào (Việt kiều)** | Mỹ · Úc · Canada · Đức · Czech · Nhật · Hàn · Đài Loan | Về thăm nhà **+** làm thẩm mỹ trong cùng chuyến | **XA** (ai lo cho tôi khi tôi bay về) | **Tiếng Việt** + English | Cao–Rất cao |
| **C · Thị trường phát triển** | Úc · Mỹ · UK · NZ · Canada · GCC (UAE · Saudi · Kuwait) | Chênh giá 60–80% so với nước họ | **SỢ** + **XA** (mổ ở nước ngoài có an toàn không) | English (GCC thêm Arabic) | **Rất cao** |
| **D · Expat đang sống tại VN** | Người nước ngoài làm việc/định cư ở HN · TP.HCM | Tiện + cần bác sĩ nói được tiếng Anh | **NGỜ** (giao tiếp, tiêu chuẩn y khoa) | English | Trung bình–Cao |

### 1.1 Vì sao tầng B và tầng D hay bị bỏ sót — và đó là sai lầm đắt nhất

**Tầng B (kiều bào)** là tầng **dễ chốt nhất** trong bốn tầng và thường bị gộp vào tầng C:
- Họ **đã tin thương hiệu Việt**, không phải thuyết phục từ số 0.
- Họ nói được tiếng Việt → không cần phiên dịch → chi phí phục vụ thấp nhất.
- Họ **đã có vé máy bay** vì lý do khác (Tết · hè · cưới hỏi · tang lễ) → rào cản chi phí đi lại **bằng không**.
- Nhưng họ tìm kiếm bằng **tiếng Việt từ IP nước ngoài** — nếu chiến dịch chỉ nhắm từ khoá tiếng Anh thì không bao giờ gặp họ.

→ **Luật:** tầng B phải có chiến dịch riêng, **từ khoá tiếng Việt**, **geo-target = nước đang sống**, và lịch theo **mùa bay** (§4).

**Tầng D (expat tại VN)** không phải medical tourism — họ **đã ở trong nước**. Gộp vào chiến dịch du lịch y tế làm hỏng cả hai: landing nói về đưa đón sân bay và khách sạn là vô nghĩa với người đang sống ở Hà Nội.

→ **Luật:** tầng D dùng **geo-target Presence (đang ở VN)**, landing **không có** khối du lịch, CTA là *đặt khám trực tiếp*.

---

## §2. ⚠️ CỔNG GEO — RÀNG BUỘC CỨNG CỦA GÓI NÀY

Đây là cổng tương đương với **cổng TUYẾN** của gói nội địa. Mức độ nghiêm trọng như nhau.

**Vấn đề:** cùng một từ khoá, hai người hoàn toàn khác nhau.

> `"plastic surgery hanoi"`
> — gõ từ **Sydney** = khách tầng C đang lên kế hoạch bay sang, cần giá · hộ chiếu · số ngày ở lại · bảo hành từ xa.
> — gõ từ **Hà Nội** = expat tầng D đang sống ở đó, cần địa chỉ · bác sĩ nói tiếng Anh · đặt khám tuần này.
>
> Một landing, một mẫu quảng cáo → **mất cả hai**.

**Luật:** mọi dòng từ khoá **phải khai đủ hai trường**, không được để trống:

| Trường | Giá trị | Nghĩa |
|---|---|---|
| `market` | mã thị trường (`AU` · `US` · `KH` · `VN-EXPAT` · `VN-DIASPORA-AU`…) | **Người gõ đang ở đâu** — không phải thành phố trong từ khoá |
| `geo_mode` | `Presence` hoặc `Presence+Interest` | Kiểu nhắm vị trí trong Google Ads |

**Quy tắc chọn `geo_mode`:**

| Tầng | `geo_mode` | Vì sao |
|---|---|---|
| A · B · C (du lịch y tế) | **`Presence+Interest`** | Cần hứng cả người đang ở nước họ **và** người đang tìm hiểu về Việt Nam |
| **D · expat tại VN** | **`Presence` — bắt buộc** | Dùng `Presence+Interest` ở đây sẽ hút toàn bộ traffic du lịch y tế vào landing sai |

⛔ **Để mặc `geo_mode` = Google tự chọn `Presence or interest`** (mặc định của nền tảng) → chiến dịch expat bị tràn traffic quốc tế, CPL trông rẻ mà không ai đến khám. Đây là lỗi tốn tiền nhất của gói này, và nó **im lặng** — không có cảnh báo nào trong Google Ads.

**Cổng tự động:** `tools/build_keyword_workbook.py` **chặn build** nếu một dòng từ khoá có tên thành phố Việt Nam (hanoi · ho chi minh · saigon · hcmc · da nang…) mà **không khai** `market` và `geo_mode`.

---

## §3. BẢN ĐỒ THỊ TRƯỜNG × DỊCH VỤ — dịch vụ nào bán được cho tầng nào

Không phải dịch vụ nào cũng bay được. Phép thử: **giá trị ca có đủ bù chi phí một chuyến bay + khách sạn + số ngày nghỉ việc không?**

| Dịch vụ | Tầng A | Tầng B | Tầng C | Tầng D | Ghi chú |
|---|---|---|---|---|---|
| **Rhinoplasty** (nâng mũi) | ✅ lõi | ✅ lõi | ✅ **lõi** | ✅ | Dịch vụ đầu kéo của cả 4 tầng |
| **Breast augmentation** | ✅ | ✅ | ✅ **lõi** | ✅ | Giá trị ca cao nhất, scrutiny cao nhất |
| **V-line / jaw contouring** | ✅ | ✅ | ✅ | ⚠️ | Đại phẫu — số ngày ở lại dài nhất |
| **Facelift / neck lift** | ⚠️ | ✅ **lõi** | ✅ **lõi** | ✅ | Tầng B và C: độ tuổi cao, ngân sách lớn |
| **Liposuction / Lipo 360** | ✅ | ✅ | ✅ | ✅ | ⛔ Cấm before–after cơ thể (§5) |
| **Eyelid surgery** | ✅ | ✅ | ✅ | ✅ | Giá thấp nhất trong nhóm phẫu thuật → chỉ bán được khi **ghép combo** |
| **Hair transplant (ICEFUE)** | ✅ | ✅ | ✅ **lõi** | ✅ | Khách nam, rào cản riêng tư rất cao |
| **Facial paralysis / reconstructive** | ✅ | ✅ | ⚠️ | ✅ | Ngách hẹp, intent y tế thật — CPC thấp, giá trị cao |
| **Da liễu · spa · clinic đơn lẻ** | ❌ | ⚠️ | ❌ | ✅ **lõi** | **Không bay vì một buổi trị nám.** Chỉ bán cho tầng D, hoặc làm cross-sell tại chỗ |
| **Nha khoa (KDT)** | ✅ | ✅ | ✅ | ✅ | Sub-brand riêng — xem ranh giới ở `kn-ho-so-thuong-hieu-qt.md` |

**Luật combo.** Dịch vụ giá thấp (mí mắt · da liễu · clinic) **chỉ chạy cho tầng A/B/C khi ghép vào gói combo** với một ca lớn. Chạy đơn lẻ cho khách quốc tế là đốt ngân sách: không ai bay 6 giờ để cắt mí.
→ Từ khoá dịch vụ giá thấp + tầng A/B/C: `win` tối đa **2/4**, và `ghi_chu` phải khai *"chỉ dùng làm cụm combo / cross-sell, không dựng landing riêng"*.

---

## §4. MÙA — LỊCH CHẠY THEO MÙA BAY, KHÔNG THEO MÙA KHUYẾN MÃI

Khách nội địa đặt lịch khi có ưu đãi. Khách quốc tế đặt lịch khi **có vé máy bay**. Hai nhịp hoàn toàn khác nhau.

| Mùa | Tầng ảnh hưởng | Nhịp |
|---|---|---|
| **Trước Tết 8–10 tuần** | **B** (kiều bào) | Cao điểm số 1 của tầng B. Chạy từ **tháng 10–11** cho ca Tết, không chạy vào đúng Tết |
| **Hè (6–8)** | B · C | Kỳ nghỉ dài, phụ huynh đưa con đi cùng |
| **Mùa khô VN (11–4)** | A · C | Thời tiết thuận cho hồi phục — dùng được làm lý do thật cho *"tại sao là bây giờ"* |
| **Ramadan + Eid** | **C (GCC)** | ⛔ **Không** chạy ca phẫu thuật trong Ramadan. Chạy **trước** Ramadan và **sau Eid** |
| **Trước cưới 3–6 tháng** | A · B · C | Tình huống, không phải mùa — nhưng là intent mạnh nhất |

**Luật:** độ trễ lead → đến khám của khách quốc tế là **4–12 tuần**. Vì vậy:
- Chiến dịch tầng B/C **không được đánh giá trong cửa sổ ngắn hơn 8 tuần**.
- Ngân sách phải bật **trước cao điểm 8–10 tuần**, không bật đúng cao điểm.

Chi tiết về đo lường độ trễ này ở `kn-chan-doan-chi-so-qt.md`.

---

## §5. ⚠️ LUẬT QUẢNG CÁO THEO THỊ TRƯỜNG — HAI TẦNG PHÁP LÝ CÙNG LÚC

Đây là khác biệt pháp lý lớn nhất so với gói nội địa, và là chỗ dễ sai nhất.

**Nội dung chịu HAI hệ luật cùng lúc:**
① **Luật Việt Nam** — cơ sở ở VN, nội dung quảng cáo dịch vụ KCB cần **giấy xác nhận nội dung quảng cáo**. Áp dụng bất kể khách ở đâu.
② **Luật nước người xem** — nền tảng quảng cáo áp chính sách theo **vị trí người nhìn thấy quảng cáo**, không theo vị trí người đăng.

→ Một mẫu quảng cáo hợp pháp ở Việt Nam **vẫn có thể bị từ chối hoặc bị cơ quan quản lý nước đích xử lý**.

### 5.1 Bảng rủi ro theo thị trường — **phải verify trước khi bật, không được suy đoán**

| Thị trường | Cơ quan / bộ quy tắc cần tra | Điểm nóng đã biết | Mức rủi ro |
|---|---|---|---|
| **Úc (AU)** | AHPRA — *Guidelines for registered health practitioners who advertise regulated health services*; TGA | **Cấm testimonial về kết quả lâm sàng**; before–after bị ràng buộc rất chặt; cấm dùng từ gợi ý khuyến khích dịch vụ không cần thiết | 🔴 **Cao nhất** |
| **UK** | ASA / CAP Code; GMC | Không quảng cáo thuốc kê đơn (botox); yêu cầu bằng chứng cho mọi claim | 🔴 Cao |
| **EU/EEA** | luật quảng cáo y tế từng nước + **GDPR** cho form | GDPR: cần cơ sở pháp lý + thông báo **chuyển dữ liệu sang Việt Nam** | 🔴 Cao |
| **Mỹ (US)** | FTC — *Health Products Compliance Guidance*; luật từng bang | Claim phải có cơ sở; disclosure phải "clear and conspicuous" | 🟠 Trung bình–Cao |
| **Canada / NZ** | tương tự AU/UK, nhẹ hơn | Testimonial và before–after cần rà | 🟠 Trung bình |
| **GCC (UAE · Saudi · Kuwait)** | cơ quan y tế từng nước (vd DHA/MOHAP tại UAE) duyệt nội dung quảng cáo y tế | Yêu cầu giấy phép quảng cáo y tế riêng; chuẩn mực hình ảnh nghiêm | 🔴 Cao |
| **Campuchia · Lào · Indonesia · Philippines · Malaysia** | luật quảng cáo y tế từng nước | Ít tiền lệ thực thi hơn, **không có nghĩa là được phép** | 🟡 Trung bình |

⛔ **Luật tuyệt đối:** Agent **không đưa ra kết luận pháp lý**. Agent chỉ được **① nêu tên cơ quan/bộ quy tắc phải tra · ② gắn cờ ⚠️ vào đúng thành phần rủi ro · ③ đề xuất biến thể đã hạ rủi ro**. Dòng kết luận luôn là: *"cần Pháp chế xác nhận cho thị trường [X] trước khi bật"*.

### 5.2 Ba thành phần creative rủi ro cao — xử lý theo thị trường

| Thành phần | Tầng A | Tầng B/D | **Tầng C (AU · UK · EU · GCC)** |
|---|---|---|---|
| **Before–after** | ✅ nếu có consent | ✅ nếu có consent | 🔴 **Mặc định KHÔNG DÙNG** — cần Pháp chế duyệt riêng từng thị trường |
| **Testimonial / review khách** | ✅ nếu thật | ✅ nếu thật | 🔴 **Mặc định KHÔNG DÙNG cho claim kết quả lâm sàng** (AHPRA cấm thẳng). Chỉ được dùng về **trải nghiệm phi lâm sàng**: phiên dịch · đưa đón · khách sạn · thái độ nhân viên |
| **Before–after cơ thể / giảm béo** | ⛔ không | ⛔ không | ⛔ **không** — vi phạm cả policy Meta/Google ở mọi thị trường |

→ **Hệ quả thiết kế:** landing cho tầng C **không được dựa vào** before–after và testimonial làm trụ bằng chứng. Trụ bằng chứng của tầng C là: **giấy phép Bộ Y tế → hồ sơ bác sĩ (bằng cấp, CCHN, năm kinh nghiệm) → quy trình an toàn → chính sách bảo hành/chỉnh sửa có văn bản → quy trình chăm sóc từ xa sau khi về nước**.
Đây là lý do khối *"Out of Town Patients"* 5 bước trên trang tham chiếu quan trọng hơn khối testimonial: nó là bằng chứng **được phép dùng ở mọi thị trường**.

---

## §6. NGÔN NGỮ & VIẾT CHO NGƯỜI ĐỌC KHÔNG NÓI TIẾNG ANH BẢN NGỮ

Phần lớn khách tầng A và GCC đọc tiếng Anh như **ngôn ngữ thứ hai**. Luật viết:

- **Câu ngắn.** Một ý một câu. Tránh câu ghép nhiều tầng.
- **Không thành ngữ, không chơi chữ, không ẩn dụ.** *"Turn heads"* · *"a new lease on life"* → bỏ.
- **Số viết bằng chữ số**, kèm đơn vị rõ: `7–10 days`, không `about a week or so`.
- **Thuật ngữ y khoa đi kèm giải thích ngắn**: *"rhinoplasty (nose surgery)"* ở lần xuất hiện đầu.
- **Tên dịch vụ dùng đúng tên quốc tế**, không dịch nguyên văn từ tiếng Việt: `V-line surgery` không phải `jaw-grinding`.
- ⛔ **Không dùng giọng "khoe"** cho tầng A và GCC — văn hoá tiếp nhận khác.

**Ngôn ngữ theo tầng:**

| Tầng | Ngôn ngữ landing | Ngôn ngữ ad | Ghi chú |
|---|---|---|---|
| A | English | English + **Khmer** cho KH/LA | Site đã hỗ trợ Khmer — dùng lại |
| **B** | **Tiếng Việt** (chính) + English | **Tiếng Việt** | Viết như nói với người Việt ở xa, không như nói với người nước ngoài |
| C | English | English (+ Arabic cho GCC) | Register cao hơn, nhiều số liệu hơn |
| D | English | English | Nhấn *English-speaking doctor*, địa chỉ, giờ mở cửa |

⛔ **Không dùng máy dịch cho nội dung y khoa.** Bản Khmer/Arabic phải có người bản ngữ rà. Chưa có → ghi `[PENDING: native review — Khmer]` và **không bật** biến thể đó.

---

## §7. GIÁ & TIỀN TỆ — KHÁC HOÀN TOÀN GÓI NỘI ĐỊA

Gói nội địa **ẩn giá** (dữ liệu động, lấy tại `/bang-gia/`). Gói quốc tế **phải hiện giá** — vì **chênh giá chính là cái hook**. Khách tầng C vào trang để tìm đúng con số đó.

**Năm luật bắt buộc khi hiện giá:**

① **Luôn nêu đồng tiền.** USD là đơn vị chính cho tầng A/C, VND đi kèm trong ngoặc.
② **Luôn nêu phụ phí quốc tế.** Trang tham chiếu ghi nguyên văn: *"The price shown does not include 10% international service charge"*. **Bỏ dòng này là bom niềm tin** — khách phát hiện ở quầy thanh toán thì mất cả ca và nhận review xấu.
③ **Luôn nêu tỷ giá là tham chiếu**: *"USD figures are approximate and depend on the exchange rate on the day of payment"*.
④ **Luôn nêu cái gì có trong giá** — tư vấn · xét nghiệm · thuốc hậu phẫu · tái khám · bảo hành. Và cái gì **không** có — vé máy bay · khách sạn · phiên dịch (nếu tính riêng).
⑤ **Giá cuối do bác sĩ chốt sau khám**: *"Final cost is confirmed by the doctor after in-person examination"*.

⛔ **Không so sánh giá với một quốc gia hoặc cơ sở có tên.** *"70% cheaper than Australia"* là claim cần bằng chứng và là rủi ro ở AU/UK. Viết dạng: *"Published price list — compare it yourself"* và **để bảng giá nói thay**.

> Giá hiện tại lấy từ `/price-list/` tại thời điểm chạy. Bản chụp **2026-10-21** ở `kn-ho-so-thuong-hieu-qt.md` §6 — dùng để đối chiếu, **không dùng để đăng**.

---

## §8. SỐ NGÀY Ở LẠI VIỆT NAM — TRƯỜNG DỮ LIỆU QUAN TRỌNG NHẤT CHƯA CÓ

Với khách nội địa, câu chặn là *"nghỉ bao lâu mới đi làm được"*.
Với khách quốc tế, câu chặn là **"tôi phải ở Việt Nam bao nhiêu ngày"** — và đây là câu hỏi **kế hoạch**, không phải câu hỏi nỗi sợ. Nó quyết định khách có đặt vé hay không.

Khách không trả lời được câu này thì **không thể đặt vé**, và không đặt vé thì lead không bao giờ thành ca.

| Dịch vụ | Số ngày tối thiểu ở VN | Nguồn |
|---|---|---|
| Rhinoplasty | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| Breast augmentation | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| V-line / jaw | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| Facelift | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| Liposuction | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| Eyelid | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |
| Hair transplant | `[CHỜ CẬP NHẬT]` | Khoa Chuyên môn |

⛔ **Agent KHÔNG được tự suy ra số ngày này.** Đây là mốc y khoa (thời điểm cắt chỉ, tái khám, được phép bay), không phải con số marketing. Bay quá sớm sau phẫu thuật là **rủi ro y khoa thật**.
→ Chưa có số → ghi `[PENDING: minimum stay — Medical Dept]` đúng vị trí trên trang, **và liệt kê lại ở bảng cần bổ sung cuối output**.
→ Có số rồi thì viết dạng **khoảng + "varies by case"**, kèm nêu rõ **mốc nào** (ngày cắt chỉ · ngày tái khám cuối · ngày được phép bay).

**Điền xong bảng này là việc có đòn bẩy cao nhất trong cả gói.** Mọi landing tầng A/B/C đều cần nó.

---

## §9. SCHEMA MÃ THỊ TRƯỜNG — dùng trong cột `market`

```
AU · US · CA · UK · NZ · DE · CZ
AE · SA · KW · QA                  (GCC)
KH · LA · MM · ID · PH · MY · IN · SG · TH
JP · KR · TW · CN-HK
VN-EXPAT                            (tầng D — người nước ngoài đang ở VN)
VN-DIASPORA-<mã nước>               (tầng B — vd VN-DIASPORA-AU, VN-DIASPORA-US)
```

**Một chiến dịch = một tầng × một nhóm thị trường cùng luật quảng cáo.**
⛔ Không gộp `AU` với `KH` vào một chiến dịch: khác luật quảng cáo (§5), khác ngôn ngữ, khác giá chấp nhận được, khác múi giờ gọi lại.

---

## §10. BA SAI LẦM ĐẶC TRƯNG CỦA GÓI QUỐC TẾ

| Sai | Đúng |
|---|---|
| Dịch landing tiếng Việt sang tiếng Anh rồi chạy | Viết lại theo **rào cản XA** và **bộ bằng chứng được phép dùng ở thị trường đó** (§5.2) |
| Một landing English cho cả bốn tầng | 1 tầng × 1 nhóm thị trường × 1 dịch vụ = **1 trang** |
| Gộp kiều bào vào chiến dịch English | Tầng B chạy **từ khoá tiếng Việt**, geo-target nước đang sống (§1.1) |
| Đánh giá chiến dịch quốc tế sau 2 tuần theo CPL | Độ trễ 4–12 tuần → đo **chi phí trên khách đã đến khám**, cửa sổ ≥ 8 tuần (§4) |
| Để Google tự chọn kiểu nhắm vị trí | Khai `geo_mode` cho từng dòng từ khoá (§2) |
| Dùng testimonial kết quả cho thị trường Úc | Trụ bằng chứng tầng C = giấy phép → bác sĩ → quy trình → bảo hành → chăm sóc từ xa (§5.2) |


===== kn-truy-van-geo-qt.md =====

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

