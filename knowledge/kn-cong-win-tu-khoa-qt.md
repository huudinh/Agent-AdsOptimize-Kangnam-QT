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
