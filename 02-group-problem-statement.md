# Phase 3 — Group Convergence: Từ 12 Candidates về 1

## Bước 3.1 — Trình bày top 3
Mỗi thành viên trong nhóm trình bày các candidate problems từ lăng kính và trải nghiệm thực tế của mình để cả nhóm cùng ghi nhận.

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|---|
| 1 | Thành viên 1 | Đánh giá thủ công sự thay đổi của văn bản luật | Sinh viên làm đồ án RAG | Đọc đối chiếu 2 bản PDF hành chính tốn 2-3 tiếng | Rất cụ thể, tính ứng dụng kỹ thuật cao |
| 2 | Thành viên 1 | "Bơi" trong tài liệu công nghệ (Documentation) | Thực tập sinh mới | Mất 2-3 ngày đọc tài liệu và tự search lỗi cấu hình | Context rộng, quy trình mang tính khám phá |
| 3 | Thành viên 1 | Đánh giá chất lượng câu trả lời của Chatbot RAG | Sinh viên, AI Developer | Ngồi đọc và chấm điểm thủ công từng câu (45-60 phút) | Workflow rất chặt, đậm chất kỹ thuật AI |
| 4 | Thành viên 2 | Tìm phòng trọ quanh khu Vinhomes | Sinh viên, Intern | Tin đăng hết phòng chưa xóa, ảnh khác thực tế | Bài toán consumer quen thuộc nhưng khó verify data |
| 5 | Thành viên 2 | Chọn đồ ăn trong canteen mất thời gian | Sinh viên, NV văn phòng | Thiếu thông tin realtime về độ đông và giá | Tần suất lặp lại cao, thiên về bài toán Rule |
| 6 | Thành viên 2 | Giá đồ ăn nội khu quá cao | Cư dân, sinh viên | Mất thời gian so sánh giá và tìm combo lợi nhất | Thiên về hướng xây dựng app/web so sánh giá |
| 7 | Thành viên 3 | Review Problem Card của học viên | Lab Coach | Phải kiểm tra thủ công các lỗi lặp lại, thiếu field | Workflow cực kỳ rõ, có sẵn data mẫu tại lớp |
| 8 | Thành viên 3 | Ghép nhóm học viên làm dự án | BTC, Lab Coach | Đọc hồ sơ và đánh giá năng lực thủ công số lượng lớn | Workflow ngắn, mang tính chất thuật toán gom cụm |
| 9 | Thành viên 3 | Theo dõi học viên có nguy cơ bỏ cuộc | Lab Coach | Tổng hợp dữ liệu thủ công từ nhiều nguồn LMS/Git | Bài toán dự đoán rủi ro tốt nhưng khó thu thập data |
| 10| Thành viên 4 | Weekly review report | Nhân viên, Manager | Nhân viên giấu review để bảo vệ bản thân | Đau đớn thật nhưng rào cản tâm lý khó giải bằng AI |
| 11| Thành viên 4 | Cost report | Nhân viên tài chính | Tối ưu hóa việc viết báo cáo thu nhập, độ chính xác | Thiên về tính chính xác số liệu, nặng về Rule |
| 12| Thành viên 4 | Food waste | Quán ăn, Khách hàng | Xu hướng khách hàng ăn gì biến động liên tục | Bài toán dự báo chuỗi thời gian, khó giải quyết trong lab |

---

## Bước 3.2 — Gom trùng / cluster
Nhóm tiến hành phân loại các ý tưởng trùng lặp hoặc có cùng bản chất thành các cụm (clusters) để dễ dàng đánh giá.

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| **A. Tóm tắt & Đối chiếu văn bản** | Candidate 1, 2, 7 | Gom thông tin từ các nguồn tài liệu (Luật, Doc công nghệ, Bài nộp học viên) để đối chiếu, kiểm tra checklist hoặc bóc tách thay đổi. | Workflow có tính cấu trúc rất cao, AI can thiệp tốt ở bước xử lý ngôn ngữ. |
| **B. Đánh giá & Giám sát hệ thống** | Candidate 3, 9 | Chạy script kiểm thử tự động, thu thập log/dữ liệu để chấm điểm chất lượng hoặc đưa ra cảnh báo sớm. | Thuần kỹ thuật dữ liệu, cần bộ tiêu chí chấm điểm/đánh giá rất rõ ràng. |
| **C. Tìm kiếm & Đề xuất đời sống** | Candidate 4, 5, 6, 12 | Tổng hợp dữ liệu từ các nguồn consumer (phòng trọ, đồ ăn nội khu, canteen) để match theo nhu cầu người dùng. | Impact diện rộng nhưng rủi ro lớn về tính chính xác của data đầu vào (realtime data). |
| **D. Vận hành & Viết báo cáo** | Candidate 8, 10, 11 | Các quy trình nội bộ doanh nghiệp hoặc lớp học (ghép nhóm, viết báo cáo tuần, báo cáo chi phí). | Dễ bị giải quyết bằng Rule hoặc phụ thuộc vào yếu tố con người quá nhiều. |

---

## Bước 3.3 — Shortlist
Nhóm loại bỏ các bài toán quá rộng, thiếu evidence hoặc khó tiếp cận dữ liệu, giữ lại 3 bài toán đáp ứng tốt nhất tiêu chí của lớp học.

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| **Review Problem Card của học viên (C7)** | Workflow 10 bước cực kỳ rõ ràng, giải quyết nỗi đau lặp đi lặp lại của Coach ngay tại lớp học, dễ lấy data mẫu để validate. | Cần xây dựng một Prompt gác cổng chuẩn để không bị bắt lỗi sai/sót tiêu chí của học viên. |
| **Đánh giá chất lượng Chatbot RAG (C3)** | Tận dụng tốt năng lực chuyên môn AI của nhóm sinh viên năm cuối, quy trình kỹ thuật khép kín và có metric thời gian sờ nắn được. | Chưa chắc chắn cách thiết kế bộ câu hỏi mẫu (Gold Dataset) ban đầu sao cho khách quan. |
| **Tìm phòng trọ quanh Vinhomes (C4)** | Ý tưởng gần gũi với đời sống sinh viên, pain bộc lộ rất rõ qua việc mất nhiều ngày đi xem phòng thực tế. | Dữ liệu từ các group Facebook và môi giới rất hỗn loạn, cực khó để "auto-pull" data sạch về cho AI xử lý. |

---

## Bước 3.4 — Score để đồng thuận
Nhóm tiến hành chấm điểm các ứng viên shortlist theo thang điểm từ 1 đến 5 để đưa ra quyết định cuối cùng.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Review Problem Card** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **Đánh giá Chatbot RAG** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **Tìm phòng trọ Vinhomes** | 4 | 4 | 4 | 4 | 3 | 4 | 4 | **27** |

### Kết quả thảo luận và chốt ứng viên cuối cùng:

* **Candidate nhóm chọn:** **Review Problem Card của học viên**
* **Vì sao chọn:** Đây là bài toán đạt điểm tuyệt đối và mang lại sự hào hứng nhất cho cả nhóm khi thảo luận. Bài toán có actor (Lab Coach) và workflow vận hành cực kỳ cụ thể. Lợi thế lớn nhất là nhóm có thể tương tác và validate trực tiếp với các Coach đang ngồi trong lớp để hoàn thiện metric, đồng thời dữ liệu mẫu (các file Problem Card lỗi/thiếu field) có sẵn ngay tại chỗ. Ranh giới giữa Rule (quét từ khóa thiếu field) và AI Workflow (đọc hiểu xem bottleneck có khớp với metric không) cực kỳ đẹp và trực quan.
* **Vì sao không chọn các candidate còn lại:**
  * *Tìm phòng trọ Vinhomes:* Bị loại vì rào cản kỹ thuật ở bước thu thập dữ liệu (Data Access) quá lớn. Việc quét bài đăng tự động từ Facebook/Zalo rất dễ bị chặn và dữ liệu rác/môi giới ảo quá nhiều.
  * *Đánh giá Chatbot RAG:* Dù đạt điểm tuyệt đối về mặt kỹ thuật, nhưng nhóm nhận thấy đề tài này hơi mang tính "cá nhân" phục vụ đồ án đơn lẻ, trong khi bài toán Review Problem Card mang tính tương tác tập thể và giúp nhóm dễ trình bày, thuyết phục người nghe hơn trong buổi bảo vệ lab.
* **Nếu có disagreement, nhóm xử lý thế nào:** Ban đầu nhóm chia làm hai phe (phe thích làm kỹ thuật RAG và phe thích làm bài toán ứng dụng Review Card). Nhóm đã xử lý bằng cách bỏ phiếu dựa trên tiêu chí "Khả năng thu thập data ngay trong 4 tiếng của buổi lab". Do bài toán Review Card có sẵn data là các file bài tập hiện tại của các nhóm khác, nhóm đã đạt được sự đồng thuận 100% chuyển sang chọn đề tài này.

---

# Phase 4 — Quick Validation + Research giải pháp (30')

## Mục tiêu

Sau khi chọn candidate problem, nhóm cần kiểm tra nhanh:

- pain có thật không,
- người khác có gặp không,
- đã có giải pháp nào tương tự chưa,
- bài toán có nên giải bằng AI không.

# Phase 4 — Quick Validation + Research giải pháp

## Bước 4.1 — Quick validation
Nhóm đã tiến hành phỏng vấn nhanh (Quick Interview) ngay tại lớp học với 2 Lab Coach đang chịu trách nhiệm chấm bài cho các nhóm để thu thập tín hiệu thực tế.

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Interview Lab Coach** | 2 Coach | 100% Coach xác nhận cực kỳ ngán bước check checklist thủ công (thiếu field, sai format, metric không đo được).<br>• Trung bình mất 10-15 phút/bài do phải viết feedback giải thích lỗi lặp đi lặp lại. | Có những bài học viên viết đúng format nhưng ý tưởng quá vĩ mô/phi thực tế, AI khó mà bắt hết được nếu không có chuyên môn sâu. | Thu hẹp bài toán: Không bắt AI thay Coach chấm điểm ý tưởng tốt/xấu, mà biến AI thành **"Gác cổng Checklist & Tính Logic"** (Check đủ 6 field, đối chiếu logic giữa Bottleneck và Metric). |

---

## Bước 4.2 — Research giải pháp đã có
Nhóm tìm kiếm các pattern gác cổng dữ liệu văn bản và chấm bài tự động hiện nay.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **GitHub Actions Linter / Markdownlint** | https://github.com/marketplace/actions/markdown-lint | Tự động check format file `.md`, cấu trúc heading, và các ký tự đặc biệt. | Chạy cực nhanh, chính xác 100% về mặt định dạng, không tốn chi phí API. | Chỉ check được cú pháp (syntax), hoàn toàn không hiểu được ngữ nghĩa (semantics) học viên viết gì. | Dùng Rule-based (Regex/Linter) để check cấu trúc file trước khi gọi AI. |
| **Grader AI / LLM-as-a-Judge Pattern** | https://arxiv.org/abs/2306.05685 | Dùng một LLM lớn để chấm điểm và viết nhận xét cho một văn bản/bài luận dựa trên tiêu chí (rubric) có sẵn. | Hiểu được ngữ cảnh, phát hiện tốt các câu văn mơ hồ, viết được feedback chi tiết bằng tiếng Việt. | Rủi ro bị "ảo tưởng" (hallucination), chấm điểm không nhất quán giữa các lần chạy nếu prompt không chặt. | Cần thiết kế System Prompt dạng cấu trúc nghiêm ngặt (JSON Output) và ép AI trích dẫn câu lỗi của học viên. |



# Phase 5 — Workflow + Problem Statement

## Bước 5.1 — Current workflow bản nhóm
Quy trình chấm bài thủ công hiện tại của các Lab Coach khi chưa có sự hỗ trợ của AI. (Xem sơ đồ Mermaid riêng đính kèm trong thư mục dự án).

### Chi tiết các bước hiện tại:
| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|
| **1. Mở bài** | Lab Coach | Link Repo GitHub của học viên. | Giao diện Markdown bài nộp hiển thị trên màn hình. | 1 phút / bài | Thao tác thủ công lặp đi lặp lại. |
| **2. Check Checklist** | Lab Coach | Nội dung văn bản Problem Card. | Danh sách các field bị thiếu hoặc viết sai format. | 3 phút / bài | **Bottleneck 1**: Cực kỳ nhàm chán khi phải đếm xem bài có đủ 6 fields không. |
| **3. Đọc hiểu & Check Logic** | Lab Coach | Các phần: Actor, Bottleneck, Metric, Boundary. | Đánh giá bài toán có thật, có mơ hồ hay không. | 5 phút / bài | **Bottleneck 2**: Tốn nhiều "não" để phát hiện xem Metric đã đo được chưa. |
| **4. Viết Feedback** | Lab Coach | Đánh giá cá nhân của Coach. | Đoạn văn bản nhận xét bằng tiếng Việt. | 5 phút / bài | **Bottleneck 3**: Phải gõ đi gõ lại các câu nhắc nhở lỗi cơ bản. |

---

## Bước 5.2 — Future workflow bản nhóm
Quy trình tối ưu hóa áp dụng mô hình "Gác cổng AI" (Human-in-the-loop). (Xem sơ đồ Mermaid riêng đính kèm trong thư mục dự án).

### So sánh tác động Before/After:
| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| **Tổng thời gian review** | 10 - 15 phút / bài | **Dưới 3 phút / bài** | Target chính của toàn bộ pipeline. |
| **Số bước của Coach** | 5 bước thủ công | 2 bước (Review Draft -> Chốt) | Giảm tải 80% thao tác lặp lại. |
| **Tỷ lệ bài lỗi cơ bản tới tay Coach** | 40% số bài nộp | **0%** (Bị AI gác cổng block từ đầu) | Coach chỉ nhận các bài đã đủ chất lượng. |
| **Risk mới** | Không có rủi ro công nghệ | Rủi ro AI chấm quá lỏng tay hoặc hallucination | Cần Coach kiểm soát ở bước cuối. |

---

## Bước 5.3 — Problem Statement v0
| Field | Nội dung |
|---|---|
| **Actor** | Lab Coach phụ trách review bài tập cho học viên. |
| **Workflow** | Học viên nộp bài -> Coach mở bài -> Check checklist -> Đọc check logic -> Viết feedback -> Trả bài. |
| **Bottleneck** | Bước kiểm tra checklist thủ công và viết đi viết lại các câu feedback lỗi cơ bản mất rất nhiều thời gian. |
| **Impact** | Tốn 10-15 phút cho một bài, khiến tốc độ trả bài cho học viên bị chậm, Coach bị quá tải nhận thức. |
| **Success Metric** | Giảm thời gian chấm bài từ 10 phút xuống dưới 3 phút; giảm 50% số bài bị trả lại do lỗi cơ bản. |
| **Boundary** | AI không được tự ý chấm điểm; không tự động trả bài nếu chưa qua bộ lọc rule; không thay thế quyết định cuối của Coach. |



---


# Phase 6 — Rule / Workflow / Agent + Decision

## Bước 6.0 — Ma trận độ phù hợp với AI
* **Độ mơ hồ:** **Trung bình - Cao**. Việc đếm số lượng field thì độ mơ hồ thấp (Rule giải được), nhưng việc đọc hiểu xem một câu Metric viết đã "đo lường được chưa" (độ mơ hồ cao) đòi hỏi khả năng xử lý ngôn ngữ tự nhiên.
* **Độ phức tạp:** **Thấp - Trung bình**. Quy trình chấm bài diễn ra theo tuyến tính thẳng, không có nhiều nhánh rẽ phức tạp hay đòi hỏi gọi nhiều công cụ bên ngoài cùng lúc.
* **Kết luận:** Bài toán nằm ở ô **Workflow có AI hỗ trợ một vài bước ngôn ngữ cụ thể** là hoàn toàn đủ và tối ưu nhất.

---

## Bước 6.1 — So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Dùng Regex/Script quét file để đếm số lượng headings (`#`, `##`) xem đủ 6 fields không. | Đủ nếu học viên chỉ hay quên điền field, format bài nộp bị lộn xộn. | Không check được nội dung bên trong (Ví dụ: Học viên bỏ trống hoặc viết chữ "A" đối phó). | **Có sử dụng** (Làm bộ lọc thô ở bước đầu tiên). |
| **Workflow** | Script check cấu trúc -> API AI đọc hiểu nội dung & Draft feedback -> Đẩy về giao diện cho Coach duyệt. | **Đủ và hợp lý nhất** vì quy trình cố định, AI chỉ tập trung mạnh vào bước ngôn ngữ (đối chiếu logic và sinh feedback văn bản). | AI có thể viết nhận xét hơi rập khuôn hoặc bỏ sót lỗi ngữ nghĩa sâu xa. | ⭐ **CHỌN PHƯƠNG ÁN NÀY** |
| **Agent** | Xây dựng một Agent tự động đi "ping" từng học viên trễ hạn, tự thảo luận với học viên trên Discord để giải thích lỗi, tự động update bảng điểm. | Chỉ cần khi muốn tự động hóa toàn bộ việc vận hành và giao tiếp của một lớp học. | Quá rộng, vi phạm phân quyền dữ liệu, rủi ro giao tiếp sai lệch với học viên cao. | **Không chọn** (Quá phức tạp so với quy mô buổi Lab). |

---

## Bước 6.2 — Problem Statement v1
| Field | Nội dung |
|---|---|
| **Actor** | Lab Coach phụ trách chấm bài Problem Card của học viên. |
| **Workflow** | Học viên đẩy bài lên GitHub -> Hệ thống tự động kích hoạt pipeline -> AI đánh giá thô -> Coach duyệt feedback cuối -> Trả bài. |
| **Bottleneck** | Bước rà soát checklist thủ công và gõ các câu nhận xét lỗi cơ bản (thiếu metric, sai actor) tốn 8-10 phút của Coach. |
| **Impact** | Gây nghẽn tiến độ trả bài, Coach mệt mỏi dẫn đến chất lượng feedback các bài sau bị giảm sút. |
| **Success Metric** | Thời gian Coach bấm duyệt feedback dưới **3 phút/bài**; 100% bài nộp đến tay Coach đều điền đủ thành phần quy định. |
| **Boundary** | AI không được tự động cho điểm số; không tự gửi feedback thẳng cho học viên mà bắt buộc phải qua giao diện duyệt của Coach. |
| **AI intervention point** | **Sau khi bài nộp vượt qua vòng quét Rule-based về mặt cấu trúc**, AI can thiệp ngay trước bước Coach phải đọc bài để tự động tạo bản nháp nhận xét (Draft Feedback). |
| **Mức chọn** | **Workflow** (Phối hợp giữa Rule-based gác cổng format và GenAI gác cổng ngữ nghĩa). |
| **Rủi ro & người thật kiểm tra** | **Rủi ro:** AI hallucination (báo lỗi sai dù học viên viết đúng). **Người thật kiểm tra:** Coach bắt buộc phải đọc lướt qua bài và nhấn nút "Approve" hoặc chỉnh sửa lại câu chữ của AI trước khi gửi đi. |

---

## Bước 6.3 — Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor và workflow đã rõ chưa? | **YES** | Thể hiện chi tiết qua quy trình chấm bài 10 bước của Coach. |
| Baseline và success metric đã đo được chưa? | **YES** | Đo bằng số phút chấm bài (10 phút giảm xuống dưới 3 phút). |
| Có data/input đủ dùng chưa? | **YES** | Dùng chính các file bài tập Markdown của các nhóm trong lớp làm dữ liệu mẫu. |
| Nếu AI sai, hậu quả có chấp nhận được không? | **YES** | Biện pháp duy trì Coach gác cổng duyệt cuối bảo vệ bài thi của học viên. |
| Có người review/owner vận hành không? | **YES** | Chính các thành viên trong nhóm đóng vai trò vận hành và các Coach hỗ trợ. |
| Có cách non-AI đơn giản hơn không? | **NO** | Biện pháp Checklist/Template đã dùng nhưng học viên vẫn thường xuyên viết sai logic phần Metric. |

* **Decision:** **GO**
* **Lý do:** Problem và workflow đáp ứng xuất sắc mọi tiêu chuẩn gắt gao của Day 02 Lab. Dự án có tính khả thi cực kỳ cao và giải quyết được một "nỗi đau" có thật, sờ nắn được ngay tại chỗ.
* **Pilot nhỏ nhất cần làm (MVP):** Thiết lập một prompt chuẩn (System Prompt) chạy trên giao diện web đơn giản (Streamlit/Gradio). Copy nội dung một file Problem Card bất kỳ của học viên dán vào -> AI xuất ra kết quả chấm xem đủ field chưa và tự động nháp một đoạn feedback bằng tiếng Việt. Nhóm sẽ tự đo thời gian xem đoạn nháp đó có dùng được ngay hay phải sửa lại nhiều.

---
