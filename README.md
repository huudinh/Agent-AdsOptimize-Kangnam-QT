# 🌏 ADS OPTIMIZE — KANGNAM QUỐC TẾ (KN-QT)

> Version 1.1 · AI **nghiên cứu bộ từ khoá · sinh mẫu quảng cáo tiếng Anh · dựng landing page · sản xuất nội dung để AI trích dẫn (GEO)** cho khách quốc tế của **Kangnam Korean Aesthetic Hospital** — làm theo chỉ số, theo **tầng thị trường**, và theo **luật quảng cáo của nước người xem**.

Theo công thức HCI **R·M·K·W·O**. Kiến trúc **BRAIN brand-neutral** ([`SYSTEM-PROMPT.md`](SYSTEM-PROMPT.md)) + **MODULE thương hiệu tách riêng** ([`knowledge/kn-ho-so-thuong-hieu-qt.md`](knowledge/kn-ho-so-thuong-hieu-qt.md)) → đổi brand chỉ cần thay module.

**Site phục vụ:** <https://kangnamaesthetichospital.com/> — khác site nội địa.

Agent anh em: [`Agent-AdsOptimize-Kangnam`](../Agent-AdsOptimize-Kangnam/) (nội địa) · [`Agent-LDP-Kangnam`](../Agent-LDP-Kangnam/) (landing nội địa).

---

## Ba đầu ra lõi + hai mode kế thừa/mở rộng

| Mode | Làm gì | Input tối thiểu | Đầu ra |
|---|---|---|---|
| **1 · KEYWORD-RESEARCH** | Từ 1 **thị trường × dịch vụ** → bộ từ khoá theo tầng → chân dung → hành trình S1–S7 | **market** + dịch vụ + ngân sách | **file `.xlsx` 5 sheet** + báo cáo + danh sách `[PENDING]` |
| **2 · WIN-AD** | Từ bộ từ khoá → mẫu quảng cáo tiếng Anh | từ khoá + **market** + dịch vụ | 15 headline + 4 description + 3–5 biến thể Meta + bảng chấm 14 điểm |
| **3 · LDP-BUILD** | Từ cụm từ khoá → landing khung L1–L6 | cụm từ khoá + **market** + dịch vụ | copy-deck 14 khối, hoặc **HTML single-file** + bảng kê ảnh |
| **4 · OPTIMIZE** *(kế thừa)* | Đọc Ads + GA4 + CRM → chẩn đoán | số liệu **cắt theo market** | điểm nghẽn theo phễu 8 bước + 4 quyết định |
| **5 · GEO-ANSWER** ★ | Nội dung EN để **AI trích dẫn** Kangnam | **cụm Q01–Q15** | nội dung EN theo trang đích + prompt đo **Share of Voice** |

⛔ **Thiếu `market` thì không chạy mode nào.** Không biết người xem ở đâu thì không biết luật nào áp, viết ngôn ngữ nào, gắn kênh nào.

---

## Bảy thứ khác hẳn gói nội địa

Gói này **không phải bản dịch** của gói nội địa. Bảy thứ dưới đây là thay đổi logic.

### ① Chia theo THỊ TRƯỜNG × DỊCH VỤ, không theo ZONE dịch vụ

| Tầng | Ai | Động cơ | Rào cản nặng nhất | Ngôn ngữ |
|---|---|---|---|---|
| **A · Khu vực** | KH · LA · MM · ID · PH · MY · IN | Gần + rẻ hơn Thái/Hàn | **NGỜ** | English · Khmer · Bahasa |
| **B · Kiều bào** | Việt kiều US · AU · CA · DE · JP · KR | Về thăm nhà **+** làm thẩm mỹ cùng chuyến | **XA** + NGẠI | **Tiếng Việt** |
| **C · Phát triển** | AU · US · UK · NZ · CA · GCC | Chênh giá 60–80% | **SỢ** + **XA** | English (+Arabic) |
| **D · Expat tại VN** | Người nước ngoài sống ở HN · TP.HCM | Tiện + cần bác sĩ nói tiếng Anh | **NGỜ** (giao tiếp) | English |

**Hai tầng hay bị bỏ sót, và đó là sai lầm đắt nhất:**

- **Tầng B là tầng dễ chốt nhất** — đã tin thương hiệu Việt, nói được tiếng Việt (không cần phiên dịch, chi phí phục vụ thấp nhất), và **đã có vé máy bay** vì lý do khác (Tết · hè · cưới hỏi). Nhưng họ tìm bằng **tiếng Việt từ IP nước ngoài** → chiến dịch chỉ có từ khoá tiếng Anh thì **không bao giờ gặp họ**. Ngân sách tối thiểu **15%**.
- **Tầng D không phải du lịch y tế** — họ đã ở trong nước. Landing nói về đưa đón sân bay và khách sạn là vô nghĩa với người đang sống ở Hà Nội.

### ② Rào cản thứ tư: **XA**

Nội địa có **SỢ · NGỜ · NGẠI**. Quốc tế thêm **XA** — *"bay về rồi ai lo cho tôi"*.

XA là rào cản **cuối cùng**: khách đã vượt ba rào kia rồi mới chạm vào nó, nên **mất khách ở đây là đắt nhất** — họ đã đọc hết trang, đã so giá, đã tin bác sĩ.

**Bốn câu của rào cản XA, theo thứ tự khách nghĩ:**

| # | Khách nghĩ | Trang phải trả lời bằng |
|---|---|---|
| 1 | *"Tôi phải ở Việt Nam bao nhiêu ngày?"* | **Một con số khoảng** + mốc nào (cắt chỉ · tái khám cuối · được phép bay) |
| 2 | *"Về nhà có vấn đề thì liên hệ ai?"* | Tên bộ phận · kênh · ngôn ngữ · **trong bao lâu** |
| 3 | *"Phải chỉnh sửa thì ai trả chi phí và vé?"* | **T&C bảo hành bằng văn bản** |
| 4 | *"Có ai nói được tiếng tôi, cả lúc mổ và sau khi về?"* | Phiên dịch: ngôn ngữ nào · tính phí không · bao lâu |

> **Phép thử trước khi xuất bất kỳ landing nào:**
> *"Đọc trang này xong, khách có đủ thông tin để mở app hàng không và chọn ngày bay chưa?"*
> Chưa → trang chưa xong.

### ③ Phễu 7 chặng — chèn **S4 · LÊN KẾ HOẠCH CHUYẾN ĐI**

| Chặng | Dấu hiệu từ khoá (EN) | Rào cản | Landing |
|---|---|---|---|
| S1 NHẬN BIẾT | `what is` · `should I` | — | ❌ Không chạy landing chốt |
| **S2 SO SÁNH ĐIỂM ĐẾN ★** | `in vietnam` · `vs thailand` · `is vietnam safe` | NGỜ | **L1 Destination** |
| **S3 CÂN NHẮC & NỖI SỢ ★** | `safe` · `pain` · `review` · `revision` | **SỢ** | **L2 Answer-first** |
| **S4 KẾ HOẠCH CHUYẾN ĐI ★★** | `how many days` · `before flying` · `english speaking` · `visa` · `interpreter` | **XA** | **L3 Trip-plan** |
| S5 THỰC HIỆN | `cost` · `price` · `book` | NGẠI | **L4 Price & Book** |
| S6 HẬU PHẪU TỪ XA ★ | `swelling after` · `when can I fly` | XA | Trang CRM — ❌ không ads |
| S7 GẮN BÓ | `other procedures` | — | L4 dịch vụ mới |

**S4 là chặng quyết định của gói này, và là chặng bị bỏ ngân sách.** Khách đến S4 **đã vượt qua cả Sợ và Ngờ** — họ muốn làm, chỉ đang tính chuyến đi có chạy được không. Từ khoá S4 có **cạnh tranh thấp nhất trong cả phễu** (đối thủ đổ tiền vào từ khoá giá), và **gần như không đối thủ nào làm trang trả lời nó**.

→ **Ngân sách: S4 ≥ 15% · S3 ≥ 10% · tầng B ≥ 15%.** Chia theo **ý định mua × giá trị ca**, ⛔ không theo lượng tìm kiếm.

### ④ ⚠️ CỔNG GEO — ràng buộc cứng, thay cho cổng TUYẾN

Gói nội địa có bẫy TUYẾN (đại phẫu + tên tỉnh chỉ có viện tỉnh). **Gói QT không có bẫy đó** — site quốc tế chỉ công bố **2 cơ sở, cả hai là tuyến bệnh viện** (Hanoi 190 Trường Chinh · HCMC 666 CMT8), nên mời đại phẫu là hợp lệ ở cả hai.
⛔ Nhưng **không giới thiệu 5 viện thẩm mỹ tỉnh** cho khách quốc tế — các cơ sở đó không làm đại phẫu.

Thay vào đó, gói QT có bẫy riêng, mức độ nghiêm trọng như nhau:

> `plastic surgery hanoi` gõ từ **Sydney** = khách tầng C sắp bay sang → cần giá · **số ngày ở lại** · bảo hành từ xa.
> `plastic surgery hanoi` gõ từ **Hà Nội** = expat tầng D đang sống ở đó → cần địa chỉ · bác sĩ nói tiếng Anh · lịch tuần này.
> **Một landing, một mẫu quảng cáo → mất cả hai.**

| Từ khoá | `market` | `geo_mode` | Landing |
|---|---|---|---|
| `english speaking plastic surgeon hanoi` | `AU` | `Presence+Interest` | **L3 Trip-plan** |
| `english speaking plastic surgeon hanoi` | `VN-EXPAT` | **`Presence`** | **L5 Expat** — ⛔ không có khối du lịch |

**Cùng chuỗi ký tự, hai dòng từ khoá, hai chiến dịch, hai landing.** Đây là cách đúng, không phải trùng lặp.

⛔ **Để Google tự chọn kiểu nhắm** (mặc định `Presence or interest`) cho chiến dịch expat → tràn traffic quốc tế, CPL trông rẻ mà **không ai đến khám**. **Lỗi này im lặng** — Google Ads không cảnh báo.

Cài ở **4 chỗ**: §4 bộ não · tiêu chí ⑦ bảng chấm WIN (0 điểm → loại thẳng) · bước ③ MODE 3 · **cổng GEO-TARGET trong generator**.

### ⑤ ⚠️ HAI TẦNG PHÁP LÝ cùng lúc

| Tầng | Áp vì | Luôn áp? |
|---|---|---|
| ① **Luật Việt Nam** | Cơ sở ở VN, dịch vụ là KCB. Cần **giấy xác nhận nội dung quảng cáo** | ✅ **Luôn**, bất kể khách ở đâu |
| ② **Luật nước người xem** | Nền tảng áp policy theo **vị trí người nhìn thấy quảng cáo** | ✅ Theo từng market |

| Thị trường | Cơ quan / bộ quy tắc | Điểm nóng | Mức |
|---|---|---|---|
| **Úc** | **AHPRA** · TGA | **Cấm testimonial về kết quả lâm sàng**; before–after rất chặt | 🔴 **Cao nhất** |
| UK | ASA / CAP Code · GMC | Không QC thuốc kê đơn; mọi claim cần bằng chứng | 🔴 |
| EU/EEA | luật từng nước + **GDPR** | Dữ liệu sức khoẻ = special category; phải nêu **chuyển dữ liệu sang VN** | 🔴 |
| GCC | cơ quan y tế từng nước | Cần giấy phép QC y tế riêng | 🔴 |
| Mỹ | FTC | Claim phải có cơ sở; disclosure rõ ràng | 🟠 |
| KH · LA · ID · PH · MY | luật từng nước | Ít tiền lệ thực thi **không có nghĩa là được phép** | 🟡 |

**Hệ quả thiết kế, không phải hệ quả câu chữ:**

| Creative | Tầng A · B · D | **Tầng C (AU·UK·EU·US·GCC)** |
|---|---|---|
| Before–after mặt | ✅ nếu có đồng ý **phạm vi quốc tế** | 🔴 **Mặc định KHÔNG** |
| Testimonial **kết quả lâm sàng** | ✅ nếu thật | 🔴 **KHÔNG** — AHPRA cấm thẳng |
| Testimonial **trải nghiệm phi lâm sàng** *(phiên dịch · đưa đón · khách sạn · nhân viên)* | ✅ | ✅ **dùng được — lối đi hợp lệ** |
| Before–after **cơ thể** / giảm béo | ⛔ | ⛔ |

→ Landing tầng C **không được dựa vào** before–after và testimonial làm trụ bằng chứng. Phải loại chúng khỏi kế hoạch **trước khi viết**, không loại sau. Trụ thay thế: **giấy phép Bộ Y tế → hồ sơ bác sĩ → quy trình an toàn → International Patient Department → quy trình 5 bước cho khách ở xa → T&C bảo hành**.

Đây cũng là lý do khối *"Out of Town Patients"* quan trọng hơn khối testimonial: nó là bằng chứng **được phép dùng ở mọi thị trường**.

⛔ **Agent không đưa ra kết luận pháp lý** — nêu cơ quan phải tra, gắn cờ ⚠️, đề xuất biến thể hạ rủi ro. Dòng kết luận luôn là *"cần Pháp chế xác nhận cho thị trường [X] trước khi bật."*

### ⑥ Giá **HIỆN**, không ẩn

Gói nội địa ẩn giá (dữ liệu động, lấy tại `/bang-gia/`). Gói QT **phải hiện giá** — chênh giá chính là cái hook, và khách tầng C vào trang để tìm đúng con số đó.

**Ba dòng bắt buộc đi kèm mọi bảng giá:**
```
The price shown does not include the 10% international service charge.
USD figures are approximate and depend on the exchange rate on the day of payment.
Final cost is confirmed by the doctor after an in-person examination.
```

**Bỏ dòng đầu là bom niềm tin** — khách phát hiện ở quầy thanh toán thì mất cả ca và nhận review xấu.
⛔ **Không so giá với quốc gia hoặc cơ sở CÓ TÊN** (*"70% cheaper than Australia"*) — claim cần bằng chứng, và là rủi ro ở AU/UK. Công bố bảng giá đầy đủ, **để bảng giá nói thay**.

### ⑦ Đo bằng **chi phí/khách ĐẾN KHÁM**, không bằng CPL

```
click → lead → phản hồi được → gửi ảnh → báo giá → ĐẶT CỌC → đặt vé → ĐẾN KHÁM
```

⛔ **CPL là chỉ số gây nhầm lẫn nhất của gói này.** Lead Campuchia rẻ gấp nhiều lần lead Úc, nhưng tỷ lệ đến khám khác hoàn toàn — **so CPL giữa hai market là so hai thứ khác nhau**.

**Hai chỉ số trung gian phải đo:**
- **Tỷ lệ phản hồi được** — chẩn đoán **múi giờ và kênh**, không phải từ khoá.
- **Tỷ lệ đặt cọc** — **điểm chuyển trạng thái thật** của du lịch y tế. Khách đặt cọc rồi gần như luôn đến.

⚠️ **LUẬT ĐỘ TRỄ: `lead → đến khám` mất 4–12 tuần** (tầng B tới 6 tháng nếu chờ Tết).
→ ⛔ **Không kết luận chiến dịch tầng B/C trong cửa sổ < 8 tuần.** So theo **cohort** theo tháng nhận lead.
→ ✅ Tầng D (expat) đo được trong 1–2 tuần.

> Đây là luật bị phá nhiều nhất. Áp lực báo cáo hằng tuần làm team cắt chiến dịch tầng C ở tuần thứ 3 vì *"CPL cao, chưa ra ca"* — trong khi **ca của nó đang trên đường**, theo nghĩa đúng của từ.

**Thứ tự chẩn đoán ④→①→②→③** (④ rẻ nhất và nhanh nhất): ④ cấu hình/vận hành (`geo_mode` sai → sửa 5 phút; tỷ lệ phản hồi thấp là **vấn đề vận hành**, không phải quảng cáo) → ① đổi từ khoá → ② làm lại landing → ③ đổi mẫu QC.

---

## ⚠️ SỐ NGÀY Ở LẠI VIỆT NAM — trường dữ liệu quan trọng nhất chưa có

Với khách nội địa, câu chặn là *"nghỉ bao lâu mới đi làm được"*.
Với khách quốc tế, câu chặn là **"tôi phải ở Việt Nam bao nhiêu ngày"** — và đây là câu hỏi **kế hoạch**, không phải câu hỏi nỗi sợ. Nó quyết định khách có đặt vé hay không.

**Không trả lời được câu này thì khách không đặt vé, và không đặt vé thì lead không bao giờ thành ca.**

⛔ **Agent KHÔNG được tự suy ra số ngày này.** Đây là mốc **y khoa** (thời điểm cắt chỉ, tái khám cuối, được phép bay), không phải con số marketing. **Bay quá sớm sau phẫu thuật là rủi ro y khoa thật.**
→ Chưa có → `[PENDING: minimum stay — Medical Dept]` đúng vị trí trên trang.
→ Có rồi → **khoảng + "varies by case"** + nêu rõ **mốc nào**.

**Bảng ở [`kn-thi-truong-quoc-te.md`](knowledge/kn-thi-truong-quoc-te.md) §8 hiện toàn bộ là `[CHỜ CẬP NHẬT]`. Điền xong bảng này là việc có đòn bẩy cao nhất trong cả gói.**

---

## Cổng WIN 4 tiêu chí — qua 3/4

| # | Tiêu chí | Đạt khi |
|---|---|---|
| ① | **Sát chuyển đổi** | Intent mua **hoặc intent kế hoạch**: `cost` · `price` · `how many days` · `book` |
| ② | **Cạnh tranh ít** | Ngách · dài · **tiếng Việt tầng B** · **từ khoá S4** |
| ③ | **Giá trị ca lớn** | breast augmentation · rib-cartilage rhinoplasty · V-line · facelift · Lipo 360 · hair transplant |
| ④ ★ | **Ý chí đi lại** | Có `vietnam`/`hanoi`/`abroad`/`medical tourism`, **hoặc** thuộc tầng **B/D** |

**④ là tiêu chí cắt tiền của gói này.** `rhinoplasty cost` gõ từ Sydney đạt ①②③ và **trượt ④** — người này đang hỏi giá **ở Sydney**. Chạy từ khoá đó là trả tiền để gặp người sẽ không bao giờ bay. Bỏ tiêu chí ④ là nguyên nhân chính của *"CTR tốt, lead có, không ai đến khám"*.

**Luật combo:** dịch vụ giá thấp (mí mắt · da liễu · spa) cho tầng A/B/C → `win` tối đa **2/4**, chỉ dùng làm cụm combo. **Không ai bay 6 giờ để cắt mí.**

**Gom nhóm:** 1 dịch vụ × 1 chặng × 1 intent × **1 tầng thị trường** = 1 landing + 1 bộ QC.

---

## Ba ngách ưu tiên — nên chiếm ≥ 40% ngân sách giai đoạn đầu

**① Từ khoá kế hoạch chuyến đi (S4).** `how many days in vietnam after rhinoplasty` · `english speaking plastic surgeon hanoi` · `airport pickup hospital vietnam` · `can i fly after rhinoplasty`.
→ Cạnh tranh **gần như bằng không**. Người gõ **đã quyết định làm**. **Ngách tốt nhất của cả gói.**

**② Từ khoá tiếng Việt từ nước ngoài (tầng B).** `nâng mũi ở việt nam cho việt kiều` · `về việt nam thẩm mỹ dịp tết`.
→ **Không đối thủ quốc tế nào đấu.** Khách đã tin thương hiệu Việt và **đã có vé**.

**③ Từ khoá sửa lại.** `revision rhinoplasty vietnam` · `fix bad nose job abroad`.
→ Giá trị ca **cao nhất**, nhưng cần bộ bằng chứng riêng và **giọng khác hẳn**: không bán kết quả, bán **đánh giá lại**.

---

## Design System Kangnam International v1.0 — sạch & sang trọng

Token lấy từ trang production [`/top-plastic-surgery-in-vietnam/`](https://kangnamaesthetichospital.com/top-plastic-surgery-in-vietnam/) (bản lưu: [`template/`](template/)).

```css
--teal:#005F88;  --teal-900:#00394F;  --teal-400:#00BAC3;  --navy:#003C77;
--gold:#B08D4F;  --gold-dk:#8C6E36;   --gold-lt:#C9A86A;
--cta:#E15A01;   --cta-press:#C44D00;
--bg:#FFFFFF;    --champagne:#FAF7F2; --surface-alt:#F7F9FA;
--ink:#14212B;   --ink-2:#4A5C6A;     --ink-3:#7A8B98;  --line:#E3E8EC;
--maxw:1140px;   --maxw-text:68ch;
```

**Tỷ lệ: 78% trắng/champagne · 15% teal · 5% gold · 2% cam CTA.**

### ⚠️ Khác cấu trúc lớn nhất: **responsive full-width, KHÔNG phải thẻ 480px**

Gói nội địa dựng **thẻ khổ điện thoại `max-width:480px`** căn giữa. Gói QT dùng **`max-width:1140px` responsive**, vì:
- khách tầng C **nghiên cứu trên desktop** (so giá, đọc hồ sơ bác sĩ, mở nhiều tab) rồi mới chuyển sang mobile để nhắn tin;
- bảng giá và bảng so sánh điểm đến **cần chiều ngang**;
- một thẻ 480px trên màn 1440px đọc như một trang quảng cáo địa phương, **không như một bệnh viện quốc tế**.

### Bảy rào tương phản — đã đo, không ước lượng

| Luật | Số đo |
|---|---|
| ✅ `--teal` **an toàn mọi cỡ**, cả chữ trên trắng và trắng trên nền teal | **7,02:1** AA/AAA cả hai chiều |
| ✅ `--teal-900` · `--navy` | 12,37 · 10,98 AAA |
| ⛔ **`--teal-400` KHÔNG làm chữ trên trắng** | **2,38 — fail.** Chỉ vạch, viền, icon |
| ⛔ **`--gold` KHÔNG làm chữ nhỏ trên trắng** | **3,10** → chỉ **≥24px thường hoặc ≥19px/700**; nhỏ hơn dùng **`--gold-dk` (4,77 AA)** |
| ⛔ **`--cta` là màu NỀN NÚT, không phải màu chữ** | Trắng trên nó **3,71** → nhãn nút **≥19px/700**; nút nhỏ hơn dùng **`--cta-press` (4,76 AA)** |
| ⛔ **`--ink-3` KHÔNG dùng cho chữ thân** | **3,52 — fail.** Chữ phụ dùng **`--ink-2` (6,93 AA)** |
| ✅ Gold trên nền tối | `--gold-lt` trên `--teal-900` = **5,47 AA** · `#FEC465` = **7,83 AAA** |

### Hai font

**Cormorant Garamond 600** (display, **≥28px** — không bao giờ nhỏ hơn) + **Inter** 400/500/600/700 (body · UI · nút · form). Body **17px**, input **16px**.

> ⚠️ Lệch với production (đang chạy **Roboto** cho toàn bộ). Cặp font này là **register quốc tế của gói**, cần brand chốt một lần — xem *Việc còn treo* ở [`doc/CHANGELOG.md`](doc/CHANGELOG.md). Chưa chốt thì dùng Inter cho cả display (weight 600) và **nói rõ đang dùng bản dự phòng**.

### "Sang trọng" đến từ ba thứ, không đến từ màu

① **khoảng trắng lớn** (section padding 96px desktop / 48px mobile) · ② **serif hiển thị ở cỡ lớn** · ③ **gold dùng rất ít**, chỉ vạch mảnh và eyebrow.
**Dùng nhiều gold làm trang trông rẻ đi, không sang hơn.**

⛔ Không nền tối toàn trang · quá 3 màu chính · gradient/neon · nhiều style icon · chồng shadow · popup chặn màn đầu · đếm ngược tự reset.

**Mẫu dựng sẵn:** [`template/lp-skeleton-en.html`](template/lp-skeleton-en.html) — khung **L3 Trip-plan**, đầy đủ token · 14 khối · form quốc tế · ô ảnh tạm · khối `[PENDING]` · `§LEGAL` cuối file.

---

## Form quốc tế **không thể 3 trường** như gói nội địa

| # | Trường | Bắt buộc |
|---|---|---|
| 1–2 | Full name · **country code + phone** | ✅ |
| 3 | **Email** | ✅ — lệch múi giờ nên email là kênh chắc chắn nhất |
| 4–5 | Country/market · service of interest | ✅ |
| 6 | **Preferred messaging channel** — chọn **1**, không chọn nhiều | ✅ |
| 7 ★ | **Preferred contact time + time zone** | ✅ |
| 8 | Planned travel window | — |
| 9 | **Consent** — nêu rõ **chuyển dữ liệu sang Việt Nam** + link privacy policy | ✅ |

### ★ Vì sao trường ⑦ quyết định tỷ lệ kết nối

Bệnh viện mở **8am–5pm giờ Việt Nam (UTC+7)**:

| Giờ VN 8am–5pm | = giờ khách |
|---|---|
| Sydney | 11am – 8pm ✅ |
| Dubai | 5am – 2pm ⚠️ |
| London | 1am – 10am ⚠️ |
| **Los Angeles** | **5pm – 2am** 🔴 |

→ Lead từ California gửi form buổi tối ở họ sẽ **không có ai trả lời trong ~12 giờ**, và cuộc gọi lại sẽ đến vào **2 giờ sáng** giờ họ.
→ Không thu trường ⑦ thì lead tầng C **mất phần lớn ở khâu kết nối**, và báo cáo sẽ hiển thị như *"lead chất lượng kém"* trong khi vấn đề là **múi giờ**.

Trang thank-you phải nói rõ sẽ liên hệ **khi nào theo giờ của khách**.

---

## 🔴 Ba lỗi đang có trên trang tham chiếu production — phát hiện 21/10/2026

Trang `/top-plastic-surgery-in-vietnam/` là **mẫu style** của gói này. Nó **không phải mẫu nội dung**.

| # | Lỗi | Nguyên văn trên bản live | Vì sao nghiêm trọng |
|---|---|---|---|
| ① | **Tên bác sĩ của cơ sở khác** trong FAQ | *"**Dr. Granzow** will be able to provide a good estimate for the length of your procedure during your consultation."* | FAQ **copy từ website một bác sĩ Mỹ khác**. Không có bác sĩ nào tên Granzow ở Kangnam. Khách tầng C tra tên này sẽ thấy ngay → mất toàn bộ niềm tin |
| ② | **Bộ đếm hỏng** | *"Trusted by **0+** clients"* | Khối social proof đang hiện số **0**. Tệ hơn là không có khối nào |
| ③ | **Cam kết kết quả vĩnh viễn** | *"Is rhinoplasty a permanent procedure? **Yes**, … the results are permanent."* | Cam kết kết quả y khoa — vi phạm luật VN, rủi ro FTC/ASA/AHPRA |

Thêm hai claim cần xử lý: **"Lifetime warranty"** (không có T&C công bố) và **"The Leading / Top-Rated Aesthetic Hospital in Vietnam"** (superlative — dùng trong tiêu đề SEO là chuyện của SEO, nhưng **đưa vào mẫu quảng cáo hoặc headline landing là không được**).

✅ Lấy từ trang tham chiếu: **token màu · nhịp section · spec form quốc tế · khối 5 bước cho khách ở xa**.
❌ Không lấy: câu FAQ · con số social proof · câu định vị superlative · claim `lifetime`/`permanent`.

Bộ não đã cài luật không sao chép bốn thứ này (§18 rule 20). Chi tiết: [`kn-ho-so-thuong-hieu-qt.md`](knowledge/kn-ho-so-thuong-hieu-qt.md) §4.4.

---

## Quick start (6 bước)

1. Tạo 1 Project / Gem / GPT mới. Tên và mô tả: [`doc/01-cai-dat.md` §0](doc/01-cai-dat.md).
2. **Instructions:** dán khối ▼▲ trong [`SYSTEM-PROMPT.md`](SYSTEM-PROMPT.md) — riêng **ChatGPT** dùng [`SYSTEM-PROMPT-NGAN.md`](SYSTEM-PROMPT-NGAN.md) và **đọc phần đánh đổi ở đầu file**.
3. **Knowledge:** upload **7 file** trong [`knowledge/`](knowledge/).
4. **Cho MODE 1** (xuất Excel): bật công cụ chạy code + upload [`tools/build_keyword_workbook.py`](tools/) · [`markets/README.md`](markets/README.md) · [`markets/rhinoplasty-tier-c-au.json`](markets/).
5. **Cho MODE 3:** upload [`template/lp-skeleton-en.html`](template/lp-skeleton-en.html).
6. Chạy **6 câu smoke test** ở [`doc/01-cai-dat.md` §3](doc/01-cai-dat.md) — nhất là **câu 3** (Agent không được tự nghĩ ra số ngày ở lại).

**Câu lệnh mẫu:**
```
MODE 1 — dựng bộ từ khoá cho Rhinoplasty, thị trường Úc (AU),
ngân sách 200 triệu VND/tháng. Xuất file Excel cho tôi tải về.
```
```
MODE 3 — landing cho cụm "how many days in vietnam after rhinoplasty",
market AU, tầng C. Chọn khung, nói rõ vì sao, rồi dựng HTML.
```

Bộ câu lệnh đầy đủ: [`doc/02-cau-lenh.md`](doc/02-cau-lenh.md)

---

## Tài liệu

| File | Nội dung | Trạng thái |
|---|---|---|
| [SYSTEM-PROMPT.md](SYSTEM-PROMPT.md) | Bộ não — 20 mục · **43.452 ký tự** | ✅ |
| [SYSTEM-PROMPT-NGAN.md](SYSTEM-PROMPT-NGAN.md) | Bản cổng chặn **7.979 ký tự** — chỉ cho **ChatGPT**. ⚠️ Đã cắt phần quy trình, **bắt buộc nạp Knowledge** | ✅ |
| [knowledge/kn-rao-phap-ly-qt.md](knowledge/kn-rao-phap-ly-qt.md) | **Cổng pháp lý hai tầng** · từ cấm tiếng Anh · luật ảnh theo market · GDPR | ✅ |
| [knowledge/kn-thi-truong-quoc-te.md](knowledge/kn-thi-truong-quoc-te.md) | ★ **File lõi** — 4 tầng · cổng GEO-TARGET · bản đồ thị trường × dịch vụ · mùa bay · giá · **số ngày ở lại** | ✅ |
| [knowledge/kn-chan-dung-hanh-trinh-qt.md](knowledge/kn-chan-dung-hanh-trinh-qt.md) | ★ **4 rào cản (có XA)** · 7 chân dung · **phễu 7 chặng** | ✅ |
| [knowledge/kn-cong-win-tu-khoa-qt.md](knowledge/kn-cong-win-tu-khoa-qt.md) | **Cổng WIN 3/4** · cổng GEO-TARGET · gom nhóm · 3 ngách ưu tiên | ✅ |
| [knowledge/kn-engine-win-ad-qt.md](knowledge/kn-engine-win-ad-qt.md) | B1–B7 · 10 archetype · A/B 6 lô · **chấm 14 điểm** · template RSA/Meta | ✅ |
| [knowledge/kn-khung-landing-qt.md](knowledge/kn-khung-landing-qt.md) | **6 khung L1–L6 · 14 khối · Design System v1.0 · form quốc tế · scorecard** | ✅ |
| [knowledge/kn-ho-so-thuong-hieu-qt.md](knowledge/kn-ho-so-thuong-hieu-qt.md) | Thương hiệu · 2 cơ sở · bác sĩ · trust · bảng giá · quy trình 5 bước *(module swappable)* | ✅ |
| [knowledge/kn-chan-doan-chi-so-qt.md](knowledge/kn-chan-doan-chi-so-qt.md) | **Phễu 8 bước** · luật độ trễ · bảng chẩn đoán · báo cáo 4 chiều | ✅ |
| [knowledge/kn-truy-van-geo-qt.md](knowledge/kn-truy-van-geo-qt.md) | ★ **MODE 5** — 83 truy vấn GEO · 15 cụm · 80/20 · bản đồ trang đích · 20 prompt đo SoV · **rào R0–R9** | ✅ |
| [knowledge/kn-quy-trinh-tuan-qt.md](knowledge/kn-quy-trinh-tuan-qt.md) | ★ **Vòng lặp tuần 4 bước** — 3 nguồn từ khoá · 3 nhóm người tìm · bảng kế hoạch sản xuất · **2 tầng chỉ số** · khuôn báo cáo tuần | ✅ |
| [prompts/prompt-nghien-cuu-tu-khoa.md](prompts/prompt-nghien-cuu-tu-khoa.md) | MODE 1 — 5 prompt + checklist nghiệm thu | ✅ |
| [prompts/prompt-build-ad-set.md](prompts/prompt-build-ad-set.md) | MODE 2 — 5 prompt + checklist | ✅ |
| [prompts/prompt-build-landing-page.md](prompts/prompt-build-landing-page.md) | MODE 3 — 6 prompt + checklist giao hàng | ✅ |
| [prompts/prompt-geo-answer.md](prompts/prompt-geo-answer.md) | **MODE 5** — 6 prompt + bảng đo SoV + checklist | ✅ |
| [prompts/prompt-quy-trinh-tron-goi.md](prompts/prompt-quy-trinh-tron-goi.md) | Dây chuyền 6 bước MODE 1→2→3, **3 chốt dừng** | ✅ |
| [markets/README.md](markets/README.md) | Schema JSON 17 khối + **3 cổng chặn** | ✅ |
| [markets/rhinoplasty-tier-c-au.json](markets/) | **Ví dụ hoàn chỉnh đã build được** — 5 chân dung · 6 chiến dịch · 6 landing · 26 từ khoá | ✅ |
| [tools/build_keyword_workbook.py](tools/) | Generator `.xlsx` 5 sheet · **cổng CAM · CLAIM · GEO · REGULATED** | ✅ |
| [template/lp-skeleton-en.html](template/lp-skeleton-en.html) | **Landing page mẫu** — khung L3, Design System v1.0, form quốc tế, `§LEGAL` | ✅ |
| [template/lp-reference-*.html / .css](template/) | Trang production đã lưu — nguồn của Design System | 📦 |
| [doc/01-cai-dat.md](doc/01-cai-dat.md) | Cài 3 nền tảng · **6 câu smoke test** · test generator · xử lý sự cố | ✅ |
| [doc/02-cau-lenh.md](doc/02-cau-lenh.md) | Câu lệnh 4 mode · prompt mẫu · **điều Agent sẽ từ chối** | ✅ |
| [doc/CHANGELOG.md](doc/CHANGELOG.md) | Lịch sử · 7 khác biệt · **15 việc còn treo** | ✅ |

> **Quy ước:** version ghi trong header từng file, **KHÔNG** gắn version vào tên file.
> **Không upload** lên Knowledge: `doc/` · `out/` · `template/lp-reference-*`.

---

## Ranh giới

Không cam kết kết quả y khoa (`best` · `#1` · `top-rated` · `leading` · `guaranteed` · `permanent` · `painless` · `no scars` · `risk-free` · `completely safe` · `cheapest`) · **không tự suy số ngày ở lại hoặc mốc hồi phục cứng** · không dùng chữ **"lifetime"** khi chưa có T&C · không chẩn đoán qua ảnh *(pre-consultation là việc của bác sĩ)* · không kê đơn · không báo giá ca cụ thể · không bịa giá · bác sĩ · bằng cấp · số ca · review · tư cách hội · không tạo ảnh kết quả giả · không dùng before–after chưa duyệt pháp lý **ở đúng thị trường đó** · không chèn ảnh stock/AI thay ô ảnh tạm · không so giá với quốc gia hoặc cơ sở **có tên** · không nêu tên hạ thấp đối thủ (gồm cơ sở ở Thái Lan · Hàn Quốc · Thổ Nhĩ Kỳ) · không hứa visa/thư mời/hoàn tiền/chi trả vé ca chỉnh sửa khi chưa có xác nhận · **không dùng máy dịch cho nội dung y khoa** · không nạp hộ chiếu/hồ sơ bệnh án/**ảnh khách** lên công cụ công cộng.

**Claim hội–hiệp hội** (VSAPS · ASPS · ASAPS · ISAPS · AAFPRS) chỉ được nêu khi đủ **ba điều kiện**: gắn **đúng tên cá nhân** · có **hồ sơ thành viên còn hiệu lực** tại Pháp chế · **không** trình bày như *board certification* hoặc giấy phép hành nghề. Site quốc tế đang hiển thị các hội này ở mức thương hiệu, trong khi gói nội địa cấm thẳng — **Pháp chế phải chốt một dòng dùng chung cho cả hai site**.

**Khách quốc tế chỉ phục vụ tại 2 cơ sở tuyến bệnh viện:** Hanoi (190 Trường Chinh · GP 194/BYT-GPHĐ) · HCMC (666 CMT8 · GP 287/BYT-GPHĐ). ⛔ Không giới thiệu 5 viện thẩm mỹ tỉnh cho khách quốc tế.

**Yêu cầu về cơ xương khớp / bảo tồn khớp** thuộc thương hiệu riêng, có agent riêng [`Agent-CoXuongKhop`](../Agent-CoXuongKhop/). **Nội dung tiếng Việt cho khách trong nước** thuộc [`Agent-AdsOptimize-Kangnam`](../Agent-AdsOptimize-Kangnam/) — site khác, giá ẩn, 7 cơ sở, có bẫy TUYẾN. **Không trộn hai gói.** Ngoại lệ duy nhất: **tầng B (kiều bào)** viết bằng tiếng Việt nhưng **thuộc gói QT**, vì rào cản là XA và cơ sở chỉ có 2.

**Agent không đưa ra kết luận pháp lý.** Mọi mẫu QC / landing / bảng giá / bản dịch là **bản đề xuất**, phải qua **bốn cửa duyệt**: Pháp chế VN · Pháp chế thị trường đích · Khoa Chuyên môn · người bản ngữ.
"# Agent-AdsOptimize-Kangnam-QT" 
