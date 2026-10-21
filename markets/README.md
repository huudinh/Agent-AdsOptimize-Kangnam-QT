# MARKET CONFIG — schema file JSON sinh bộ từ khoá

Mỗi **bộ thị trường × dịch vụ** = **1 file JSON** trong thư mục này → **1 file `.xlsx` 5 sheet** trong `out/`.

> Gói nội địa chia theo **ZONE dịch vụ** (`zones/mui.json`). Gói QT chia theo **THỊ TRƯỜNG × DỊCH VỤ**, vì cùng một ca nâng mũi thì khách Campuchia và khách Úc có **động cơ, rào cản, ngôn ngữ, giá chấp nhận được và luật quảng cáo** khác nhau.

```bash
pip install openpyxl
python tools/build_keyword_workbook.py markets/rhinoplasty-tier-c-au.json
python tools/build_keyword_workbook.py "markets/*.json" -o out/
```

**Ví dụ hoàn chỉnh đã build được:** [`rhinoplasty-tier-c-au.json`](rhinoplasty-tier-c-au.json) — 5 chân dung · 6 chiến dịch · 6 landing · 26 từ khoá · phễu 7 chặng. Dùng để đối chiếu khuôn.

> ⚠️ Khoá gốc vẫn tên là `zone` để dùng chung generator với các gói anh em. Trong gói QT, `zone` **mô tả một bộ thị trường × dịch vụ**, và có thêm 4 trường QT: `markets` · `tang` · `ngon_ngu` · `rui_ro_qc`.

---

## Trật tự bắt buộc khi điền — đây chính là phương pháp luận

Điền **đúng thứ tự này**. Đảo thứ tự là quay về cách làm cũ (gom từ khoá trước, gán người sau):

```
zone → chan_dung → hanh_trinh → chien_dich → landing → tu_khoa → phu_dinh → nguong/lo_trinh
 ①       ②            ③            ④           ⑤          ⑥          ⑦            ⑧
```

① bộ này là **thị trường nào × dịch vụ nào** · ② **ai** mua · ③ họ đi qua **chặng nào (S1–S7)** · ④ mỗi chặng cần **chiến dịch** gì · ⑤ mỗi chiến dịch đổ về **trang** nào · ⑥ người đó **gõ gì**, **từ đâu** · ⑦ chặn và điều hướng truy vấn lệch · ⑧ ngưỡng vận hành.

---

## 17 khối bắt buộc

### ① `zone` — định danh bộ

| Khoá | Kiểu | Ghi chú |
|---|---|---|
| `ten` | string | Tên hiển thị, vd `"Rhinoplasty · Tier C · Úc (AU)"` |
| `ma` | string | slug nội bộ |
| `nganh` | string | `"Aesthetic · Medical tourism"` |
| `ten_file` | string | Tên file xuất, **không kèm `.xlsx`** |
| `ds_phu_dinh_chung` | string | Tên danh sách phủ định cấp tài khoản |
| `ngan_sach_thang` | number | VND. Ô đầu vào (nền vàng) trên sheet 1 |
| `muc_tieu` | string | 1 câu, nêu **thứ tự ưu tiên chỉ số** — đặt *chi phí/khách đến khám* lên trước CPL |
| ★ `markets` | string | Các mã market bộ này phục vụ, vd `"AU (+ NZ ở Pha 2)"` |
| ★ `tang` | string | `"A · khu vực"` / `"B · kiều bào"` / `"C · thị trường phát triển"` / `"D · expat tại VN"` |
| ★ `ngon_ngu` | string | `"English"` · `"Tiếng Việt"` · `"English + Khmer"` |
| ★ `rui_ro_qc` | string | Mức rủi ro quảng cáo + cơ quan phải tra, vd `"🔴 CAO — AHPRA cấm testimonial kết quả lâm sàng"` |

★ = trường riêng của gói QT, in ra đầu sheet 1.

### ② `chan_dung[]` — chân dung KH

Khuyến nghị **4–7 chân dung**.

| Khoá | Ghi chú |
|---|---|
| `ma` | `CD1`, `CD2`… — cột `chan_dung` của từ khoá tham chiếu mã này |
| `ten` | Ai, bao nhiêu tuổi, **ở đâu**, đang ở tình huống nào |
| `insight` | **Nỗi đau thật**, viết bằng lời khách. Phải ghi rõ: người gõ có phải người điều trị không · ★ **market + ngôn ngữ + múi giờ** · ★ **ràng buộc chuyến đi** (bay được mấy ngày · đi cùng ai · cửa sổ thời gian · cần visa không) |
| `rao_can` | `SỢ` / `NGỜ` / `NGẠI` / **`XA`** + một câu giải thích |
| `chang_vao` | Chặng họ bước vào phễu, vd `S2-S3` · `S4` |
| `chien_dich` | Các chiến dịch phục vụ chân dung này |
| `gia_tri_ca` | `Thấp` / `Trung bình` / `Cao` / `Rất cao` |

> **Tách hẳn hai nhóm, như gói nội địa:** ① **khách lần đầu** vs **khách đi sửa lại** (nhóm sửa lại đã mất niềm tin vào cả ngành, cần bằng chứng khác và trả được CPC cao nhất) · ② ★ **kiều bào** vs **khách bản địa cùng nước** (kiều bào tìm bằng **tiếng Việt từ IP nước ngoài**, đã tin thương hiệu Việt, và **đã có vé máy bay**).

### ③ `hanh_trinh[]` — **7 chặng S1→S7**

Đúng **7 phần tử**, theo thứ tự. Gói nội địa có 6; gói QT chèn **S4 · LÊN KẾ HOẠCH CHUYẾN ĐI**.

Khoá: `chang`, `chan_dung`, `tam_ly`, `rao_can`, `chien_dich`, `tu_khoa`, `thong_diep`, `bang_chung`, `lp`, `chuyen_doi`, `sau_lead`, `kpi`, `tiep_theo`.

| Chặng | Dấu hiệu trong từ khoá (EN) | Lưu ý |
|---|---|---|
| S1 NHẬN BIẾT | `what is` · `should I` | Không chạy landing chốt |
| **S2 SO SÁNH ĐIỂM ĐẾN** | `in vietnam` · `vs thailand` · `is vietnam safe` · `cheaper than korea` | Chọn **nước**, chưa chọn bệnh viện → ⛔ không bán Kangnam ở trang này |
| **S3 CÂN NHẮC & NỖI SỢ** | `safe` · `pain` · `review` · `revision` · `gone wrong` | Gọi tên nỗi lo rồi **trả lời ngay** |
| **S4 KẾ HOẠCH CHUYẾN ĐI ★★** | `how many days` · `before flying` · `english speaking` · `visa` · `interpreter` · `airport pickup` | **Chặng quyết định của gói QT** — cạnh tranh thấp nhất, gần như không đối thủ nào làm trang trả lời nó |
| S5 THỰC HIỆN | `cost` · `price` · `package` · `book` | |
| S6 HẬU PHẪU TỪ XA | `swelling after` · `when can I fly` · `aftercare` | Không chạy ads; vẫn cần trang cho CRM/WhatsApp |
| S7 GẮN BÓ | `other procedures` · `second trip` | Xin testimonial **phi lâm sàng** |

### ④ `chien_dich[]` + ⑤ `cap_uu_tien[]`

`chien_dich[]`: `ten`, `uu_tien` (khớp một `cap` trong `cap_uu_tien`), `vai_tro`, `ty_trong` (**tổng đúng 1.0**), `diem {y_dinh, gia_tri, kha_nang_chot}` (1–5), `bid`, `chi_tieu`.

**Quy ước tên — khoá nối sang sheet 2 (`COUNTIF`) và sheet 5:**
```
KN-QT | <tầng> | <market> | <chặng> | <cụm truy vấn>

KN-QT | C | AU | S4 | Trip Planning
KN-QT | B | VN-DIASPORA-AU | S4 | Lịch trình về nước
KN-QT | D | VN-EXPAT | S5 | English-speaking booking
```
Sửa tên ở một nơi phải sửa cả hai.

**Ngân sách tối thiểu:** `S3 ≥ 10%` · **`S4 ≥ 15%`** · `tầng B ≥ 15%`. Chia theo **ý định mua × giá trị ca**, ⛔ **không theo lượng tìm kiếm**.

`cap_uu_tien[]`: `cap` (`P1`…`P4`), `quy_tac`.

### ⑥ `landing[]`

`ma_ten` dạng **`LPx: tên trang`** — generator cắt phần trước dấu `:` làm mã đối chiếu với cột `lp`.

| Khoá | Ghi chú |
|---|---|
| `loai` | Khung: `L1 - Destination` · `L2 - Answer-first` · `L3 - Trip-plan` · `L4 - Price & Book` · `L5 - Expat` · `L6 - Diaspora`. Quy tắc chọn: `kn-khung-landing-qt.md` §1 |
| `chang` | Chặng trang này phục vụ, vd `S4` |
| `chan_dung` | Mã `CDx`, có thể nhiều mã |
| `rao_can` | Rào cản **trang này phải gỡ** — không gỡ chung chung cả bốn |
| `noi_dung` | Nội dung bắt buộc phải có. **Trang tầng A/B/C phải ghi rõ có khối B08 (số ngày ở lại) và B09 (ai lo sau khi về)** |
| `cta` | CTA chính |
| `micro` | Micro-conversion đặt **trước** form |

> 4 trường `loai` / `chang` / `chan_dung` / `rao_can` là đầu vào trực tiếp của [`prompts/prompt-build-landing-page.md`](../prompts/prompt-build-landing-page.md). Thiếu thì Agent phải đoán khung.

### ⑦ `tu_khoa[]` — 1 dòng = 1 từ khoá × 1 kiểu khớp

| Khoá | Ghi chú |
|---|---|
| `chien_dich` | Phải khớp **chính xác** một `chien_dich[].ten` |
| `nhom_qc` | Nhóm quảng cáo |
| `tu_khoa` | Viết thường, không dấu ngoặc |
| `khop` | `Exact` / `Phrase`. **`Broad` bị generator chặn** |
| ★ **`market`** | **Người gõ ĐANG Ở ĐÂU** — không phải thành phố trong từ khoá. **Generator chặn nếu thiếu** |
| ★ **`geo_mode`** | `Presence` hoặc `Presence+Interest`. **Generator chặn nếu thiếu, hoặc nếu `market=VN-EXPAT` mà không phải `Presence`** |
| `uu_tien` | `P1`…`P4` |
| `chang` | `S1`…`S7` |
| `chan_dung` | Mã `CDx` |
| `rao_can` | `SỢ` / `NGỜ` / `NGẠI` / `XA` |
| `canh_tranh` | `Thấp` / `Trung bình` / `Cao` / `Rất cao` |
| `win` | Điểm cổng WIN dạng `3/4` — **gói QT có 4 tiêu chí, qua 3/4** |
| `lp` | Mã `LPx` |
| `thong_diep` | Thông điệp + CTA. **Bị quét từ cấm và quét claim đã gỡ** |
| `volume`, `cpc` | **Để TRỐNG** — Keyword Planner, **chạy riêng theo từng market** |
| `ghi_chu` | Điều kiện bật/tắt · quy tắc cắt · **và cách xử lý creative nếu market thuộc nhóm rủi ro cao** (xem cổng REGULATED) |

**Mã market:**
```
AU · US · CA · UK · NZ · DE · CZ · IE
AE · SA · KW · QA                        (GCC)
KH · LA · MM · ID · PH · MY · IN · SG · TH
JP · KR · TW
VN-EXPAT                                  (tầng D — người nước ngoài đang ở VN)
VN-DIASPORA-<mã nước>                     (tầng B — vd VN-DIASPORA-AU)
```

**Cổng WIN 4 tiêu chí** (`knowledge/kn-cong-win-tu-khoa-qt.md`) — ① sát chuyển đổi · ② cạnh tranh ít · ③ giá trị ca lớn · ④ **ý chí đi lại**:
- `4/4`, `3/4` → được sản xuất nội dung riêng.
- `2/4` hoặc thấp hơn → **giữ để hứng volume** nhưng **không viết nội dung riêng**, để P3/P4, ghi rõ quy tắc cắt trong `ghi_chu`.
- Dịch vụ giá thấp (mí · da liễu · spa) cho tầng A/B/C → tối đa `2/4`, `ghi_chu` ghi *"combo/cross-sell only"*.

### ⑧ `phu_dinh_chung[]` / `phu_dinh_cheo[]` / `quy_trinh_phu_dinh[]`

Khoá: `nhom`, `tu`, `khop`, `ap_dung`, `ly_do`.

> **Phủ định chéo không phải để loại khách — là để ĐIỀU HƯỚNG.** Trước khi thêm, hỏi: truy vấn này thuộc **chân dung nào, chặng nào, market nào?** Có chân dung phù hợp → đẩy sang đúng chiến dịch. Không có → mới loại.

**Phủ định bắt buộc của gói QT:** tên nước điểm đến khác (`korea` `thailand` `turkey` `istanbul` `mexico`) · `free` · `jobs` · `salary` · `course` · `training` · `insurance covered`.
⚠️ **Miễn trừ nhóm so sánh:** `vietnam vs korea` · `cheaper than korea` là người **đang so sánh, chưa quyết** → giữ lại, chặng S2, giá trị cao. Phân biệt bằng `vs` · `compare` · `or` · `cheaper than` · `instead of`.

### ⑨ Còn lại

`phieu` (6 ô mô hình phễu + `ghi_chu`), `nguyen_tac[]`, `nguong[]` (`moc` = `cpl` hoặc `ca_chot`), `lo_trinh[]` (3 pha), `quy_tac_canh_tranh[]`, `ab_test[]`, `rui_ro[]`, `hook_format[]` (tuỳ chọn).

**`phieu` của gói QT gom phễu 8 bước về 5 mốc đo được:**
```
click → lead → ĐẶT CỌC → ĐẾN KHÁM → ca chốt
```
| Khoá | Nghĩa trong gói QT |
|---|---|
| `cpc` | CPC trung bình |
| `click_lead` | click → lead |
| `lead_lich` | **lead → ĐẶT CỌC** (đã tính cả khâu phản hồi được) |
| `show_up` | **đặt cọc → ĐẾN KHÁM** |
| `chot` | đến khám → ca chốt |
| `gia_tri_ca` | giá trị ca trung bình |

Sheet 1 xuất thêm dòng **Chi phí / khách ĐẾN KHÁM** — **chỉ số bắc đẩu** của gói này. ⛔ Đánh giá chiến dịch bằng cột đó, **không bằng CPL**: so CPL giữa hai market là so hai thứ khác nhau.

---

## Cổng kiểm tra

Generator dừng và in lỗi nếu:

- thiếu bất kỳ khoá nào trong 17 khối bắt buộc;
- `sum(ty_trong) ≠ 1.0`;
- từ khoá trỏ tới `chien_dich` / `lp` / `chan_dung` chưa khai báo;
- chiến dịch dùng `uu_tien` chưa có trong `cap_uu_tien`;
- có `khop: "Broad"`;
- trùng cặp (từ khoá × kiểu khớp);
- **cổng CAM** — `thong_diep` chứa từ cấm, bản **tiếng Anh** (`best` · `#1` · `top-rated` · `leading` · `guaranteed` · `permanent` · `painless` · `no scar` · `risk-free` · `cheapest` · `100% success`…) **và tiếng Việt** (cho tầng B);
- **cổng CLAIM** — còn `lifetime warranty` · `board certified` · `VSAPS`/`ASAPS`/`ISAPS`/`AAFPRS` · `cheaper than <quốc gia>` trong `thong_diep` · `nhom_qc` · `hanh_trinh` · `landing` · tên chiến dịch;
- 🆕 **cổng GEO-TARGET** — dòng từ khoá thiếu `market` hoặc `geo_mode`; `geo_mode` không hợp lệ; `market=VN-EXPAT` mà `geo_mode ≠ Presence`; hoặc từ khoá có địa danh Việt Nam mà thiếu một trong hai trường;
- 🆕 **cổng REGULATED** — dòng từ khoá có `market` thuộc nhóm rủi ro cao (**AU · UK · NZ · US · CA · IE · EU · GCC**) mà `ghi_chu` **chưa khai cách xử lý creative**.

### Vì sao có cổng GEO-TARGET

Cùng một chuỗi ký tự là **hai người hoàn toàn khác nhau**:

| Từ khoá | `market` | `geo_mode` | Là ai | Landing |
|---|---|---|---|---|
| `english speaking plastic surgeon hanoi` | `AU` | `Presence+Interest` | Khách Úc sắp bay sang | **L3 Trip-plan** |
| `english speaking plastic surgeon hanoi` | `VN-EXPAT` | **`Presence`** | Expat đang sống ở Hà Nội | **L5 Expat** — ⛔ không có khối du lịch |

→ **Cùng chuỗi, hai dòng từ khoá, hai chiến dịch, hai landing.** Đây là cách đúng, không phải trùng lặp.

⛔ Để Google tự chọn kiểu nhắm (mặc định `Presence or interest`) cho chiến dịch expat → tràn traffic quốc tế, CPL trông rẻ, **không ai đến khám**. Lỗi này **im lặng** — Google Ads không cảnh báo.

### Vì sao có cổng REGULATED

Nội dung chịu **hai hệ luật cùng lúc**: luật Việt Nam (luôn áp) **và luật nước người xem**. AHPRA (Úc) **cấm thẳng testimonial về kết quả lâm sàng**; before–after bị ràng buộc rất chặt ở AU/UK/EU/GCC.

→ `ghi_chu` của dòng từ khoá nhắm market rủi ro cao phải nêu **một trong**: landing không dùng before–after · không dùng testimonial kết quả lâm sàng · chỉ dùng testimonial phi lâm sàng · đang chờ Pháp chế thị trường duyệt. Generator nhận ra đã xử lý khi `ghi_chu` chứa một trong các cụm: *no before-after · không before-after · no testimonial · không testimonial · non-clinical · phi lâm sàng · AHPRA · ASA · CAP Code · FTC · GDPR · Pháp chế · legal review · chờ duyệt*.

```json
{ "tu_khoa": "rhinoplasty vietnam reviews", "khop": "Phrase",
  "market": "AU", "geo_mode": "Presence+Interest",
  "ghi_chu": "⚠️ Từ khoá review nhưng market AU KHÔNG dùng được testimonial kết quả lâm sàng (AHPRA). Landing trả lời bằng giấy phép + hồ sơ bác sĩ + testimonial phi lâm sàng." }
```

### Cổng CLAIM **không** quét cột `tu_khoa` — và đó là có chủ ý

Từ khoá là chữ **khách gõ**, không phải claim của mình. `cheaper than korea` là truy vấn thật và **được phép nhắm** (chặng S2, giá trị cao); điều bị cấm là **viết lại nó thành claim** trong `thong_diep`. Vì vậy cổng CLAIM chỉ quét những gì chúng ta viết: `thong_diep` · `nhom_qc` · `hanh_trinh` · `landing` · tên chiến dịch.

**Ba cổng này chặn lỗi cấu trúc, KHÔNG thay người duyệt.** Mọi mẫu quảng cáo và landing vẫn phải qua Pháp chế VN **và** Pháp chế thị trường đích.

---

## Sau khi build

1. Mở file trong `out/`, điền 2 cột Keyword Planner (`volume`, `cpc`) — **chạy Planner riêng cho từng market**.
2. Thay các ô **nền vàng chữ xanh** ở sheet 1 và sheet 5 bằng số thực từ CRM.
3. Giá là **dữ liệu động** — lấy tại `/price-list/` **ở thời điểm chạy**, và luôn kèm 3 dòng bắt buộc.
4. Sửa nội dung thì sửa **file JSON rồi build lại**, đừng sửa thẳng `.xlsx` — lần build sau sẽ ghi đè.
5. Điền bảng **số ngày ở lại** (`kn-thi-truong-quoc-te.md` §8) — việc có đòn bẩy cao nhất trong cả gói.
