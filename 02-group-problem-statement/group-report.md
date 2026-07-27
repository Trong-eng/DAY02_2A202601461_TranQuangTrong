# Group Report — Day 02

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1   | Nguyễn Quang Huy | 2A202601954 | Thành viên |
| 2   | Trần Quang Trọng | 2A202601461 | Thành viên |
| 3   | Tô Thái Dương    | 2A202601994 | Nhóm trưởng |
| 4   | Nguyễn Ngọc Thuận | 2A202601949 | Thành viên |

## Danh sách candidate problem của nhóm

| Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|
| Nguyễn Quang Huy | Tạo quiz ôn tập cuối kỳ từ slide, giáo trình và ghi chú môn học | Sinh viên đại học chuẩn bị thi cuối kỳ | Phải đọc lại tài liệu, chọn kiến thức trọng tâm, viết câu hỏi, đáp án nhiễu và kiểm tra đáp án; có thể mất khoảng 120 phút cho 20 câu | Phù hợp với AI, dễ làm prototype, đầu vào–đầu ra rõ và dễ đo thời gian tiết kiệm |
| Nguyễn Quang Huy | Trao đổi email để chốt lịch phỏng vấn | Recruiter, ứng viên và người phỏng vấn | Phải đọc khung giờ trong email, đổi múi giờ, kiểm tra nhiều calendar và trao đổi lại khi không có lịch trùng | Workflow lặp lại và dễ đo |
| Nguyễn Quang Huy | Tạo kịch bản tình huống nguy hiểm cho kiểm thử xe tự lái | Kỹ sư kiểm thử | Khó chuyển hazard requirement thành actor, hành vi, trigger, tham số và scenario hợp lệ với simulator; có thể mất khoảng 4 giờ cho một base scenario | Giá trị lớn và có tính khác biệt, nhưng cần giới hạn vào một ODD cụ thể và bắt buộc kỹ sư review |
| Trần Quang Trọng | Phải mở nhiều kênh (LMS, group chat, email) để gom deadline, file bài tập và format nộp. | Sinh viên | Thông tin bị phân tán ở nhiều nơi, khó chắc chắn đã gom đủ và không bỏ sót yêu cầu. | Workflow (AI trích xuất thông tin thành checklist/calendar -> SV xác nhận) |
| Trần Quang Trọng | Các câu hỏi về format, rubric, cách chạy code bị hỏi đi hỏi lại nhiều lần trong group lớp. | Sinh viên, TA, Giảng viên | Câu hỏi lặp lại nhưng câu trả lời không được hệ thống hóa, làm TA/Giảng viên tốn thời gian trả lời lại nhiều lần. | Workflow (AI tra cứu RAG gợi ý câu trả lời -> TA/GV duyệt gửi) |
| Trần Quang Trọng | Phải đọc từng đề thi cũ để tự đếm và thống kê xem chương nào hay ra để tập trung ôn tập. | Sinh viên | Phân loại và thống kê đề thi thủ công tốn thời gian, dễ bỏ sót pattern trọng tâm. | Workflow (AI phân loại ngữ nghĩa câu hỏi vào topic -> tự động xuất bảng tần suất) |
| Tô Thái Dương | Tự động phát hiện kẹt xe/nguy hiểm tại ngã tư bằng camera giao thông | Cảnh sát giao thông | Camera có sẵn nhưng chủ yếu để xem lại; phát hiện sự cố như tai nạn, xe dừng sai, ùn tắc vẫn phụ thuộc con người | Thực tế, có actor rõ, dễ demo bằng video giao thông và computer vision |
| Tô Thái Dương | Hỗ trợ nhân viên kho tìm và kiểm hàng nhanh hơn | Nhân viên kho, quản lý kho | Hàng nhiều mã, dễ nhầm vị trí, kiểm kê thủ công lâu, sai số tồn kho gây chậm giao hàng | Pain point rõ về thời gian và sai sót; có thể dùng AI nhận diện mã hàng, OCR, barcode, tối ưu vị trí lấy hàng |
| Tô Thái Dương | Detect code smell trong quá trình làm việc với mã nguồn theo team | Những người cần review code trong codebase lớn | Code do nhiều người tạo ra, vibecode có thể khó hiểu, vi phạm nhiều nguyên tắc lập trình, khó review hoặc phát hiện, khó scale và bàn giao | Phù hợp với AI, workflow đơn giản |
| Nguyễn Ngọc Thuận | Ghi chép & theo dõi công việc sau họp | Trưởng nhóm / PM tổng hợp biên bản | Sau mỗi cuộc họp nhóm, trưởng nhóm phải tổng hợp biên bản thủ công từ trí nhớ và ghi chú rời rạc | Workflow lặp lại, đầu vào–đầu ra rõ, dễ prototype và đo thời gian tiết kiệm. |
| Nguyễn Ngọc Thuận | Nhập liệu thủ công từ hóa đơn / PDF | ế toán nội bộ SME; nhân viên kho nhận hàng | Kế toán SME phải nhập tay từng dòng dữ liệu từ hóa đơn, ảnh chụp, PDF vào phần mềm kế toán | Điểm đau rõ về thời gian và sai sót, phù hợp AI OCR, nên bắt đầu với một loại chứng từ cụ thể. |
| Nguyễn Ngọc Thuận | Tìm kiếm tài liệu & kiến thức nội bộ | Nhân viên mới onboarding | Nhân viên mất nhiều thời gian tìm tài liệu nội bộ rải rác trên Drive, email, chat; không biết đâu là phiên bản mới nhất | Nhu cầu thường xuyên, phù hợp RAG; cần quản lý quyền truy cập, phiên bản tài liệu và trích dẫn nguồn. |

## Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Học tập và thông tin học vụ | Tạo quiz ôn tập cuối kỳ từ tài liệu<br>Gom deadline, file bài tập và format nộp từ nhiều kênh<br>Trả lời các câu hỏi lặp lại về format, rubric và cách chạy code<br>Phân loại đề thi cũ để thống kê chủ đề thường xuất hiện | Chuyển tài liệu học tập phân tán thành đầu ra có cấu trúc để sinh viên tìm, hiểu hoặc ôn tập nhanh hơn | Các candidate cùng phục vụ sinh viên nhưng khác đầu ra. Tạo quiz có phạm vi hẹp và metric thời gian rõ nhất để đưa vào shortlist. |
| B — Điều phối và tổng hợp knowledge work | Trao đổi email để chốt lịch phỏng vấn<br>Ghi chép và theo dõi công việc sau họp<br>Tìm kiếm tài liệu và kiến thức nội bộ | Đọc thông tin phi cấu trúc từ email, ghi chú hoặc kho tài liệu rồi biến thành lịch, biên bản, action item hoặc câu trả lời có thể hành động | Chốt lịch phỏng vấn có trigger, actor và before/after workflow rõ nhất. Tìm kiếm nội bộ có rủi ro về quyền truy cập và phạm vi dữ liệu. |
| C — Nhận diện và kiểm tra trong vận hành | Phát hiện kẹt xe/nguy hiểm tại ngã tư từ camera<br>Hỗ trợ nhân viên kho tìm và kiểm hàng<br>Nhập liệu thủ công từ hóa đơn/PDF | Nhận diện đối tượng hoặc trích xuất dữ liệu từ video, ảnh và chứng từ để giảm thời gian kiểm tra, nhập liệu và sai sót thủ công | Pain rõ nhưng cần dữ liệu hình ảnh/chứng từ đại diện, tích hợp thiết bị hoặc OCR; rủi ro vượt phạm vi lab trong ngày. |
| D — Đảm bảo chất lượng kỹ thuật | Tạo kịch bản tình huống nguy hiểm cho kiểm thử xe tự lái<br>Detect code smell trong quá trình làm việc với mã nguồn theo team | Phân tích artifact kỹ thuật theo rule và context, phát hiện hoặc tạo ra các trường hợp cần kỹ sư review trước khi sử dụng | Cả hai đều cần human review. Code smell dễ giới hạn vào một repo, một ngôn ngữ và một PR/diff nên phù hợp lab hơn scenario xe tự lái. |

## Shortlist


| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| Detect code smell trong quá trình làm việc với mã nguồn theo team | Nhóm hiểu workflow phát triển và review code; bottleneck nằm ở bước reviewer phải đọc diff cùng context để phát hiện vấn đề về maintainability. Có thể đo review time, số smell hợp lệ được phát hiện, false positive và lỗi bị bỏ sót. Rule / Workflow / Agent có ranh giới so sánh rất rõ. | Khái niệm code smell phụ thuộc ngôn ngữ và convention của team; linter đã xử lý được nhiều smell đơn giản. Cần giới hạn vào một ngôn ngữ, một repo và 3–5 loại smell, đồng thời bắt buộc reviewer duyệt kết quả. |
| Tạo quiz ôn tập cuối kỳ từ slide, giáo trình và ghi chú môn học | Actor, đầu vào và đầu ra rõ; có baseline giả định khoảng 120 phút cho 20 câu; prototype dễ làm với một bộ tài liệu nhỏ và có thể vẽ before/after workflow. | Chất lượng câu hỏi, đáp án nhiễu và độ bao phủ kiến thức khó chấm nhanh; số liệu thời gian mới là giả định và AI có thể tạo câu hỏi sai nhưng trông hợp lý. |
| Trao đổi email để chốt lịch phỏng vấn | Workflow lặp lại, bottleneck cụ thể ở trích xuất availability, đổi múi giờ và tìm slot giao nhau; impact đo được bằng active handling time, số vòng email và lỗi lịch. | Calendly, ATS hoặc form availability đã giải quyết nhiều trường hợp chuẩn; demo đầy đủ cần email/calendar integration và xử lý dữ liệu cá nhân. AI có thể không cần thiết nếu input đã có cấu trúc. |

## Score để đồng thuận


| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Detect code smell trong quá trình làm việc với mã nguồn theo team | 4 | 5 | 4 | 5 | 5 | 5 | 5 | **33** |
| Tạo quiz ôn tập cuối kỳ từ slide, giáo trình và ghi chú môn học | 5 | 5 | 3 | 4 | 5 | 4 | 5 | **31** |
| Trao đổi email để chốt lịch phỏng vấn | 5 | 5 | 3 | 4 | 4 | 5 | 4 | **30** |

Candidate nhóm chọn:

```text
Detect code smell trong quá trình làm việc với mã nguồn theo team
```

Vì sao chọn:

```text
- Nhóm hiểu domain phát triển và review code, đồng thời có thể dùng một repo hoặc PR/diff nhỏ để kiểm tra ngay trong lab.
- Bottleneck đủ cụ thể: reviewer phải đọc thay đổi cùng context để tìm các vấn đề về maintainability mà rule đơn giản có thể bỏ sót.
- Impact đo được bằng review time, số smell hợp lệ phát hiện được, false-positive rate và số finding được reviewer chấp nhận.
- Dễ so sánh ba hướng: Rule = linter/static rule; Workflow = CI chạy rule, tổng hợp và phân loại finding; Agent = đọc diff cùng context, giải thích và đề xuất refactor để reviewer duyệt.
- Có thể giữ scope vừa sức: một ngôn ngữ, một repo, một PR/diff và 3–5 loại code smell; không cho hệ thống tự sửa hoặc merge code.
```

Vì sao không chọn các candidate còn lại:

```text
- Tạo quiz: dễ prototype nhưng metric chất lượng khó thống nhất trong thời gian ngắn; câu hỏi hoặc đáp án sai có thể trông vẫn hợp lý, và baseline 120 phút chưa được validate.
- Chốt lịch phỏng vấn: workflow rõ nhưng non-AI alternative như Calendly, ATS và form availability đã mạnh; demo thật còn phụ thuộc email/calendar integration và quyền truy cập dữ liệu.
- Các candidate ngoài shortlist hoặc trùng pattern với ba bài trên, hoặc cần dữ liệu, thiết bị, quyền truy cập hay domain chuyên sâu hơn mức nhóm có thể kiểm chứng trong lab hôm nay.
```

Nếu có disagreement, nhóm xử lý thế nào:

```text
Nhóm dùng điểm để mở thảo luận chứ không chọn máy móc theo tổng. Mỗi ý kiến khác nhau phải chỉ ra tiêu chí đang chấm lệch và evidence còn thiếu. Nếu vẫn chưa thống nhất, nhóm thu hẹp từng candidate thành một thử nghiệm 30 phút, kiểm tra dữ liệu đầu vào có sẵn và khả năng đo output. Sau khi giới hạn bài code smell vào một repo, một ngôn ngữ và 3–5 smell, nhóm chấm lại và chọn candidate có tổng điểm cao nhất mà không có phản đối nghiêm trọng về actor, workflow hoặc phạm vi.
```

## Quick validation


| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview  | 3 | 2/3 developer nói phần tốn thời gian nhất khi review là mở các file liên quan, hiểu context và kiểm tra xem thay đổi có làm code khó bảo trì hơn không | 1/3 cho rằng linter và IDE đã bắt đủ lỗi thường gặp; AI review dễ tạo comment chung chung | Thu hẹp problem: không phải “AI review toàn bộ code”, mà là “draft finding cho một PR/diff nhỏ, tập trung vào các smell phụ thuộc context và luôn để reviewer duyệt” |
| Mini poll trong lớp | 6 | 4/6 từng gặp duplicate logic, long function hoặc class có quá nhiều trách nhiệm nhưng chỉ phát hiện muộn khi review hoặc sửa code | 2/6 ưu tiên checklist và static analysis vì kết quả ổn định, dễ giải thích hơn AI | Dùng rule/static analysis làm baseline; AI chỉ bổ sung finding có file/dòng, evidence và gợi ý refactor. Đo false positive thay vì đếm số comment thô |

Insight sau validation:

```text
Giả thuyết trọng tâm cần kiểm chứng: pain không nằm ở việc bắt mọi lỗi style mà rule đã xử lý tốt. Pain nằm ở đoạn reviewer phải nối diff với context, convention và trách nhiệm của module để phát hiện vấn đề maintainability, rồi viết comment đủ cụ thể để tác giả sửa được.
```

## Research giải pháp


> Để giữ scope cho lab, phần research và pilot dưới đây giả định team dùng **Python**. Nếu codebase thật dùng ngôn ngữ khác, thay Ruff bằng linter tương ứng nhưng giữ nguyên cấu trúc Rule → AI draft → Human review.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Ruff Linter | https://docs.astral.sh/ruff/linter/ | Chạy lint trên file hoặc thư mục Python theo bộ rule được cấu hình; một số lỗi có thể tự sửa | Chạy nhanh, deterministic, dễ dùng làm baseline và tích hợp vào bước kiểm tra trước review | Chỉ phát hiện những pattern đã được mã hóa thành rule; kết quả phụ thuộc bộ rule và cấu hình của team | Không dùng AI cho lỗi mà linter đã bắt ổn định. Chạy Ruff trước để loại noise và đo phần giá trị tăng thêm của AI |
| SonarQube Cloud PR Analysis | https://docs.sonarsource.com/sonarqube-cloud/improving/pull-request-analysis | Phân tích code change trong pull request, báo issue và áp quality gate trước merge | Có rule/profile, metric maintainability và tích hợp CI/PR rõ ràng | Cần cấu hình quality profile/gate; issue theo rule vẫn chưa thay thế judgment về design và context của reviewer | Workflow nên tái sử dụng static analysis và quality gate sẵn có thay vì xây lại hệ rule |
| Semgrep custom rules | https://docs.semgrep.dev/writing-rules/rule-ideas | Mã hóa các code pattern hoặc comment review lặp lại thành custom rule và tự động đưa vào PR/CI | Phù hợp convention riêng của team; rule có thể review, version và chạy lại nhất quán | Team phải viết và bảo trì rule; khó biểu diễn smell cần hiểu intent hoặc quan hệ giữa nhiều module | Comment nào lặp lại và diễn đạt được bằng pattern thì chuyển thành Rule; chỉ đưa phần còn lại sang AI |
| GitHub Copilot code review | https://docs.github.com/en/enterprise-cloud@latest/copilot/concepts/agents/code-review | Review pull request, dùng context repository, chỉ ra issue và đề xuất fix | Cho thấy AI có thể bổ sung review theo context và tạo suggestion ngay trên PR | GitHub nêu rõ Copilot không đảm bảo tìm được mọi lỗi, có thể mắc sai lầm và phải được human review | AI finding chỉ là draft/hypothesis. Không dùng AI review làm approval hoặc merge gate duy nhất |

Research takeaway:

```text
Không nên build một agent tự review, sửa và merge code. Hướng hợp lý hơn là Workflow nhiều lớp: rule/static analysis xử lý pattern xác định trước → AI đọc diff cùng context giới hạn để draft finding → developer kiểm chứng, edit và quyết định comment nào được gửi.
```

## Workflow before/after

File nhóm nộp kèm:

```text
02-group-problem-statement-workflow.png
```

Nội dung workflow:

```text
CURRENT STATE — 6 bước, khoảng 45 phút/PR cỡ 100–300 LOC

[1 Đọc mô tả PR/ticket: 5']
→ [2 Scan toàn bộ diff: 8']
→ [3 Mở các file liên quan để hiểu context: 12']  <-- bottleneck
→ [4 Đối chiếu convention và tìm code smell: 10']  <-- bottleneck
→ [5 Viết comment + gợi ý refactor: 7']
→ [6 Đọc lại và submit review: 3']

FUTURE STATE — 5 bước, khoảng 21 phút active time

[1 Ruff/Semgrep scan changed files: 1']                 -- Rule/script
→ [2 Workflow gom diff + tối đa 3 file context: 2']      -- Workflow step
→ [3 AI draft finding có vị trí/evidence/gợi ý: 2']      -- AI step
→ [4 Reviewer kiểm chứng + tìm phần AI bỏ sót: 14']       -- Human boundary
→ [5 Reviewer edit và submit comment hợp lệ: 2']

Fallback:
AI finding chung chung, sai context hoặc không chỉ ra evidence
→ bỏ toàn bộ AI draft và review thủ công; kết quả Ruff/Semgrep vẫn được giữ.

Bottleneck mới:
Reviewer kiểm chứng finding và kiểm tra phần AI bỏ sót. Đây là bottleneck chấp nhận được vì đó là điểm kiểm soát chất lượng và trách nhiệm cuối cùng.
```

> Các mốc thời gian là giả định ban đầu để thiết kế pilot; nhóm phải đo baseline trên PR thật hoặc PR đã ẩn dữ liệu nhạy cảm.

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Active review time cho PR 100–300 LOC | Khoảng 45 phút | Dưới 25 phút | Target chính; cần đo median trên cùng bộ PR |
| Số bước | 6 | 5 | Giá trị chính đến từ giảm effort tìm context và viết comment, không chỉ giảm số bước |
| Bước hoàn toàn thủ công | 6/6 | 2/5 | Reviewer vẫn kiểm chứng/edit và submit review |
| Tỷ lệ AI finding được reviewer chấp nhận | Chưa có baseline | Tối thiểu 80% | Finding hợp lệ phải có vị trí, evidence và action đề xuất |
| Code smell bị bỏ sót trên bộ mẫu đã gắn nhãn | Chưa đo | Không kém reviewer-only baseline | Không đánh đổi chất lượng để lấy tốc độ |
| Bottleneck chính | Tìm context + xác định smell | Kiểm chứng/edit finding | Human boundary |
| Risk chính | Review không nhất quán, bỏ sót smell | AI false positive, bỏ sót hoặc suy diễn sai context | Không tự comment, sửa hoặc merge code |

## Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Developer hoặc tech lead phụ trách review pull request trong team 3–8 người làm việc trên một codebase Python. |
| **Workflow** | Với mỗi PR cỡ 100–300 LOC, reviewer đọc ticket và diff, mở các file liên quan, đối chiếu convention, tìm code smell, viết comment, kiểm tra lại rồi submit review. |
| **Bottleneck** | Bước mở context và xác định smell mất khoảng 22 phút vì reviewer phải hiểu trách nhiệm của module, so sánh với convention và phân biệt vấn đề maintainability thật với lỗi style mà linter đã bắt. |
| **Impact** | Theo giả định ban đầu, một PR mất khoảng 45 phút active review. Với 5 PR/tuần, một reviewer tốn khoảng 225 phút; review vội hoặc không nhất quán có thể để duplicate logic, long function hoặc class quá nhiều trách nhiệm đi vào main branch. |
| **Success Metric** | Giảm median active review time xuống dưới 25 phút/PR; tối thiểu 80% AI finding được reviewer xác nhận hợp lệ; tỷ lệ smell phát hiện trên bộ mẫu không thấp hơn reviewer-only baseline. |
| **Boundary** | Chỉ đọc diff và context được cấp; không tự comment lên PR, không tự sửa/commit/merge code; không thay thế linter, test, security scan hoặc approval của reviewer. |

## Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Ruff/Semgrep/SonarQube chạy rule, complexity threshold và quality gate trên changed files | Đủ với lỗi có pattern ổn định, convention lặp lại và threshold đo được | Bỏ sót design smell cần context; rule quá nhiều tạo noise và false positive | Không chọn làm toàn bộ, nhưng bắt buộc dùng làm baseline và bước đầu tiên |
| **Workflow** | Static scan → gom diff/context giới hạn → AI draft finding → reviewer kiểm chứng/edit → submit | Phù hợp vì thứ tự bước rõ, AI chỉ hỗ trợ phần đọc-ngôn ngữ cần context và human boundary cố định | Draft có thể sai hoặc chung chung; context đưa vào có thể thiếu hoặc chứa dữ liệu nhạy cảm | **Chọn** |
| **Agent** | Agent tự điều hướng repo, chọn file/tool, chạy test, đề xuất hoặc thực hiện refactor và comment lên PR | Chỉ cần khi bài toán có nhiều nhánh, phải tự quyết bước phân tích tiếp theo và được cấp nhiều tool | Permission rộng, khó dự đoán, có thể sửa sai hoặc lộ source; quá rộng cho pilot | Chưa chọn |

Mức chọn:

```text
Workflow.
```

Vì sao:

- Lỗi xác định trước nên để rule/static analysis xử lý nhanh và nhất quán.
- Code smell phụ thuộc context cần AI hỗ trợ đọc diff, đối chiếu convention và draft lời giải thích.
- Reviewer vẫn kiểm chứng từng finding nên false positive không đi thẳng vào PR.
- Chưa cần agent vì workflow tuyến tính, input được giới hạn và không cần AI tự lập kế hoạch hoặc tự thay đổi code.

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Developer hoặc tech lead review PR trong team 3–8 người dùng Python. |
| **Workflow** | Đọc ticket → scan diff 100–300 LOC → mở file liên quan để hiểu context → đối chiếu convention → tìm code smell → viết và submit comment. Khi dùng AI, context được giới hạn ở tối đa 3 file. |
| **Bottleneck** | Reviewer mất khoảng 22 phút để gom context và phát hiện các maintainability smell mà rule đơn giản bỏ sót. |
| **Impact** | Giả định khoảng 45 phút/PR và 225 phút/tuần với 5 PR; smell bị bỏ sót làm code khó hiểu, khó mở rộng và khó bàn giao. |
| **Success Metric** | Median review time dưới 25 phút; ≥80% AI finding được reviewer chấp nhận; detection trên bộ mẫu không thấp hơn reviewer-only baseline. |
| **Boundary** | AI không tự comment, sửa, commit hoặc merge; chỉ đọc diff/context được cấp; không thay test, security scan, static analysis hay human approval. |
| **AI intervention point** | Sau khi Ruff/Semgrep đã quét changed files và workflow đã gom diff cùng context giới hạn, trước bước reviewer tự tìm smell và viết comment. |
| **Mức chọn** | Workflow: rule/static scan → AI draft finding → reviewer kiểm chứng/edit → submit. |
| **Rủi ro & người thật kiểm tra** | Risk: false positive, bỏ sót smell, suy diễn sai intent, comment quá chung và rò rỉ source. Người thật kiểm tra: reviewer xác minh file/dòng, evidence và tính phù hợp của refactor trước khi gửi. |

## Final decision

Decision:

```text
Go với scope nhỏ.
```

Pilot nhỏ nhất:

- Chọn 6 PR/diff Python đã đóng hoặc đã ẩn dữ liệu nhạy cảm, mỗi PR khoảng 100–300 LOC.
- Giới hạn 3–5 smell: duplicate logic, long function, too many responsibilities, deep nesting và inappropriate coupling.
- Một reviewer gắn nhãn finding hợp lệ cho bộ mẫu và đo thời gian review thủ công để tạo baseline.
- Chạy Ruff/Semgrep trước, sau đó đưa diff cùng tối đa 3 file context và convention của team cho AI draft finding.
- Reviewer chấm từng finding theo: hợp lệ/không hợp lệ, có evidence/không, dùng được/cần viết lại; đồng thời ghi active review time.
- So sánh Rule-only, Workflow có AI và reviewer-only bằng time, accepted-finding rate và số smell bị bỏ sót.

Exit / rollback:

- Nếu dưới 70% AI finding được reviewer chấp nhận trong 2 vòng thử liên tiếp, bỏ bước AI và giữ linter + checklist review.
- Nếu Workflow bỏ sót nhiều smell hơn reviewer-only baseline hoặc làm review lâu hơn, không tích hợp vào PR process.
- Nếu AI cần source/context vượt boundary đã định hoặc làm lộ secret/dữ liệu nội bộ, dừng pilot và chỉ dùng công cụ chạy local đã được phê duyệt.
- Nếu reviewer phải viết lại hơn 50% nội dung của đa số finding, chuyển AI output thành checklist riêng, không tạo draft comment.

Decision rationale:

- Problem có actor, workflow, bottleneck và metric kiểm chứng được.
- Rule-based alternatives đã có sẵn và được dùng làm baseline thay vì build lại.
- AI chỉ can thiệp ở bước cần hiểu context và draft giải thích, không ôm toàn bộ code review.
- Human review và rollback condition rõ ràng.

---
