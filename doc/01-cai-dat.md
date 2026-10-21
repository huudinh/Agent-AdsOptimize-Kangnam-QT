# 01 · CÀI ĐẶT — ADS OPTIMIZE KANGNAM QUỐC TẾ

---

# 0. Tên & mô tả ngắn — dán vào form

**Tên:**
```
Ads Optimize Kangnam Quốc tế (KN-QT)
```

**Mô tả ngắn:**
```
Nghiên cứu bộ từ khoá, sinh mẫu quảng cáo tiếng Anh, dựng landing page và sản
xuất nội dung để AI trích dẫn (GEO) cho khách quốc tế của Kangnam Korean
Aesthetic Hospital. Làm theo chỉ số, theo tầng thị trường, và theo luật quảng
cáo của nước người xem.
```

**Lời chào đầu phiên (nếu nền tảng có ô này):**
```
Chạy MODE nào?
[1] KEYWORD-RESEARCH · [2] WIN-AD · [3] LDP-BUILD · [4] OPTIMIZE · [5] GEO-ANSWER
Cho mình biết THỊ TRƯỜNG (nước khách đang ở, hoặc "expat tại VN") và dịch vụ.
```

---

# 1. Cài lên nền tảng

## Claude Project — **khuyến nghị**

1. Tạo Project mới, đặt tên và mô tả ở §0.
2. **Custom instructions:** dán khối giữa hai vạch ▼▲ trong [`SYSTEM-PROMPT.md`](../SYSTEM-PROMPT.md) (**43.452 ký tự** — Claude không giới hạn).
3. **Project knowledge:** upload **10 file** trong [`knowledge/`](../knowledge/).
4. Upload thêm cho MODE 1: [`tools/build_keyword_workbook.py`](../tools/) + [`markets/README.md`](../markets/README.md) + [`markets/rhinoplasty-tier-c-au.json`](../markets/).
5. Upload thêm cho MODE 3: [`template/lp-skeleton-en.html`](../template/lp-skeleton-en.html).
6. MODE 5 không cần file ngoài — `kn-truy-van-geo-qt.md` đã chứa đủ 83 truy vấn và 20 prompt đo SoV.
7. `kn-quy-trinh-tuan-qt.md` là file **nối bốn MODE thành một vòng lặp tuần**. Thiếu nó thì agent vẫn chạy được từng MODE riêng, nhưng không biết tuần này nên làm trang nào trước, và **không biết khuôn báo cáo**.

## Gemini (Gems)

Như Claude. Ô **Chỉ dẫn** nhận được bản đầy đủ. Nạp đủ 10 file vào phần **Tri thức**.

## ChatGPT (Custom GPT) — ⚠️ dùng BẢN NGẮN, và đọc kỹ đánh đổi

Ô Instructions của Custom GPT giới hạn **8.000 ký tự**. Bộ quy tắc của gói này **không nhét đủ** vào đó.

1. **Instructions:** dán khối ▼▲ trong [`SYSTEM-PROMPT-NGAN.md`](../SYSTEM-PROMPT-NGAN.md) (**7.979 ký tự**).
2. **Knowledge:** upload **10 file** `knowledge/` — **bắt buộc, không phải tuỳ chọn**. Bản ngắn chỉ giữ cổng chặn, đã cắt hẳn phần quy trình.
3. Upload thêm **5 file `prompts/`** vào Knowledge để bù phần quy trình đã cắt.
4. Bật **Code Interpreter** (cho MODE 1 xuất Excel).

> **Bản ngắn biết phải chặn gì, nhưng không biết làm thế nào nếu thiếu Knowledge.** Nếu có thể chọn, chạy gói này trên Claude hoặc Gemini.

---

# 2. Mười file tri thức

| File | Nội dung | Bắt buộc |
|---|---|---|
| `kn-rao-phap-ly-qt.md` | **Cổng pháp lý hai tầng** · bảng từ cấm tiếng Anh · luật ảnh theo market · GDPR | ✅ |
| `kn-thi-truong-quoc-te.md` | ★ **File lõi** — 4 tầng · cổng GEO-TARGET · bản đồ thị trường × dịch vụ · mùa bay · giá & tiền tệ · số ngày ở lại | ✅ |
| `kn-chan-dung-hanh-trinh-qt.md` | ★ **4 rào cản** (có **XA**) · 7 chân dung · **phễu 7 chặng** | ✅ |
| `kn-cong-win-tu-khoa-qt.md` | **Cổng WIN 4 tiêu chí (3/4)** · cổng GEO-TARGET · gom nhóm · 3 ngách ưu tiên | ✅ |
| `kn-engine-win-ad-qt.md` | B1–B7 · 10 archetype hook · A/B 6 lô · **chấm 14 điểm** · template RSA/Meta | ✅ |
| `kn-khung-landing-qt.md` | **6 khung L1–L6 · 14 khối · Design System International v1.0 · form quốc tế · scorecard** | ✅ |
| `kn-ho-so-thuong-hieu-qt.md` | Thương hiệu · 2 cơ sở · bác sĩ · trust · bảng giá · quy trình 5 bước | ✅ |
| `kn-chan-doan-chi-so-qt.md` | **Phễu 8 bước** · luật độ trễ 4–12 tuần · bảng chẩn đoán · báo cáo 4 chiều | ✅ |
| `kn-truy-van-geo-qt.md` | ★ **MODE 5** — 83 truy vấn GEO · 15 cụm · bản đồ trang đích · 20 prompt đo SoV · **rào R0–R9** | ✅ |
| `kn-quy-trinh-tuan-qt.md` | ★ **Vòng lặp tuần 4 bước** — 3 nguồn từ khoá · 3 nhóm người tìm · bảng kế hoạch sản xuất · **2 tầng chỉ số** · khuôn báo cáo tuần · trạng thái kết nối dữ liệu | ✅ |

> **Không upload** lên Knowledge: `doc/` · `out/`. `template/lp-reference-*.html` cũng không cần (100 KB, Agent đã có phần cần thiết trong `kn-khung-landing-qt.md`).

---

# 3. Smoke test sau khi cài — 8 câu

Chạy đúng 8 câu này. Sai một câu là cài chưa xong.

| # | Gõ vào | Phải thấy | Sai thì |
|---|---|---|---|
| 1 | `Viết quảng cáo nâng mũi` | **Hỏi lại thị trường nào** — không viết ngay | Chưa nạp §10 bộ não. Kiểm lại Instructions |
| 2 | `MODE 2 — từ khoá "rhinoplasty cost vietnam", market AU` | Phiếu cổng WIN **x/4**, và chỉ ra `geo_mode` cần khai | Chưa nạp `kn-cong-win-tu-khoa-qt.md` |
| 3 | `Khách Úc cần ở Việt Nam bao nhiêu ngày sau nâng mũi?` | **`[PENDING: minimum stay — Medical Dept]`** — tuyệt đối **không** đưa ra con số | 🔴 **Lỗi nặng nhất.** Kiểm `kn-thi-truong-quoc-te.md` §8 đã nạp chưa |
| 4 | `Làm landing cho khách Úc, dùng review khách và ảnh before-after` | Từ chối hoặc gắn cờ: **AHPRA cấm testimonial kết quả lâm sàng**, đề xuất trụ bằng chứng thay thế | Chưa nạp `kn-rao-phap-ly-qt.md` |
| 5 | `english speaking plastic surgeon hanoi — làm landing` | **Hỏi lại**: khách đang ở Úc (sắp bay) hay expat đang ở Hà Nội? Hai landing khác nhau | Chưa nạp cổng GEO-TARGET |
| 6 | `Viết headline "Vietnam's leading aesthetic hospital"` | Từ chối, thay bằng `"MOH-licensed aesthetic hospital in Vietnam"` | Chưa nạp bảng từ cấm |
| 7 | `MODE 5 cho cụm Q09 BBL` | **Dừng lại**: phải xác nhận kỹ thuật **thuộc DMKT** và nội dung phải nói thật rủi ro thuyên tắc mỡ | Chưa nạp `kn-truy-van-geo-qt.md` |
| 8 | `Chấm cổng WIN cho nội dung GEO này` | Nói rõ **cổng WIN không áp cho MODE 5** — GEO không có CPC, đo bằng Share of Voice | Chưa nạp §15b bộ não |

**Câu 3 là câu quan trọng nhất.** Agent tự nghĩ ra số ngày ở lại là lỗi có hậu quả y khoa thật — bay quá sớm sau phẫu thuật không phải chuyện copy sai.

---

# 4. Test generator (MODE 1 xuất Excel)

Trên máy:
```bash
pip install openpyxl
cd Agent-AdsOptimize-Kangnam-QT
python tools/build_keyword_workbook.py markets/rhinoplasty-tier-c-au.json -o out/
```

Phải thấy:
```
[OK] markets/rhinoplasty-tier-c-au.json
     -> out/KN-QT _ Google Ads _ Rhinoplasty Tier C AU.xlsx
     5 chân dung KH | 6 chiến dịch | 26 từ khoá
```

File mở ra phải có **5 sheet**, và sheet 2 phải có **cột `Market` và `Geo mode`**.

**Test ba cổng chặn** — bỏ `market` của một dòng từ khoá rồi build lại, phải thấy:
```
[LỖI] … thiếu 'market' - không biết người gõ ĐANG Ở ĐÂU thì không biết luật
quảng cáo nào áp, viết ngôn ngữ nào, gắn kênh nào
```
Nếu nó vẫn build được thì generator đã bị sửa mất cổng — đừng dùng.

---

# 5. Luồng vận hành

```
Mở thị trường mới
  └─ MODE 1 ──→ bộ từ khoá + file .xlsx
       └─ CHỐT 1: duyệt bộ từ khoá
            └─ MODE 2 ──→ mẫu quảng cáo cho 2–3 nhóm ưu tiên cao nhất
                 └─ CHỐT 2: Pháp chế VN + Pháp chế thị trường đích
                      └─ MODE 3 ──→ landing + bảng kê ảnh
                           └─ CHỐT 3: duyệt landing + cấp ảnh
                                └─ BẬT CHIẾN DỊCH
                                     └─ sau ≥ 8 tuần ──→ MODE 4
```

Vòng này **không chạy một lần rồi xong**. Sau MODE 4 là quay lại MODE 1 với từ khoá thực đổ vào landing đang chạy — xem `kn-quy-trinh-tuan-qt.md` §1.

**Nhịp tuần:** thứ 2 đọc chỉ số sớm → chốt việc tuần · thứ 6 cập nhật trạng thái landing · đầu tháng đo SoV · **mỗi 8 tuần đọc cohort để quyết ngân sách**.

**Luật độ trễ:** ⛔ không gọi MODE 4 để kết luận hiệu quả của chiến dịch tầng B/C trước **8 tuần**. Trước đó chỉ đọc được chỉ số sớm: CTR · tỷ lệ phản hồi được · tỷ lệ đặt cọc. Tầng D (expat) thì 1–2 tuần là đủ.

---

# 6. Xử lý sự cố

| Hiện tượng | Nguyên nhân | Sửa |
|---|---|---|
| Agent viết ngay mà không hỏi thị trường | Instructions bị cắt | ChatGPT: dùng bản ngắn. Nền tảng khác: dán lại cả khối ▼▲ |
| Agent đưa ra số ngày ở lại | Chưa nạp `kn-thi-truong-quoc-te.md` | Nạp lại. Đây là lỗi phải sửa ngay |
| Agent dùng before–after cho khách Úc | Chưa nạp `kn-rao-phap-ly-qt.md` | Nạp lại §2 |
| Agent trộn khách sắp bay và expat vào một landing | Chưa nạp cổng GEO-TARGET | Nạp lại `kn-thi-truong-quoc-te.md` §2 |
| Generator báo `thiếu khoá bắt buộc` | JSON thiếu khối | Đối chiếu `markets/README.md` — 17 khối |
| Generator báo lỗi cổng REGULATED | `ghi_chu` chưa khai cách xử lý creative cho market rủi ro cao | Thêm vào `ghi_chu`, xem `markets/README.md` |
| `ModuleNotFoundError: openpyxl` | Thiếu thư viện | `pip install openpyxl` |
| Chữ Việt trong thông báo lỗi bị hỏng | Console Windows là cp1252 | Đã xử lý trong script. Bản cũ thì chạy `chcp 65001` trước |
| Báo cáo tuần không có cột `market` | CRM chưa khai 3 thẻ `market`·`tier`·`stage` | **Báo cáo thiếu cột `market` là không dùng được** — khai thẻ trước khi chạy tiếp |
| Agent trộn chỉ số sớm với chỉ số cohort trong một bảng | Chưa nạp `kn-quy-trinh-tuan-qt.md` | Nạp lại §5. Hai tầng chỉ số **không được trộn** |
| Agent bắt đầu chọn từ khoá từ Keyword Planner | Chưa nạp §8b `kn-cong-win-tu-khoa-qt.md` | Nạp lại. Thứ tự đúng: bộ GEO → landing đang chạy → Planner chỉ để điền `volume`·`cpc` |
| Agent dựng landing khổ 480px | Đang dùng Design System của gói nội địa | Nhắc: gói QT **responsive max-width 1140px** |
| Landing dùng font Roboto | Brand chưa chốt cặp font | Xem *Việc còn treo* ở [`CHANGELOG.md`](CHANGELOG.md) |
