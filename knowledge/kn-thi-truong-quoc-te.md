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
