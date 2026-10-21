# PROMPT MẪU — MODE 5 · GEO-ANSWER (nội dung để AI trích dẫn)

> Dùng khi: muốn **AI trích dẫn Kangnam** khi khách nước ngoài hỏi ChatGPT · Gemini · AI Overview bằng tiếng Anh.
> Nguồn: [`knowledge/kn-truy-van-geo-qt.md`](../knowledge/kn-truy-van-geo-qt.md) — **83 truy vấn · 15 cụm · 53 CORE**.
> Đo bằng **Share of Voice**, không bằng CPL. Mục tiêu quý: **SoV ≥ 30%** ở cụm Tầng A.

## ⚠️ Đây là kênh khác, không phải quảng cáo

| | Ads (MODE 1–4) | **GEO (MODE 5)** |
|---|---|---|
| Đo bằng | CPL · chi phí/khách đến khám | **Share of Voice** |
| Nhịp | Tuần · cohort 8 tuần | **Quý** |
| Khung viết | **AIDA** (L1–L6) | **PAS** |
| `market` / `geo_mode` | ✅ bắt buộc | ⛔ **không có** |
| Cổng WIN 3/4 | ✅ | ⛔ không áp |

⛔ Đừng hỏi Agent chấm cổng WIN hay gắn `market` cho nội dung GEO — AI không có geo-targeting và không có CPC.

---

## 1 · PROMPT CHÍNH — làm một cụm

```
MODE 5 — GEO-ANSWER.

Cụm: [vd Q13 · Medical tourism logistics]
     (hoặc chỉ nói tên dịch vụ, Agent tự map sang cụm và nói rõ đã map vào đâu)

Làm theo G1→G7:

G1 · Xác nhận cụm + tầng ưu tiên. Nếu cụm này KHÔNG thuộc Tầng A mà 4 cụm
     Tầng A (Q10 · Q12 · Q11 · Q13) chưa làm xong → NÓI RÕ là đang đi sai thứ tự,
     và cho tôi biết vì sao thứ tự đó quan trọng.
G2 · Liệt kê các truy vấn CORE của cụm, nguyên văn tiếng Anh.
G3 · Với từng truy vấn, đọc cột "Khối trả lời cần có" — đó là brief, không phải
     gợi ý. Nêu luôn từ khoá ưu tiên và trang đích.
G4 · Rà mã rào R# của TỪNG truy vấn TRƯỚC KHI VIẾT. Nêu rõ: rào nào chạm,
     không được viết gì, thay bằng gì. (Rà sau là phải viết lại.)
G5 · Viết nội dung EN cho trang đích, khung PAS. Mỗi truy vấn là một H2/H3
     dùng ĐÚNG câu khách gõ, và trả lời ngay trong 2–3 câu đầu.
G6 · Tự soát R1 (cam kết kết quả) + R2 (DMKT) + R3 (pháp nhân) + R7 (thiết bị/
     số lưu hành) + R8 (KCB cho người nước ngoài) + R9 (bản EN vẫn cần GXNNDQC).
G7 · Ghi lại prompt đo SoV tương ứng và tháng sẽ đo lại.

Cuối cùng: danh sách [PENDING] nêu rõ AI CẤP.
```

---

## 2 · PROMPT NGẮN

```
MODE 5 cho cụm [Qxx]. Rà rào pháp lý trước khi viết.
```

---

## 3 · PROMPT SÓNG 1 — bốn cụm Tầng A

```
MODE 5 — Sóng 1, 90 ngày, 70% ngân sách EN.

Làm kế hoạch cho đúng 4 cụm Tầng A, theo thứ tự ưu tiên:
  Q10 · Choosing a hospital & surgeon   (15,5% điểm)
  Q12 · Safety, accreditation & licensing (12,8%)
  Q11 · Cost & price transparency (USD)   (11,7%)
  Q13 · Medical tourism logistics         (6,9%)

Với mỗi cụm cho tôi: số truy vấn CORE · trang đích · dạng nội dung cần sản xuất
· rào pháp lý phải qua · dữ liệu còn thiếu.

Nói rõ cụm nào BỊ CHẶN vì thiếu dữ liệu, và ai phải cấp dữ liệu đó.
⛔ Chưa cần viết nội dung ở bước này — tôi cần kế hoạch và danh sách chặn trước.
```

> Trang `/medical-tourism-guide` (Q13) cần **số ngày ở lại** — vẫn `[CHỜ CẬP NHẬT]`. Agent phải nêu điều này, không được viết bằng số tự suy.

---

## 4 · PROMPT ĐO SoV hằng tháng

```
MODE 5 — đo Share of Voice tháng [MM/YYYY].

Cho tôi 20 prompt đo ở dạng danh sách để tôi dán lần lượt, kèm hướng dẫn:
chế độ ẩn danh · ngôn ngữ giao diện EN · VPN/IP thị trường mục tiêu.

Rồi cho tôi khuôn bảng ghi kết quả: ChatGPT / Gemini / AI Overview
+ cột "đối thủ được AI nhắc".

Nhắc tôi vì sao cột đối thủ là cột quan trọng nhất.
```

**Bảng ghi kết quả:**

| # | Prompt | Cụm | ChatGPT | Gemini | AI Overview | Số nền tảng nhắc | Đối thủ AI nhắc |
|---|---|---|---|---|---|---|---|

`SoV = (số prompt có nhắc Kangnam) / (tổng số prompt)` — tính riêng từng nền tảng.

---

## 5 · PROMPT RÀ NỘI DUNG EN ĐÃ CÓ

```
Rà bài EN này theo bộ truy vấn GEO. Kiểm 7 điểm:

1. Bài trả lời truy vấn nào trong 83 truy vấn? Nếu không khớp cái nào →
   nói thẳng là bài này không phục vụ cụm nào.
2. Tiêu đề H2/H3 có dùng ĐÚNG câu khách gõ không, hay đang viết kiểu marketing?
3. Câu trả lời có nằm trong 2–3 câu đầu sau tiêu đề không?
4. Có đoạn nào là tính từ rỗng (AI không bao giờ trích) thay vì dữ kiện
   kiểm chứng được?
5. Rào R1 — còn "permanent" / "lifetime" / "100% safe" / "no scars"?
6. Rào R2/R3/R7 — có nêu kỹ thuật ngoài DMKT · gộp pháp nhân · thiết bị không
   rõ số lưu hành?
7. Bài có dùng khung AIDA (sai) thay vì PAS (đúng cho GEO)?

Xuất bảng: lỗi · vị trí · sửa thành gì. Rồi viết lại đoạn yếu nhất.
```

---

## 6 · PROMPT HỎI ĐÁP

```
Vì sao Tầng A là 4 cụm ngang dịch vụ, không phải trang dịch vụ?
```
```
Cụm nào đang bị chặn vì chưa chốt được điều kiện pháp lý, và chốt với ai?
```
*(Đáp án đúng: **Q08 Dental** — pháp nhân RHM · **Q09 BBL** — kỹ thuật có trong DMKT không + phải nói thật rủi ro thuyên tắc mỡ.)*
```
Rào R8 là gì và vì sao nó khác các rào còn lại?
```
*(Đáp án đúng: R2/R3/R7 nói về **câu chữ**; R8 nói về **điều kiện hoạt động** — có được tiếp nhận khách quốc tế hay không.)*

---

## Checklist nghiệm thu

☐ Mở đầu bằng `Cụm · Tầng · Giai đoạn GEO · Rào R#` *(không phải `Market · geo_mode` — đó là của kênh ads)*
☐ Nếu làm cụm Tầng B/C/D trước khi xong Tầng A → Agent **đã cảnh báo**
☐ Mỗi truy vấn có **mã rào R#**, và rà rào **trước khi viết**
☐ Tiêu đề `H2`/`H3` dùng **đúng câu khách gõ**, không nhồi từ khoá
☐ Câu trả lời nằm trong **2–3 câu đầu** sau tiêu đề
☐ Khung **PAS**, không phải AIDA
☐ Nội dung là **dữ kiện kiểm chứng được**, không phải tính từ
☐ Đã soát **R1 · R2 · R3 · R7 · R8 · R9**
☐ Có **prompt đo SoV** tương ứng + tháng sẽ đo lại
☐ Danh sách `[PENDING]` nêu rõ **ai cấp**
☐ ⛔ Không chấm cổng WIN, không gắn `market`/`geo_mode`, không đo bằng CPL
