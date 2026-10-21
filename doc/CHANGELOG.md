# CHANGELOG — ADS OPTIMIZE KANGNAM QUỐC TẾ

## v1.1 — 21/10/2026 · Nạp bộ truy vấn GEO + 4 rào pháp lý còn thiếu

Nguồn: **`HCI-Knowledge/GEOQUOCTE.xlsx`** (8 sheet, bản cập nhật 14/09/2026) → trích xuất thành [`knowledge/kn-truy-van-geo-qt.md`](../knowledge/kn-truy-van-geo-qt.md).

### Thêm MODE 5 · GEO-ANSWER

**83 truy vấn tiếng Anh · 15 cụm · 53 CORE 80/20.** Mục tiêu: khi khách nước ngoài hỏi AI bằng tiếng Anh về thẩm mỹ tại Việt Nam, **câu trả lời trích dẫn Kangnam**. Mục tiêu quý: **Share of Voice ≥ 30%** ở cụm Tầng A.

Đây là **kênh khác**, không phải quảng cáo trả tiền — và trộn lẫn là sai cả hai:

| | Ads (MODE 1–4) | **GEO (MODE 5)** |
|---|---|---|
| Đo bằng | CPL · chi phí/khách đến khám | **Share of Voice** |
| Nhịp | Tuần · cohort 8 tuần | **Quý** |
| Khung viết | **AIDA** (L1–L6) | **PAS** |
| `market` / `geo_mode` | ✅ bắt buộc | ⛔ **không có** |
| Cổng WIN 3/4 | ✅ | ⛔ không áp |

### ⚠️ Đổi tên: "cổng GEO" → "cổng GEO-TARGET"

Chữ **GEO** bị dùng cho hai thứ khác nhau, và nhầm là nhầm cả kênh:

| Viết là | Nghĩa | Thuộc |
|---|---|---|
| **GEO-TARGET** (`geo_mode`) | Geo-targeting — `Presence` vs `Presence+Interest` | Paid ads |
| **GEO** | **Generative Engine Optimization** — tối ưu để AI trích dẫn | MODE 5 |

→ Đã đổi tên nhất quán trong **9 file**. Trường JSON `geo_mode` **giữ nguyên** (là thuật ngữ Google Ads, không gây nhầm trong ngữ cảnh).

### ✅ Bộ GEO xác nhận độc lập ba kết luận của v1.0

Hai bộ được làm **độc lập** mà trùng kết luận — tín hiệu tốt, nghĩa là các kết luận đó không phải suy diễn:

| v1.0 tự dựng | Bộ GEO gọi là |
|---|---|
| **Rào cản XA** (*bay về rồi ai lo cho tôi*) | *"nỗi sợ riêng của medical tourism"* — cụm Q14+Q15, **10,9% điểm** |
| **Chặng S4 · kế hoạch chuyến đi** | **G-S4 · PLAN THE TRIP** — khớp **chính xác**, và cũng được xếp là đòn bẩy đặc thù |
| **Số ngày ở lại là nút thắt** | Q13-01 là truy vấn **Hot/P1/CORE** đứng đầu cụm logistics |
| **Giá phải hiện, bằng USD** | Q11 hạng 3 — *"bảng giá USD công khai min–max là đòn quyết định"* |

### 🔴 Bốn rào pháp lý v1.0 CÒN THIẾU — đã bổ sung vào `kn-rao-phap-ly-qt.md` §4b

Đây là phần có giá trị thực nhất từ bộ GEO. Cả bốn là **rào cứng**, áp cho **cả nội dung GEO và quảng cáo trả tiền**:

| Mã | Rào | Chạm | Vì sao là rào cứng |
|---|---|---|---|
| **R2** | **Danh mục kỹ thuật (DMKT)** | 3 TV (3 CORE) | ⛔ Không QC kỹ thuật **ngoài danh mục đã phê duyệt** — **deep plane · BBL · abs etching**. Vượt phạm vi hoạt động |
| **R3** | **Đúng pháp nhân** — điểm nóng | 8 TV (7 CORE) | ⛔ Site EN không gộp nhiều cơ sở/pháp nhân; không dùng tên "Kangnam" cho dịch vụ ngoài phạm vi |
| **R7** | **Túi ngực · thiết bị · filler** | **9 TV** (6 CORE) | ⛔ Chỉ nêu hãng **thực dùng, có số lưu hành**. Nhiều thứ hai sau R1 |
| **R8** | **KCB cho người nước ngoài** | 4 TV (4 CORE) | 🔴 **Nóng nhất** — xem dưới |

**R8 là rào quan trọng nhất mà gói này từng thiếu.** R2/R3/R7 nói về **câu chữ**; R8 nói về **điều kiện hoạt động** — có được tiếp nhận khách quốc tế hay không.

> Một chiến dịch chạy tốt, landing chấm 90 điểm, mẫu quảng cáo 14/14 — nhưng cơ sở **chưa đủ điều kiện R8** thì **lead đổ về là rủi ro, không phải thành tích.**

**Hai dịch vụ bị chặn tới khi chốt được điều kiện:**
- **Q08 Dental** — chốt **pháp nhân RHM** (Kangnam Dental hay Nha Khoa Paris) trước khi xuất bản bất kỳ nội dung nào *(R3)*.
- **Q09 BBL** — chỉ làm nếu kỹ thuật **thuộc DMKT**, và nội dung phải **nói thật rủi ro thuyên tắc mỡ** *(R2)*. Thủ thuật rủi ro cao nhất ngành.

### Thứ tự quyết định của khách quốc tế — và hệ quả

Bộ GEO làm rõ khách quốc tế hỏi AI **theo thứ tự**:
```
① Vietnam/cơ sở có an toàn & được phép không
      → ② giá USD so với nước nhà/Thái/Hàn
            → ③ chuyến đi thu xếp ra sao, ở bao lâu
                  → ④ MỚI TỚI từng dịch vụ
```
→ **Tầng A là 4 cụm NGANG dịch vụ, không phải trang dịch vụ:** Q10 chọn cơ sở · Q12 an toàn/giấy phép · Q11 giá USD · Q13 logistics. Bốn cụm = **46,9% điểm**, **70% ngân sách EN**, Sóng 1 (90 ngày).
⛔ Làm trang dịch vụ trước 4 trang Tầng A là **đi sai thứ tự** — AI không có gì để trích dẫn khi khách hỏi câu ① ② ③.

### ⚠️ Hai hệ giai đoạn KHÔNG trùng khớp — dùng bảng ánh xạ, đừng đánh số lại

Bộ GEO dùng **6 giai đoạn** (G-S1…G-S6); bộ não dùng **7 chặng** (S1…S7). Hai chỗ lệch:
① **"S2"** ở hai bộ là hai thứ khác nhau — G-S2 là chọn **kỹ thuật**, S2 (ads) là chọn **nước**.
② **Giá**: GEO coi giá là phần của nỗi sợ (G-S3); ads coi giá là chặng hành động (S5). Cả hai đúng cho kênh của mình.

⛔ **Không đánh số lại một hệ theo hệ kia** — file nguồn do team GEO/Content bảo trì. Bảng ánh xạ: `kn-truy-van-geo-qt.md` §2.

### Thay đổi file

```
SYSTEM-PROMPT.md       36.128 → 42.478 ký tự   (+ §15b MODE 5, + 6 rule, + phân biệt GEO)
SYSTEM-PROMPT-NGAN.md   7.961 →  7.967 ký tự   (vẫn dưới 8.000 — xem đánh đổi dưới)
knowledge/              8 → 9 file             (+ kn-truy-van-geo-qt.md, 80 KB)
prompts/                4 → 5 file             (+ prompt-geo-answer.md)
kn-rao-phap-ly-qt.md    + §4b (R2·R3·R7·R8) + 4 dòng "cần xác nhận"
```

**Đánh đổi của bản ngắn:** để nhét MODE 5 và rào **R8** vào 8.000 ký tự, đã **cắt các dòng SPEC** (giới hạn ký tự RSA/Meta · danh sách kênh CTA từng market · token màu · 7 rào tương phản · ô ảnh tạm) — tất cả đều có **đầy đủ trong Knowledge**. Giữ lại các dòng **GATE** (chặn output hoặc gây hại nếu vi phạm). Nguyên tắc: *bản ngắn là bộ cổng chặn, không phải bộ spec.*

### ⚠️ Việc còn treo — thêm 4 mục

Ngoài 15 mục của v1.0:

| # | Việc | Ai | Mức |
|---|---|---|---|
| 16 | 🔴 **R8 — cơ sở + bác sĩ đủ điều kiện KCB cho người nước ngoài**, phiên dịch chuyên môn, hồ sơ song ngữ | Pháp chế + Điều phối QT | 🔴 Chặn mọi chiến dịch quốc tế |
| 17 | **R2 — DMKT từng cơ sở**: deep plane · BBL · abs etching có trong danh mục không | Pháp chế | 🔴 Chặn Q03 · Q09 |
| 18 | **R3 — pháp nhân site EN**, và **nha khoa: Kangnam Dental hay Nha Khoa Paris** | Pháp chế | 🔴 Chặn Q08 |
| 19 | **R7 — số lưu hành** túi ngực · thiết bị · filler thực dùng | BS + Pháp chế | 🟠 Chạm 9 truy vấn |

> Mục 1 của v1.0 (**bảng số ngày ở lại**) giờ chặn **hai** thứ: khối B08 của landing **và** trang `/medical-tourism-guide` của Q13. Đòn bẩy của nó cao hơn trước.

---

## v1.0 — 21/10/2026 · Bản đầu tiên

Gói mới, tách khỏi [`Agent-AdsOptimize-Kangnam`](../../Agent-AdsOptimize-Kangnam/) (nội địa) và kế thừa bộ não của nó + [`Agent-LDP-Kangnam`](../../Agent-LDP-Kangnam/).

**Site phục vụ:** `kangnamaesthetichospital.com` — khác site nội địa (`benhvienthammykangnam.com.vn`).

---

### Cấu trúc

```
SYSTEM-PROMPT.md          36.128 ký tự  (Claude / Gemini)   → v1.1: 42.478
SYSTEM-PROMPT-NGAN.md      7.961 ký tự  (ChatGPT)            → v1.1:  7.967
knowledge/   8 file                                          → v1.1: 9 file
prompts/     4 file                                          → v1.1: 5 file
markets/     schema + 1 ví dụ đã build được
tools/       generator .xlsx, 3 cổng chặn, 14/14 test gate pass
template/    lp-skeleton-en.html + bản lưu trang tham chiếu
doc/         3 file
```

---

### Bảy khác biệt so với gói nội địa

Không phải bản dịch. Bảy thứ dưới đây là **thay đổi logic**, và chúng là lý do gói này tồn tại riêng.

#### ① Chia theo THỊ TRƯỜNG × DỊCH VỤ, không theo ZONE dịch vụ
Gói nội địa: 1 ZONE = 1 nhóm dịch vụ cùng rào cản. Gói QT: **1 bộ = 1 tầng × 1 nhóm market cùng luật quảng cáo × 1 nhóm dịch vụ**.
Vì cùng một ca nâng mũi, khách Campuchia và khách Úc có động cơ, rào cản, ngôn ngữ, giá chấp nhận được **và luật quảng cáo** khác nhau.

**Bốn tầng:** A khu vực · **B kiều bào** · C thị trường phát triển · **D expat tại VN**.
Tầng B và D là hai tầng hay bị bỏ sót nhất:
- **B dễ chốt nhất** (đã tin brand Việt · không cần phiên dịch · **đã có vé**) nhưng tìm bằng **tiếng Việt từ IP nước ngoài** → chiến dịch chỉ có từ khoá tiếng Anh thì không bao giờ gặp họ.
- **D không phải du lịch y tế** — họ đã ở trong nước. Landing nói về đưa đón sân bay là vô nghĩa.

#### ② Rào cản thứ tư: XA
Nội địa có SỢ · NGỜ · NGẠI. QT thêm **XA** — *"bay về rồi ai lo cho tôi"*.

XA là rào cản **cuối cùng**: khách đã vượt ba rào kia rồi mới chạm vào nó, nên mất khách ở đây là **đắt nhất**. Bốn câu của nó, theo thứ tự khách nghĩ: ① ở Việt Nam mấy ngày ② về nhà có vấn đề thì liên hệ ai ③ phải chỉnh sửa thì ai trả chi phí và vé ④ có ai nói được tiếng tôi.

Scorecard landing dành **15 điểm riêng** cho rào cản này. Một trang English rất đẹp, trust rất đầy, nhưng không nói số ngày ở lại và ai lo sau khi về thì **không thể đạt 80** — và đúng như vậy.

#### ③ Phễu 7 chặng, chèn S4 · LÊN KẾ HOẠCH CHUYẾN ĐI
Nội địa dồn ngân sách vào S3 (nỗi sợ). QT phải dồn vào **S3 và S4**.

S4 là chặng khách rụng nhiều mà **không ai đo**, vì nó xảy ra sau khi lead đã vào CRM. Khách đến S4 đã vượt Sợ và Ngờ — họ muốn làm, chỉ đang tính chuyến đi có chạy được không. Từ khoá S4 (`how many days in vietnam after rhinoplasty` · `english speaking plastic surgeon hanoi`) có **cạnh tranh thấp nhất cả phễu**, và **gần như không đối thủ nào làm trang trả lời nó**.

→ Ngân sách **S4 ≥ 15%**, S3 ≥ 10%, tầng B ≥ 15%.

#### ④ Cổng GEO-TARGET — ràng buộc cứng, thay cho cổng TUYẾN
Gói nội địa có bẫy TUYẾN (đại phẫu + tên tỉnh chỉ có viện tỉnh). **Gói QT không có bẫy đó** — site quốc tế chỉ công bố 2 cơ sở, cả hai là tuyến bệnh viện.

Nhưng nó có bẫy riêng, mức độ nghiêm trọng như nhau:

> `plastic surgery hanoi` gõ từ **Sydney** = khách sắp bay, cần số ngày ở lại và bảo hành từ xa.
> `plastic surgery hanoi` gõ từ **Hà Nội** = expat đang sống ở đó, cần địa chỉ và lịch tuần này.
> Một landing, một mẫu QC → **mất cả hai**.

→ Mọi dòng từ khoá khai `market` (người gõ **đang ở đâu**) + `geo_mode`. Tầng D bắt buộc `Presence`.
⛔ Để Google tự chọn (mặc định `Presence or interest`) cho chiến dịch expat → tràn traffic quốc tế, CPL trông rẻ, **không ai đến khám**. **Lỗi này im lặng** — Google Ads không cảnh báo.

Cài ở 4 chỗ: §4 bộ não · tiêu chí ⑦ bảng chấm WIN (0 điểm = loại thẳng) · bước ③ MODE 3 · **cổng GEO-TARGET trong generator**.

#### ⑤ Hai tầng pháp lý cùng lúc
Nội dung chịu **luật Việt Nam** (luôn áp) **và luật nước người xem**.

**AU 🔴 cao nhất** — AHPRA **cấm thẳng testimonial về kết quả lâm sàng**; before–after ràng buộc rất chặt. UK (ASA/CAP) · EU (+**GDPR**) · GCC 🔴 · US 🟠 (FTC).

**Hệ quả thiết kế, không phải hệ quả câu chữ:** landing tầng C **không được dựa vào** before–after và testimonial làm trụ bằng chứng. Phải loại chúng khỏi kế hoạch **trước khi viết**. Trụ bằng chứng thay thế: giấy phép Bộ Y tế → hồ sơ bác sĩ → quy trình an toàn → **International Patient Department** → **quy trình 5 bước cho khách ở xa** → T&C bảo hành.

Đây cũng là lý do khối *"Out of Town Patients"* quan trọng hơn khối testimonial: nó là bằng chứng **được phép dùng ở mọi thị trường**.

#### ⑥ Giá HIỆN, không ẩn
Gói nội địa ẩn giá (dữ liệu động). Gói QT **phải hiện giá** — chênh giá chính là cái hook, khách tầng C vào trang để tìm đúng con số đó.

**Ba dòng bắt buộc đi kèm mọi bảng giá:**
- *The price shown does not include the 10% international service charge.*
- *USD figures are approximate and depend on the exchange rate on the day of payment.*
- *Final cost is confirmed by the doctor after an in-person examination.*

Bỏ dòng đầu là **bom niềm tin**: khách phát hiện ở quầy thanh toán thì mất cả ca và nhận review xấu.
⛔ Không so giá với quốc gia hoặc cơ sở **có tên** — công bố bảng giá đầy đủ, để bảng giá nói thay.

#### ⑦ Đo bằng chi phí/khách ĐẾN KHÁM, không bằng CPL
Phễu 8 bước: `click → lead → phản hồi được → gửi ảnh → báo giá → ĐẶT CỌC → đặt vé → ĐẾN KHÁM`.

⛔ **CPL là chỉ số gây nhầm lẫn nhất của gói này** — lead Campuchia rẻ gấp nhiều lần lead Úc nhưng tỷ lệ đến khám khác hoàn toàn. So CPL giữa hai market là so hai thứ khác nhau.

**Luật độ trễ:** `lead → đến khám` mất **4–12 tuần** (tầng B tới 6 tháng nếu chờ Tết). ⛔ **Không kết luận chiến dịch tầng B/C trong cửa sổ < 8 tuần.** Đây là luật bị phá nhiều nhất: áp lực báo cáo hằng tuần làm team cắt chiến dịch tầng C ở tuần thứ 3 vì *"CPL cao, chưa ra ca"* — trong khi ca của nó đang trên đường, theo nghĩa đúng của từ.

---

### Design System Kangnam International v1.0

Token lấy từ trang production `/top-plastic-surgery-in-vietnam/` (`--primary-color #005F88` · `--second-color #00BAC3`), cộng navy nhận diện `#003C77`, gold `#B08D4F` làm accent sang trọng, và **champagne `#FAF7F2`** làm khối ấm.

**Khác cấu trúc lớn nhất so với gói nội địa:** gói nội địa dựng **thẻ khổ điện thoại `max-width:480px`** căn giữa. Gói QT dùng **responsive full-width `max-width:1140px`**, vì:
- khách tầng C **nghiên cứu trên desktop** (so giá, đọc hồ sơ bác sĩ, mở nhiều tab) rồi mới chuyển sang mobile để nhắn tin;
- bảng giá và bảng so sánh điểm đến **cần chiều ngang**;
- một thẻ 480px trên màn 1440px đọc như trang quảng cáo địa phương, không như một bệnh viện quốc tế.

**Bảy rào tương phản — đã đo, không ước lượng:**

| | Số đo |
|---|---|
| ✅ `--teal #005F88` an toàn mọi cỡ, cả hai chiều | **7,02** AA/AAA |
| ✅ `--teal-900 #00394F` · `--navy #003C77` | 12,37 · 10,98 AAA |
| ⛔ `--teal-400 #00BAC3` không làm chữ trên trắng | **2,38 fail** → chỉ vạch/viền/icon |
| ⛔ `--gold #B08D4F` không làm chữ nhỏ trên trắng | **3,10** → chỉ ≥24px thường hoặc ≥19px/700; nhỏ hơn dùng `--gold-dk #8C6E36` (**4,77 AA**) |
| ⛔ `--cta #E15A01` là màu **nền nút** | trắng trên nó **3,71** → nhãn ≥19px/700; nút nhỏ hơn dùng `--cta-press #C44D00` (**4,76 AA**) |
| ⛔ `--ink-3 #7A8B98` không dùng cho chữ thân | **3,52 fail** → chữ phụ dùng `--ink-2 #4A5C6A` (**6,93 AA**) |
| ✅ Gold trên nền tối | `--gold-lt` trên `--teal-900` = **5,47 AA** · `#FEC465` = **7,83 AAA** |

**"Sang trọng" đến từ ba thứ, không đến từ màu:** ① khoảng trắng lớn (section padding 96px desktop) ② serif hiển thị ở cỡ lớn ③ **gold dùng rất ít**, chỉ vạch mảnh và eyebrow. Dùng nhiều gold làm trang trông **rẻ đi**, không sang hơn.

**Form quốc tế không thể 3 trường** như gói nội địa. Trường quyết định tỷ lệ kết nối là ★ **`preferred contact time + time zone`**: bệnh viện mở 8am–5pm ICT = **5pm–2am ở Los Angeles**. Thiếu trường này thì lead tầng C mất phần lớn ở khâu kết nối, và báo cáo sẽ hiển thị như *"lead chất lượng kém"* trong khi vấn đề là **múi giờ**.

---

### Generator — 3 cổng chặn, 14/14 test pass

`tools/build_keyword_workbook.py` kế thừa generator nội địa, thay cổng TUYẾN bằng:

| Cổng | Chặn gì |
|---|---|
| **CAM** | Từ cấm **tiếng Anh** (`best` · `#1` · `top-rated` · `leading` · `guaranteed` · `permanent` · `painless` · `no scar` · `risk-free` · `cheapest`…) **và tiếng Việt** (tầng B) |
| **CLAIM** | `lifetime warranty` · `board certified` · `VSAPS`/`ASAPS`/`ISAPS`/`AAFPRS` · `cheaper than <quốc gia>` |
| 🆕 **GEO** | Thiếu `market` hoặc `geo_mode` · `geo_mode` không hợp lệ · `market=VN-EXPAT` mà không phải `Presence` · từ khoá có địa danh VN mà thiếu một trong hai trường |
| 🆕 **REGULATED** | `market` thuộc nhóm rủi ro cao (AU·UK·NZ·US·CA·IE·EU·GCC) mà `ghi_chu` chưa khai cách xử lý creative |

> **Cổng CLAIM không quét cột `tu_khoa`, và đó là có chủ ý.** Từ khoá là chữ **khách gõ**, không phải claim của mình: `cheaper than korea` là truy vấn thật và **được phép nhắm** (chặng S2, giá trị cao); điều bị cấm là **viết lại nó thành claim** trong thông điệp. Lỗi này phát hiện khi chạy generator lần đầu trên file ví dụ.

Cũng đã sửa: console Windows mặc định cp1252 làm thông báo lỗi tiếng Việt bị hỏng chữ → force UTF-8 cho stdout/stderr.

---

### 🔴 Ba lỗi phát hiện trên trang tham chiếu production — 21/10/2026

Trang `/top-plastic-surgery-in-vietnam/` là **mẫu style** của gói này, **không phải mẫu nội dung**. Ba lỗi dưới đây có trên bản live và **phải gỡ ngoài repo**:

| # | Lỗi | Nguyên văn | Vì sao nghiêm trọng |
|---|---|---|---|
| ① | **Tên bác sĩ của cơ sở khác** trong FAQ | *"**Dr. Granzow** will be able to provide a good estimate for the length of your procedure during your consultation."* | FAQ **copy từ website một bác sĩ Mỹ khác**. Không có bác sĩ nào tên Granzow ở Kangnam. Khách tầng C tra tên này sẽ thấy ngay → mất toàn bộ niềm tin |
| ② | **Bộ đếm hỏng** | *"Trusted by **0+** clients"* | Khối social proof đang hiện số 0. Tệ hơn là không có khối nào |
| ③ | **Cam kết kết quả vĩnh viễn** | *"Is rhinoplasty a permanent procedure? **Yes**, … the results are permanent."* | Cam kết kết quả y khoa — vi phạm luật VN, rủi ro FTC/ASA/AHPRA |

Thêm hai claim cần xử lý: **"Lifetime warranty"** (không có T&C công bố) và **"The Leading / Top-Rated Aesthetic Hospital in Vietnam"** (superlative, rủi ro ở AU/UK).

Bộ não đã cài luật **không sao chép** bốn thứ này từ trang tham chiếu (§18 rule 20).

---

### ⚠️ Việc còn treo — phải làm ngoài repo

| # | Việc | Ai | Mức |
|---|---|---|---|
| 1 | **Điền bảng số ngày ở lại Việt Nam** từng dịch vụ (`kn-thi-truong-quoc-te.md` §8 — hiện toàn bộ là `[CHỜ CẬP NHẬT]`) | Khoa Chuyên môn | 🔴 **Đòn bẩy cao nhất của cả gói.** Mọi landing tầng A/B/C đều cần nó. Không có nó thì khách không đặt được vé, và không đặt vé thì lead không bao giờ thành ca |
| 2 | **T&C bảo hành / chỉnh sửa** — phạm vi · thời hạn · loại trừ · ai trả chi phí bay | Pháp chế | 🔴 Tới khi có, không được dùng chữ *"lifetime"* |
| 3 | **Chốt một dòng claim hội–hiệp hội dùng chung cho hai site** — site quốc tế đang hiển thị VSAPS/ASPS/ISAPS/AAFPRS ở mức thương hiệu, gói nội địa cấm thẳng | Pháp chế | 🔴 Hai site đang nói hai điều khác nhau về cùng một đội ngũ |
| 4 | **Gỡ 3 lỗi trên trang tham chiếu** (Dr. Granzow · `0+` · *results are permanent*) | Marketing + Pháp chế | 🔴 Đang hiển thị trên bản live |
| 5 | **Số CCHN từng bác sĩ** — site quốc tế công bố bằng cấp nhưng không công bố số CCHN | Pháp chế | 🟠 Chưa có thì không nêu claim tay nghề ở mức cá nhân |
| 6 | **Privacy notice đạt GDPR/UK GDPR** + thông báo chuyển dữ liệu sang Việt Nam | Pháp chế | 🔴 Nhắm EU/UK mà thiếu → **không bật chiến dịch** |
| 7 | Rà quảng cáo theo thị trường đích: AU (AHPRA) · UK (ASA/CAP) · US (FTC) · GCC | Pháp chế thị trường | 🔴 |
| 8 | **Muslim-Friendly Care gồm những gì** — halal? nhân viên nữ? phòng cầu nguyện? | Bộ phận quốc tế | 🟠 Claim vô nghĩa nếu không khai cụ thể |
| 9 | Hỗ trợ visa / thư mời — có hay không | Bộ phận quốc tế | 🟠 Câu hỏi thường gặp của tầng A |
| 10 | **Phương thức thanh toán quốc tế + mức đặt cọc** | Tài chính | 🔴 Rào cản chốt thật — khách không đặt vé khi chưa biết |
| 11 | Phiên dịch: ngôn ngữ nào · có tính phí không · kéo dài bao lâu sau khi về | Bộ phận quốc tế | 🟠 Là câu 4 của rào cản XA |
| 12 | **Chốt cặp font** — gói QT đề xuất Cormorant Garamond + Inter cho register "sạch, sang trọng"; production đang chạy **Roboto** | Brand | 🟡 Chưa chốt thì dùng Inter cho cả display (weight 600) và **nói rõ đang dùng bản dự phòng** |
| 13 | Ảnh thật có **văn bản đồng ý phạm vi quốc tế** — đồng ý dùng ở VN **không** tự động cho phép dùng ở Úc hay EU | Pháp chế | 🟠 |
| 14 | Bản Khmer / Arabic cho tầng A và GCC — cần người bản ngữ rà, ⛔ không máy dịch | Bộ phận quốc tế | 🟡 |
| 15 | Ba tag CRM `market` · `tier` · `stage` phải có từ Pha 1 | Vận hành + CRM | 🔴 Thiếu một tag là lead mù, và Pha 2 không làm được |

---

### Ràng buộc kỹ thuật cần biết khi sửa

- **Khoá JSON gốc vẫn tên `zone`** để dùng chung generator với các gói anh em. Trong gói QT nó mô tả **một bộ thị trường × dịch vụ**, và có thêm 4 trường: `markets` · `tang` · `ngon_ngu` · `rui_ro_qc`.
- **Tên chiến dịch là khoá nối** sang sheet 2 (`COUNTIF`) và sheet 5 (tham chiếu ô). Sửa tên ở một nơi phải sửa cả hai.
- `hanh_trinh` phải đúng **7 phần tử** (S1–S7). Gói nội địa là 6.
- `phieu` gom phễu 8 bước về 5 mốc: `click_lead` · `lead_lich` (= lead→**đặt cọc**) · `show_up` (= đặt cọc→**đến khám**) · `chot`. Đổi nghĩa các khoá này sẽ làm lệch mọi công thức sheet 1 và sheet 5.
- Version ghi trong header từng file, **không gắn version vào tên file**.
