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
