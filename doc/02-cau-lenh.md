# 02 · CÂU LỆNH — ADS OPTIMIZE KANGNAM QUỐC TẾ

---

# 1. Công thức ra lệnh

```
MODE [1-5] — [việc cần làm]
Thị trường: [bắt buộc với MODE 1-4]
Dịch vụ:    [bắt buộc]
[+ ngân sách / từ khoá / số liệu tuỳ mode]
[MODE 5: thay "Thị trường" bằng "Cụm: Qxx"]
```

**Trường duy nhất không bao giờ được bỏ (MODE 1–4): THỊ TRƯỜNG.** MODE 5 là ngoại lệ — AI không có geo-targeting, nên nó cần **cụm Q01–Q15**. Không biết người xem ở đâu thì không biết luật nào áp, viết ngôn ngữ nào, gắn kênh nào. Agent sẽ hỏi lại, và đó là đúng.

Nói bằng lời thường cũng được — Agent tự suy mode rồi báo lại. Nhưng nó vẫn sẽ hỏi thị trường.

---

# 2. MODE 1 — KEYWORD-RESEARCH

## 2.1 Mở một thị trường mới
```
MODE 1 — dựng bộ từ khoá cho Rhinoplasty, thị trường Úc (AU),
ngân sách 200 triệu VND/tháng. Xuất file Excel cho tôi tải về.
```

## 2.2 Tầng kiều bào — từ khoá tiếng Việt
```
MODE 1 — bộ từ khoá cho Facelift, tầng B kiều bào ở Mỹ (VN-DIASPORA-US),
ngân sách 120 triệu/tháng.

Lưu ý: tầng này tìm bằng TIẾNG VIỆT từ IP nước ngoài. Từ khoá phải là tiếng Việt,
geo-target là Mỹ. Lịch chạy theo mùa bay (trước Tết 8–10 tuần, hè).
```

## 2.3 Tầng expat — cẩn thận cổng GEO-TARGET
```
MODE 1 — bộ từ khoá cho tầng D (expat đang sống tại Hà Nội và TP.HCM),
nhóm dịch vụ da liễu + clinic, ngân sách 60 triệu/tháng.

Nhớ: geo_mode = Presence, bắt buộc. Landing KHÔNG có khối đưa đón sân bay.
Tầng D là tầng duy nhất bán được dịch vụ da/clinic đơn lẻ.
```

## 2.4 Chỉ cần chân dung khách hàng
```
Chỉ làm bước K3: 5 chân dung khách hàng cho thị trường GCC (UAE + Saudi),
dịch vụ Rhinoplasty. Mỗi chân dung đủ 7 câu.
Chưa cần từ khoá.
```

## 2.5 Kiểm trước: dịch vụ này có bán được không
```
Tôi muốn chạy quảng cáo "trị nám" cho khách Úc. Kiểm giúp tôi trước khi làm:
dịch vụ này có bán được cho tầng C không? Giá trị ca có bù nổi vé máy bay
+ khách sạn + ngày nghỉ việc?
```
*(Câu trả lời đúng là **không** — và Agent nên nói thẳng, rồi đề xuất ghép combo.)*

## 2.6 Rà soát bộ từ khoá đã có
```
Rà bộ từ khoá này trước khi tôi giao team. Kiểm: mọi dòng có market + geo_mode
chưa · dòng VN-EXPAT nào không phải Presence · dòng market rủi ro cao nào chưa
khai cách xử lý creative · có Broad không · volume/cpc có bị điền sẵn không
· tổng ngân sách có đúng 100% và S4 có ≥ 15% không.
```

---

# 3. MODE 2 — WIN-AD

## 3.1 Một nhóm từ khoá
```
MODE 2 — nhóm từ khoá:
  rhinoplasty cost vietnam
  nose job price vietnam
  rhinoplasty package vietnam
Market: AU · Tầng: C · Dịch vụ: Rhinoplasty

Chấm cổng WIN trước. Qua cổng thì sinh RSA + Meta, đếm ký tự từng dòng,
chấm 14 điểm.
```

## 3.2 Chặng S4 — ngách tốt nhất
```
MODE 2 cho chặng S4 (kế hoạch chuyến đi), market AU, dịch vụ Rhinoplasty.
Dùng góc C (khả thi của chuyến đi).
Cần 2 headline về số ngày ở lại, 2 về phiên dịch/chăm sóc sau khi về,
2 về đưa đón + khách sạn.
```

## 3.3 Chỉ cần hook
```
Viết 5 hook cho Breast augmentation, market AU, chặng S3 (nỗi sợ).
Mỗi hook: 1 câu khách nói thật + 1 bằng chứng được phép dùng ở Úc.
Nhớ AHPRA cấm testimonial kết quả lâm sàng.
```

## 3.4 Khách sửa lại
```
MODE 2 cho nhóm "revision rhinoplasty vietnam", market AU.
Chân dung là khách đã làm ở nơi khác và thất vọng.
Giọng phải khác hẳn: bán ĐÁNH GIÁ LẠI, không bán kết quả.
```

## 3.5 Kiểm một câu có chạy được không
```
Câu này tôi viết cho quảng cáo nhắm khách Úc, có vấn đề gì không?
"Vietnam's top-rated hospital — lifetime warranty, permanent results, 
painless rhinoplasty from $1,353"
```
*(Agent phải bắt được **bốn** lỗi: `top-rated` · `lifetime warranty` chưa có T&C · `permanent results` là cam kết kết quả · `painless`. Và nhắc giá phải kèm phụ phí 10%.)*

## 3.6 Rà bộ mẫu đang chạy
```
Rà bộ mẫu quảng cáo này. Kiểm 8 điểm: khai market/geo_mode · đếm ký tự
· từ cấm tiếng Anh · testimonial hoặc before-after cho market rủi ro cao
· hứa số ngày ở lại · so giá với quốc gia có tên · CTA gắn mấy kênh.
Chấm lại 14 điểm.
```

---

# 4. MODE 3 — LDP-BUILD

## 4.1 Dựng landing từ cụm từ khoá
```
MODE 3 — landing cho cụm "how many days in vietnam after rhinoplasty",
market AU, tầng C, dịch vụ Rhinoplasty, cơ sở Hanoi.
Chọn khung, nói rõ vì sao, rồi dựng.
```

## 4.2 Khung L3 — trang quan trọng nhất
```
MODE 3 — dựng landing khung L3 Trip-plan cho Rhinoplasty, market AU.
Hai khối B08 (your trip) và B09 (after you fly home) không được làm sơ sài.
Đối chiếu template/lp-skeleton-en.html.
```

## 4.3 Dựng thẳng HTML
```
Dựng HTML một file, Design System Kangnam International v1.0.
Responsive max-width 1140px (KHÔNG phải thẻ 480px như gói nội địa).
Cormorant Garamond cho display + Inter cho body. Input 16px.
Form đủ trường, có preferred contact time + time zone.
Ảnh chưa có thì ô ảnh tạm. Cuối file kèm §LEGAL + bảng kê ảnh + self-score.
```

## 4.4 Landing cho expat — khác hẳn
```
MODE 3 — landing cho "english speaking plastic surgeon hanoi",
market VN-EXPAT, tầng D.
⛔ KHÔNG có khối đưa đón sân bay, KHÔNG có khối khách sạn, KHÔNG có khối
số ngày ở lại. Khách đang sống ở Hà Nội.
CTA là đặt khám tuần này.
```

## 4.5 Landing S2 — chưa bán Kangnam
```
MODE 3 — landing cho "vietnam vs thailand plastic surgery", market AU.
Khung L1 Destination: trả lời câu hỏi về VIỆT NAM trước, Kangnam sau.
⛔ Không hạ thấp Thái Lan — nêu tiêu chí khách quan, để khách tự so.
```

## 4.6 Rà soát trước khi đẩy traffic
```
Rà landing này theo scorecard §9. Chấm điểm từng tiêu chí.
Kiểm kỹ 3 điểm: có số ngày ở lại chưa · có nói ai lo sau khi về nước chưa
· bộ bằng chứng có đúng luật của market này chưa.
Viết lại phần yếu nhất.
```

## 4.7 Chuyển sang market khác
```
Tôi có landing này cho market AU. Chuyển sang GCC (UAE).
Trước khi viết, trả lời: GCC có cùng nhóm luật quảng cáo với AU không?
Khác tầng không? Cần thêm gì cho Muslim-friendly care?
```

---

# 5. MODE 4 — OPTIMIZE

## 5.1 Chẩn đoán đầy đủ
```
MODE 4 — số liệu 10 tuần, market AU, tầng C:
  Chi phí: … · Impression: … · Click: … · CTR: … · CPC: …
  Lead: … · Phản hồi được: … · Đặt cọc: … · Đến khám: …
  GA4: scroll depth … · form view → submit …

Chẩn đoán theo phễu 8 bước, nêu rõ rụng ở bước nào.
Ra 4 quyết định theo thứ tự ④→①→②③.
```

## 5.2 Lead nhiều mà không ai đến khám
```
MODE 4 — chiến dịch AU có 80 lead trong 6 tuần nhưng chưa ai đến khám.
CPL trông rẻ. Chẩn đoán giúp tôi.
```
*(Agent phải kiểm **tiêu chí ④ travel intent** và **cổng GEO-TARGET** trước, không nhảy vào landing. Và phải nhắc cửa sổ 6 tuần là **chưa đủ** để kết luận.)*

## 5.3 Lead không bắt máy
```
MODE 4 — tỷ lệ phản hồi được chỉ 40%. Lead chủ yếu từ US và Canada.
```
*(Đáp án đúng: **vấn đề vận hành**, không phải vấn đề quảng cáo — múi giờ. 8am–5pm ICT = 5pm–2am ở Los Angeles.)*

## 5.4 Cửa sổ chưa đủ
```
MODE 4 — số liệu 3 tuần của chiến dịch AU. CPL cao gấp đôi dự kiến.
Có nên cắt không?
```
*(Agent phải nói ngay dòng đầu: **3 tuần chưa kết luận được** — độ trễ 4–12 tuần. Chỉ đọc được chỉ số sớm.)*

## 5.5 Mở rộng winner
```
MODE 4 — mẫu A ở market AU đang có chi phí/khách đến khám tốt nhất.
Nhân bản sang market nào được, sang market nào KHÔNG được, và vì sao?
```

---

# 5b. MODE 5 — GEO-ANSWER

## 5b.1 Làm một cụm
```
MODE 5 — GEO-ANSWER cho cụm Q13 (Medical tourism logistics).
Rà rào pháp lý trước khi viết.
```

## 5b.2 Kế hoạch Sóng 1 — bốn cụm Tầng A
```
MODE 5 — Sóng 1, 90 ngày. Làm kế hoạch cho 4 cụm Tầng A (Q10 · Q12 · Q11 · Q13).
Mỗi cụm: số truy vấn CORE · trang đích · dạng nội dung · rào pháp lý · dữ liệu còn thiếu.
Nói rõ cụm nào BỊ CHẶN và ai phải cấp dữ liệu.
```

## 5b.3 Đo Share of Voice
```
MODE 5 — đo SoV tháng này. Cho tôi 20 prompt + khuôn bảng ghi kết quả
(ChatGPT / Gemini / AI Overview + cột đối thủ được AI nhắc).
```

## 5b.4 Rà bài EN đã có
```
Rà bài EN này theo bộ truy vấn GEO: nó trả lời truy vấn nào · H2 có dùng đúng
câu khách gõ không · câu trả lời có trong 2–3 câu đầu không · còn rào R1/R2/R3/R7 nào
· có dùng AIDA thay vì PAS không.
```

Chi tiết: [`prompts/prompt-geo-answer.md`](../prompts/prompt-geo-answer.md)

---

# 6. Quy trình trọn gói
```
Chạy trọn gói cho Rhinoplasty ở thị trường AU, ngân sách 200 triệu/tháng.
Dừng ở 3 chốt: sau bộ từ khoá, sau mẫu quảng cáo, sau landing.
```
Chi tiết: [`prompts/prompt-quy-trinh-tron-goi.md`](../prompts/prompt-quy-trinh-tron-goi.md)

---

# 6b. Vòng lặp tuần — chọn từ khoá → gom cụm → kế hoạch LDP → báo cáo

Mục 6 là **mở một thị trường mới**, chạy một lần. Mục 6b là **nhịp vận hành hằng tuần** sau khi
đã có landing chạy. Tri thức nền: [`knowledge/kn-quy-trinh-tuan-qt.md`](../knowledge/kn-quy-trinh-tuan-qt.md)

## 6b.1 Chạy trọn vòng một tuần — bốn bước
```
Chạy trọn vòng tuần này cho thị trường [Úc], dịch vụ [nâng mũi].

Bước 1 — chọn từ khoá: lấy từ bộ truy vấn GEO, cộng truy vấn thực đang đổ vào
landing đang chạy. Tách rõ ba nhóm người tìm.
Bước 2 — gom cụm: mỗi cụm là một landing.
Bước 3 — kế hoạch sản xuất: trang nào làm trước, ngân sách tuần, ai làm, xong khi nào.
Bước 4 — khuôn báo cáo: tuần sau đọc chỉ số nào.

Chỗ nào thiếu dữ liệu thì ghi [PENDING: ... — bộ phận nào], đừng đoán.
```

## 6b.2 Từ bộ từ khoá sang kế hoạch làm landing
```
Đây là bộ từ khoá đã duyệt cho [thị trường]. Gom thành cụm, mỗi cụm một landing.

Mỗi cụm cho tôi: tên cụm · khung landing nào (L1–L6) · chặng phễu nào (S1–S7) ·
nỗi lo chính phải gỡ · ước lượng ngân sách tuần · độ ưu tiên.

Xếp theo thứ tự nên làm, và nói rõ vì sao trang đầu tiên là trang đó.
```

## 6b.3 Báo cáo tuần các landing đang chạy
```
Làm báo cáo tuần cho các landing đang chạy ở [thị trường].

Số liệu tôi dán ở dưới, lấy từ Google Analytics và Google Ads.
Tách rõ hai tầng: chỉ số sớm (đọc tuần) và chỉ số cohort (đọc mỗi 8 tuần).
Đừng trộn hai tầng trong một kết luận.

Kết thúc bằng bảng việc tuần tới và danh sách trang đang bị chặn vì thiếu dữ liệu.

[dán số liệu]
```
> ⛔ Báo cáo **thiếu cột `market` hoặc `cohort`** là báo cáo không dùng được — agent sẽ nói
> thẳng điều đó thay vì kết luận trên số liệu đã trộn thị trường.

## 6b.4 Một trang có đang hiệu quả không
```
Trang [URL hoặc tên] chạy được [số] tuần. Số liệu ở dưới.

Nó đang hiệu quả hay không, và nếu chưa thì sai ở khối nào?
Nói rõ cái gì kết luận được bây giờ, cái gì phải chờ đủ cửa sổ.

[dán số liệu]
```
*Thời gian trên trang dưới **45 giây** thì hero sai — sửa ngay, không chờ ai đặt cọc.*

## 6b.5 Cần nối dữ liệu gì để báo cáo tự chạy
```
Liệt kê đúng những gì cần nối để báo cáo tuần tự động được: nguồn nào, lấy trường nào
từ Google Analytics và Google Ads, và cần khai thêm gì trong CRM.

Nói rõ cái gì đang thiếu khiến báo cáo chưa tự động được.
```

**Trạng thái kết nối hiện tại** (tra 21/10/2026):

| Nguồn | Trạng thái | Ghi chú |
|---|---|---|
| **Google Analytics** — site quốc tế | ✅ **đã nối** | Property `417341092` = `kangnamaesthetichospital.com` |
| Google Analytics — site nội địa | ✅ đã nối | Property `253218410` |
| **Google Ads** | ❌ **chưa có tài khoản nào được nối** | **Không có bất kỳ chỉ số chi phí nào cho tới khi nối** |
| Keyword Planner | ⚠️ đã xác thực | Chỉ dùng điền `volume` · `cpc` |
| **Trình kéo số liệu (Supermetrics)** | 🔴 **trial hết hạn 24/07/2026** | **Chặn mọi truy vấn số liệu tự động** |

Nên: bước 4 hiện **làm tay** — đọc số trên Google Analytics và Google Ads rồi điền vào khuôn
báo cáo §5.4 của `kn-quy-trinh-tuan-qt.md`. Tên trường trong khuôn đã khai đúng theo GA4
nên khi nối lại được là dùng ngay, không phải dựng lại.

**Ba việc để tự động hoá:** ① gia hạn trình kéo số liệu · ② **nối tài khoản Google Ads** ·
③ khai **ba thẻ CRM** `market` · `tier` · `stage` cho mọi lead **ngay từ đầu** — không gắn từ
đầu thì 8 tuần sau không cắt được cohort.

---

# 7. Prompt hỏi đáp (không sản xuất)

```
Giải thích rào cản XA là gì và vì sao nó là rào cản quyết định của gói quốc tế.
```
```
Thị trường nào trong danh sách của tôi có rủi ro quảng cáo cao nhất, và vì sao?
```
```
Tầng B (kiều bào) khác tầng C thế nào? Tại sao không gộp vào một chiến dịch
dù họ cùng sống ở Úc?
```
```
Tôi nên điền dữ liệu gì trước để gói này chạy được tốt nhất?
```
*(Đáp án đúng: **bảng số ngày ở lại** — việc có đòn bẩy cao nhất.)*

---

# 8. Điều Agent sẽ từ chối — và đó là đúng

| Bạn yêu cầu | Agent làm gì |
|---|---|
| Viết quảng cáo mà không nói thị trường | **Hỏi lại.** Đây là trường duy nhất không được giả định |
| Cho tôi số ngày ở lại Việt Nam | `[PENDING: minimum stay — Medical Dept]`. Mốc y khoa, không suy được |
| Dùng "lifetime warranty" | Từ chối tới khi có T&C bằng văn bản |
| Dùng review khách cho quảng cáo Úc | Gắn cờ AHPRA, đề xuất testimonial **phi lâm sàng** |
| Viết "70% cheaper than Australia" | Từ chối. Công bố bảng giá, để khách tự so |
| Nêu giá mà bỏ phụ phí 10% | Từ chối. Ba dòng bắt buộc là bắt buộc |
| Gắn VSAPS/ASPS vào mức thương hiệu | Từ chối. Chỉ gắn tên cá nhân, đủ 3 điều kiện |
| Giới thiệu viện Đà Nẵng cho khách Úc | Từ chối. Khách quốc tế chỉ Hà Nội và TP.HCM |
| Hứa hỗ trợ visa | `[PENDING]`. Chưa có xác nhận từ bộ phận quốc tế |
| Kết luận hiệu quả sau 3 tuần | Nói rõ chưa kết luận được, chỉ đọc chỉ số sớm |
| Chẩn đoán tình trạng mũi qua ảnh tôi gửi | Từ chối. Pre-consultation là việc của bác sĩ |
| Sửa generator để lách cổng | Từ chối. Sửa JSON, không sửa script |
| Viết nội dung GEO cho Q08 Dental | Chạy được — pháp nhân đã chốt. Nhưng vẫn **gắn 2 điều kiện**: bằng chứng hiện chỉ có ở TP.HCM, và trang web **không phải** phụ lục phạm vi giấy phép |
| Viết nội dung GEO cho Q09 BBL | Dừng. Kỹ thuật phải **thuộc DMKT** (R2), và nội dung phải **nói thật rủi ro thuyên tắc mỡ** |
| Chấm cổng WIN cho nội dung GEO | Từ chối. Cổng WIN và `geo_mode` **không áp cho MODE 5** |
| Bắt đầu MODE 5 từ trang dịch vụ | Cảnh báo đi sai thứ tự — **4 cụm Tầng A trước** |
| Chọn từ khoá bắt đầu từ Keyword Planner | Cảnh báo sai thứ tự. Bộ GEO → landing đang chạy → Planner chỉ để điền `volume`·`cpc` |
| Quyết ngân sách bằng chỉ số sớm | Từ chối. Time-on-site đẹp mà không ai đặt cọc **vẫn là trang hỏng** |
| Đọc báo cáo không có cột `market` | Nói thẳng báo cáo **không dùng được** thay vì kết luận trên số đã trộn thị trường |
