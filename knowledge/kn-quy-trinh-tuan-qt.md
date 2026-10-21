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
