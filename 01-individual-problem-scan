# 01 — Individual Problem Scan

## Phase 1 — Scan rộng

Một số vấn đề của học viên và ban vận hành.

### A. Pain xuyên suốt buổi lab

| # | Lăng kính | Problem | Actor | Dấu hiệu thật (ước lượng, cần validate) |
|---|---|---|---|---|
| 1 | Pain từ người khác + AI có thể tốt hơn | Lúc cao điểm số câu hỏi vượt năng lực TA: học viên chờ lâu (đôi khi hết giờ chưa tới lượt), TA quá tải phải bỏ dở câu này nhảy câu kia | Học viên đang kẹt **và** trợ giảng | 3-4 TA cho cả lớp; hàng đợi dồn vào vài phase nặng; câu hỏi lặp lại |
| 2 | Lặp lại | Tìm lại câu trả lời/quyết định cũ trong Discord (deadline, cách nộp, lỗi đã fix, giải thích đề) | Cả lớp, đặc biệt người mới | Phải scroll nhiều kênh; cùng câu hỏi bị hỏi lại nhiều lần |
| 3 | Lặp lại + Pain từ người khác | Câu hỏi onboarding/hành chính lặp lại mỗi buổi/mỗi batch (deadline, link nộp, cấu trúc repo, cách dùng git) | Học viên mới **và** TA/staff | Cùng câu hỏi xuất hiện đều đặn; TA/staff trả lời trùng |
| 4 | AI có thể tốt hơn | Không biết bài nộp đã đủ field theo rubric chưa, đến lúc nộp mới phát hiện thiếu | Học viên | Mất điểm vì thiếu metric/boundary; phải tự dò rubric thủ công |
| 5 | Tốn thời gian + AI có thể tốt hơn | Kiến thức mỗi buổi lớn, nằm rải rác nhiều nguồn (slide, recording, notes, Discord) và không có bản cô đọng → khó ôn lại, dễ quên, khó áp dụng vào bài mới | Học viên | Phải xem lại recording dài; không có recap chuẩn; quên trước buổi sau |

### B. Quá trình học của học viên

| # | Lăng kính | Problem | Actor | Dấu hiệu thật |
|---|---|---|---|---|
| 6 | AI có thể tốt hơn | Học xong không có cách tự kiểm "mình đã hiểu chưa" trước khi sang phần mới | Học viên | Tự tin sai; tới lúc làm bài mới lộ chỗ chưa hiểu |
| 7 | Tốn thời gian + Pain từ người khác | Gap lý thuyết → thực hành, nặng hơn vì lớp chênh trình độ (có người non-tech và người tech) | Học viên, nhất là người non-tech | "Hiểu rồi mà không làm được"; loay hoay ở bước đầu tiên |

### C. Vấn đề riêng của trợ giảng / giảng viên / ban tổ chức

> Hai pain TA quá tải và câu hỏi hành chính lặp đã được gộp lên #1 và #3. Phần dưới là pain **chỉ thuộc về người vận hành**.

| # | Lăng kính | Problem | Actor | Dấu hiệu thật |
|---|---|---|---|---|
| 8 | Tốn thời gian | Chấm bài theo rubric thủ công cho nhiều học viên nên rất chậm → feedback về trễ, hết tác dụng | Giảng viên / người chấm | Feedback trả về khi lớp đã sang bài mới |
| 9 | AI có thể tốt hơn | Giảng viên thiếu tín hiệu sớm để biết ai đang đuối mà can thiệp kịp | Giảng viên + ban tổ chức | Tới lúc điểm thấp hoặc nghỉ học mới phát hiện, đã muộn |

## Phase 2 — Chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Chấm bài theo rubric thủ công (#8) | Actor rõ (giảng viên), workflow rõ, metric đo được (thời gian chấm/bài, độ trễ feedback), so sánh Rule/Workflow/Agent tốt | "Chất lượng feedback" khó đo; AI chấm lệch điểm người chấm tới đâu cần kiểm |
| 2 | Câu hỏi onboarding/hành chính lặp (#3) | Lặp lại nhiều, hợp Rule/retrieval, baseline non-AI (FAQ) rõ để đối chiếu | Ranh giới câu hành chính vs câu cần người; ai duy trì FAQ |
| 3 | Recap / cô đọng kiến thức mỗi buổi (#5) | Lặp lại sau mỗi buổi, metric đo được (thời gian ôn lại), có cả phương án process fix lẫn AI để so sánh | "Đủ tốt" của bản recap khó đo; ai kiểm recap trước khi dùng |



## Problem Card #1 — Chấm bài theo rubric thủ công

**Problem 1 câu:**
Giảng viên/người chấm phải đọc từng bài và đối chiếu với rubric nhiều mục cho cả lớp, nên chấm rất chậm và feedback về tay học viên thường trễ, mất tác dụng khi lớp đã sang bài mới.

**Actor:**
Giảng viên hoặc trợ giảng được giao chấm bài. (Học viên đau gián tiếp vì feedback về trễ.)

**Thời điểm / bối cảnh:**
Sau mỗi buổi lab, khi cả lớp nộp bài và số lượng bài lớn trong ngày.

**Current workflow:**

```text
1. Mở từng repo/bài nộp
2. Đọc bài, đối chiếu với từng mục rubric
3. Cho điểm từng mục + ghi nhận xét
4. Tổng hợp điểm + viết feedback        <-- bottleneck (lặp lại cho mỗi bài)
5. Trả điểm/feedback cho học viên
```

**Bottleneck:**
Bước 2-4 — đọc kỹ và đối chiếu rubric thủ công cho từng bài, nhân với số học viên thì tốn rất nhiều giờ.

**Impact:**
Ước lượng ~15-20 phút/bài × N học viên → nhiều giờ mỗi buổi. Feedback về trễ vài ngày, lúc đó học viên đã quên bài hoặc sang buổi mới nên ít cải thiện được.

**Success metric:**
Giảm thời gian chấm trung bình/bài từ ~15-20' xuống ~6-8' (giảm ~60%); rút độ trễ trả feedback từ vài ngày xuống trong 24h. Ràng buộc chất lượng: điểm sau khi giảng viên duyệt không lệch quá 1 mục rubric so với chấm tay thuần. (Baseline cần đo lại bằng một buổi thật.)

**Non-AI alternative:**
Auto-check phần cấu trúc bằng script (đủ file, đủ field, đúng cấu trúc repo) + rubric checklist rõ ràng. Giải quyết được phần "có/không đủ", nhưng chưa giúp đánh giá **chất lượng nội dung** (lập luận, metric, boundary).

**AI hypothesis:**
AI đọc bài + rubric, đề xuất **điểm nháp** từng mục kèm trích đoạn dẫn chứng và một bản nháp feedback; giảng viên review, chỉnh và chốt. AI không tự chốt điểm, không gửi thẳng cho học viên.

**Quick gut:** `Workflow`
# Current Workflow

### Description

* Thời gian xử lý trung bình: ~15-20 phút / bài
* Bottleneck chính:

  * Viết feedback thủ công cho từng bài
  * Quy trình lặp lại nhiều bước giống nhau

### Workflow Diagram

```text
┌───────────────┐
│ 1. Mở bài     │
│    ~1'        │
└──────┬────────┘
       │
       ▼
┌──────────────────────────┐
│ 2. Đọc + đối chiếu       │
│    rubric                │
│    ~8-10'                │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ 3. Cho điểm từng mục     │
│    ~3-4'                 │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ 4. Viết feedback         │
│    ~3-5'                 │
│    <-- bottleneck        │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ 5. Trả kết quả           │
│    ~1'                   │
└──────────────────────────┘
```

---

# Future Workflow

### Description

* Thời gian xử lý trung bình: ~6-8 phút / bài
* AI chỉ đóng vai trò hỗ trợ
* Quyết định cuối cùng luôn thuộc về giảng viên

### Workflow Diagram

```text
┌────────────────────────────────────┐
│ 1. Auto-check cấu trúc bằng script │
│    <1'                             │
│    -- Rule-based checking          │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 2. AI đề xuất điểm nháp            │
│    + dẫn chứng                     │
│    + draft feedback                │
│    ~1-2'                           │
│    -- AI hỗ trợ                    │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 3. Giảng viên review               │
│    + chỉnh                         │
│    + chốt điểm                     │
│    ~4-6'                           │
│    <-- human boundary              │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 4. Trả điểm / feedback trong 24h   │
└────────────────────────────────────┘
```

### Fallback Rules

```text
Fallback cases:
  ├─ AI chấm lệch
  ├─ Feedback quá nhạt / thiếu dẫn chứng
  └─ Giảng viên tự chấm lại mục đó

Rule:
  → Không bao giờ dùng điểm AI trực tiếp
    khi chưa được giảng viên duyệt.
```



## Problem Card #2 — Câu hỏi onboarding / hành chính lặp

**Problem 1 câu:**
Học viên (nhất là người mới hoặc đầu batch) hỏi đi hỏi lại cùng câu hành chính (deadline, link nộp, cấu trúc repo, cách dùng git), khiến TA/staff phải trả lời trùng nhiều lần và mất thời gian lẽ ra dành cho câu khó.

**Actor:**
TA/staff phải trả lời lặp, và học viên mới cần câu trả lời nhanh.

**Thời điểm / bối cảnh:**
Đầu mỗi buổi và đầu mỗi batch mới.

**Current workflow:**

```text
1. Học viên có câu hành chính
2. Hỏi trong Discord (hoặc hỏi trực tiếp TA)
3. TA/staff thấy → trả lời              <-- bottleneck (lặp lại, tốn người)
4. Vài hôm sau người khác hỏi lại y hệt
```

**Bottleneck:**
Bước 3 — người thật trả lời cùng nội dung nhiều lần thay vì câu trả lời tồn tại sẵn và tự phục vụ được.

**Impact:**
Mỗi câu ~2-5'/lần × nhiều người × nhiều batch; loãng kênh Discord; TA mệt; người mới phải chờ mới được làm tiếp.

**Success metric:**
≥70-80% câu hành chính phổ biến được trả lời ngay mà không cần người thật; giảm số câu hành chính gửi tới TA/staff; thời gian học viên có câu trả lời từ "chờ vài giờ" xuống gần như tức thì.

**Non-AI alternative (mạnh — phải thử trước):**
Kênh `#faq` được pin + tài liệu onboarding chuẩn + checklist "bắt đầu từ đâu". Nếu duy trì kỷ luật thì **Rule/curate giải quyết phần lớn**, chưa chắc cần AI.

**AI hypothesis:**
Nếu FAQ tĩnh không đủ (câu diễn đạt tự do, nhiều cách hỏi), thêm một bot retrieval trả lời từ tài liệu onboarding + FAQ kèm **link gốc**; câu ngoài phạm vi → chuyển người thật.

**Quick gut:** `Rule` trước, nâng lên `Workflow/retrieval` nếu cần.

# Current vs Future Q&A Workflow

### Current State

* Học viên hỏi trực tiếp trong Discord
* Phụ thuộc vào thời gian rảnh của TA
* TA phải trả lời lặp lại các câu giống nhau qua nhiều batch

### Current Workflow Diagram

```text id="k9d2f1"
┌──────────────────────────┐
│ Học viên hỏi trong       │
│ Discord                  │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ Chờ TA rảnh              │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ TA trả lời thủ công      │
│ cho từng câu hỏi         │
│                          │
│ <-- lặp mỗi batch        │
└──────────────────────────┘
```

---

# Future State

### Description

* FAQ bot xử lý các câu hỏi phổ biến
* Rule-based retrieval để trả lời nhanh
* Các trường hợp ngoài phạm vi sẽ được chuyển cho TA

### Future Workflow Diagram

```text id="m3p8q2"
┌────────────────────────────────────┐
│ 1. Học viên gõ câu hỏi             │
│    vào #faq / bot                  │
│    <1'                             │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 2. Bot trả về                     │
│    - câu trả lời cố định          │
│    - link tài liệu gốc            │
│    <1'                            │
│    -- Rule / retrieval            │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 3. Ngoài phạm vi                  │
│    → chuyển TA                    │
│    <-- human boundary             │
└────────────────────────────────────┘
```

### Fallback Rules

```text id="t8z7a4"
Fallback cases:
  ├─ Bot không chắc câu trả lời
  ├─ Không tìm thấy FAQ phù hợp
  └─ Câu hỏi quá đặc thù / mới

Rule:
  → Chuyển cho TA xử lý
  → Sau đó thêm câu mới vào FAQ.
```


> Phân biệt với #1 (TA lúc cao điểm) và #2 (Discord) trong scan: bài này là **câu hành chính có đáp án cố định** nên hợp Rule/FAQ nhất; khác câu kỹ thuật lúc đang kẹt (cần hiểu ngữ cảnh) và khác truy hồi quyết định cũ tự do trong Discord.

---

## Problem Card #3 — Recap / cô đọng kiến thức mỗi buổi

**Problem 1 câu:**
Mỗi buổi lượng kiến thức lớn và nằm rải rác nhiều nguồn (slide, recording, notes, Discord), không có bản cô đọng, nên học viên khó ôn lại, dễ quên và khó áp dụng vào bài mới.

**Actor:**
Học viên muốn ôn lại trước buổi/bài kế. (Người mới và người non-tech đau nhất.)

**Thời điểm / bối cảnh:**
Sau mỗi buổi và trước khi làm bài/buổi tiếp theo.

**Current workflow:**

```text
1. Sau buổi, cần ôn lại một ý
2. Lục slide / mở recording / tìm notes / search Discord
3. Tự ghép các mảnh rời rạc lại            <-- bottleneck
4. Tự viết tóm tắt (hoặc bỏ, dựa vào trí nhớ)
```

**Bottleneck:**
Bước 2-3 — gom nhiều nguồn rời rạc và xem lại recording dài để dựng lại một ý.

**Impact:**
Mỗi lần ôn ~30-60'; dễ quên; vào bài mới phải dò lại từ đầu; kiến thức không đọng lại theo thời gian.

**Success metric:**
Có bản recap cô đọng cho mỗi buổi trong vòng vài giờ sau buổi; giảm thời gian ôn lại một chủ đề từ ~30-45' xuống dưới ~10'. (Đo bằng thời gian tìm + tự đánh giá còn nhớ; baseline cần validate.)

**Non-AI alternative (mạnh):**
Mỗi buổi có một bản tóm tắt chuẩn do giảng viên/TA hoặc học viên luân phiên viết, kèm index tài liệu. Đây là một **process fix** đủ mạnh và đáng thử trước.

**AI hypothesis:**
AI tóm tắt slide/recording/notes thành recap có cấu trúc (ý chính, ví dụ, điểm cần nhớ) kèm link nguồn; người thật (TA hoặc học viên) kiểm trước khi dùng. AI chỉ cô đọng, không thay việc học.

**Quick gut:** `Process fix` trước; có thể nâng lên `Workflow` (AI tóm tắt + người kiểm).

# Current vs Future Review Workflow

### Current State

* Việc ôn lại một ý thường mất nhiều thời gian
* Thông tin bị phân tán:

  * slide
  * recording
  * notes
  * Discord
* Học viên phải tự tổng hợp và tự rút ý chính

### Current Workflow Diagram

```text id="v2k7m1"
┌──────────────────────────┐
│ Cần ôn lại 1 ý           │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ Lục slide / recording /  │
│ notes / Discord          │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ Tự ghép thông tin        │
└──────────┬───────────────┘
           │
           ▼
┌──────────────────────────┐
│ Tự tóm tắt / bỏ ý        │
│                          │
│ ~30-60'                  │
└──────────────────────────┘
```

---

# Future State

### Description

* Sau mỗi buổi sẽ có recap chuẩn hóa
* AI có thể hỗ trợ tóm tắt
* Người thật kiểm duyệt trước khi công bố
* Recap trở thành điểm truy cập chính để ôn tập nhanh

### Future Workflow Diagram

```text id="n8p3c4"
┌────────────────────────────────────┐
│ 1. Sau buổi: tạo recap chuẩn       │
│                                    │
│    - Process thủ công              │
│    HOẶC                            │
│    - AI hỗ trợ tóm tắt             │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 2. Người thật kiểm recap           │
│                                    │
│    - đúng ý                        │
│    - đủ điểm cần nhớ               │
│                                    │
│    <-- human boundary              │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 3. Đăng recap + link nguồn         │
│    vào một nơi cố định             │
└────────────────┬───────────────────┘
                 │
                 ▼
┌────────────────────────────────────┐
│ 4. Học viên ôn từ recap            │
│                                    │
│    Cần sâu hơn                     │
│    → lần theo link nguồn           │
│                                    │
│    <10'                            │
└────────────────────────────────────┘
```

### Fallback Rules

```text id="f5r9w8"
Fallback cases:
  ├─ Recap AI sai ý
  ├─ Bỏ sót điểm quan trọng
  ├─ Tóm tắt quá ngắn / thiếu context
  └─ Link nguồn không đầy đủ

Rule:
  → Người kiểm sửa recap
  → Không dùng recap chưa duyệt
    làm nguồn chính thức.
```
