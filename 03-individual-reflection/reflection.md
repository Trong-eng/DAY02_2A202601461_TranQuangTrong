# 03 — Individual Reflection — Trần Quang Trọng

## Đóng góp của Trần Quang Trọng trong nhóm

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Từ quá trình scan, tôi đưa vào nhóm 3 problems trong bối cảnh học tập: gom deadline/file/format nộp từ nhiều kênh, xử lý các câu hỏi lặp lại về rubric và cách chạy code, phân loại đề thi cũ để tìm topic thường xuất hiện. | Nhóm có thêm ba candidate gần với trải nghiệm sinh viên, có actor và pain cụ thể thay vì chỉ tập trung vào bài toán doanh nghiệp. |
| Pitch Problem Card | Tôi trình bày người gặp vấn đề, thông tin đang nằm ở đâu, bước thủ công gây tốn thời gian và cách đo cho từng candidate. | Nhóm hiểu ba bài có chung pattern “biến thông tin học tập phân tán thành đầu ra có cấu trúc”, nhưng đầu ra lần lượt là checklist, câu trả lời và bảng tần suất. |
| Challenge bài của bạn khác | Tôi hỏi candidate code smell rằng linter đã giải quyết phần nào, “finding tốt” được đánh giá bằng số comment hay tỷ lệ reviewer chấp nhận, và nhóm có evidence nào cho thời gian review hay chưa. | Nhóm không đo thành công bằng số comment AI tạo ra; metric được chuyển sang accepted-finding rate, review time và số smell bị bỏ sót, đồng thời giữ reviewer làm người quyết định. |
| Gom trùng / cluster | Tôi tham gia gom các candidate về học tập vào cluster A và chỉ ra điểm giống/khác giữa quiz, deadline, FAQ và phân tích đề thi. | Nhóm giảm tranh luận trùng lặp và nhận ra các candidate cùng domain vẫn phải tách theo trigger, workflow và output. |
| Chọn candidate problem | Tôi tham gia so sánh shortlist theo actor, workflow, evidence, impact, khả năng làm trong lab và mức hiểu domain. Các candidate của tôi không vào top 3 vì chưa có baseline và dễ bị giải quyết một phần bằng checklist/search/rule. | Tôi đồng ý chọn code smell sau khi bài này đạt 33/35 và được thu hẹp vào một repo, một ngôn ngữ, một PR/diff nhỏ và 3–5 loại smell. |
| Validation / research | Tôi góp ý rằng Quick interview và mini poll phải được xem là giả thuyết cho đến khi nhóm hỏi người thật; đồng thời tham gia đối chiếu các hướng Ruff, SonarQube, Semgrep và AI code review. | Nhóm tách được hai loại evidence: interview để xác nhận pain và tài liệu tool để hiểu solution landscape; không dùng sự tồn tại của tool thay cho bằng chứng pain. |
| Workflow nhóm | Tôi rà soát current/future workflow, đặc biệt là bước linter, AI draft, reviewer kiểm chứng và fallback khi AI sai context. | Workflow cuối không cho AI tự comment hoặc merge; static scan vẫn hoạt động kể cả khi AI draft bị loại. |
| Problem Statement | Tôi góp phần làm rõ actor, loại PR, phạm vi context và metric chất lượng; phản biện câu “AI phát hiện code smell tốt hơn” vì chưa có baseline. | Problem Statement v1 có actor developer/tech lead, PR Python 100–300 LOC, intervention point, accepted-finding rate, detection baseline và boundary rõ. |
| Rule / Workflow / Agent | Tôi ủng hộ dùng rule cho pattern xác định trước và chỉ dùng AI ở bước cần đọc context, sau đó reviewer kiểm chứng. | Nhóm chọn **Workflow** thay vì Agent; giải pháp có đường đi cố định và quyền tự quyết vẫn thuộc con người. |
| Decision | Tôi tham gia thống nhất pilot 6 PR/diff, so sánh reviewer-only, Rule-only và Workflow có AI; đồng thời đặt rollback nếu AI làm review chậm hơn hoặc finding không được chấp nhận. | Nhóm chốt “Go với scope nhỏ” thay vì cam kết xây một hệ thống review tự động hoàn chỉnh. |

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý cách diễn đạt các pain học tập thành actor, trigger, workflow sơ bộ và cách đo. | Giúp tôi nhìn thấy các vấn đề lặp lại giữa LMS, group chat, email, FAQ và đề thi cũ. | AI thường nhảy ngay sang “RAG”, “tự động tạo calendar” hoặc “phân loại bằng AI” trước khi chứng minh pain. | Tôi viết lại candidate theo việc sinh viên/TA đang phải làm thủ công, còn AI chỉ để ở phần cảm nhận nhanh. |
| Problem Card | Cấu trúc nội dung pitch thành problem, actor, bottleneck, impact và future workflow. | Giúp ba candidate dễ so sánh dù có output khác nhau. | AI có thể tự giả định số phút, số câu hỏi hoặc tần suất xảy ra mà tôi chưa đo. | Tôi không dùng số liệu không có nguồn; những metric chưa đo chỉ được xem là câu hỏi cần validation. |
| Workflow | Gợi ý thứ tự Rule → AI draft → Reviewer và cách thể hiện fallback. | Giúp kiểm tra future state có trigger, input, output và human boundary hay chưa. | AI ban đầu dễ đề xuất tự comment, tự sửa code hoặc đọc toàn bộ repo, làm scope thành Agent quá sớm. | Tôi giữ flow tuyến tính, giới hạn context và yêu cầu reviewer kiểm chứng từng finding trước khi gửi. |
| Research | Tìm tool tương tự và tóm tắt khác biệt giữa linter, static analysis, custom rule và AI review. | Giúp nhóm không xây lại chức năng Ruff/SonarQube/Semgrep đã có và thấy khoảng trống của review theo context. | AI có thể đưa claim về độ chính xác hoặc tiết kiệm thời gian mà không có nguồn chính thức. | Tôi chỉ chấp nhận thông tin có link tài liệu chính thức và không dùng marketing claim làm success metric. |
| Problem Statement | Nhờ AI chỉ ra field còn rộng, mơ hồ hoặc chưa đo được. | AI giúp phát hiện actor “người review codebase lớn” và metric “phát hiện nhiều smell hơn” chưa đủ cụ thể. | AI có xu hướng gộp maintainability, bug, security và refactor thành một problem. | Tôi giữ scope ở maintainability smell trên changed code, một loại PR và một human reviewer chịu trách nhiệm cuối. |
| Rule / Workflow / Agent | Dùng AI lập bảng so sánh ba mức và liệt kê rủi ro. | Hữu ích khi phân tách phần deterministic, phần cần context và mức quyền tự chủ. | AI dễ gọi mọi hệ thống có nhiều bước là Agent, dù các bước đã được con người định sẵn. | Tôi dùng tiêu chí “ai quyết định bước tiếp theo và ai có quyền hành động”; case này là Workflow, chưa phải Agent. |
| Decision | Nhờ AI gợi ý pilot, metric và exit/rollback condition. | Giúp quyết định có cách kiểm chứng và phương án hạ xuống linter + checklist. | Các ngưỡng 70%, 80% và 50% vẫn là target thiết kế, không phải evidence lịch sử. | Tôi coi chúng là tiêu chí thử nghiệm cần điều chỉnh sau vòng pilot và luôn so sánh với reviewer-only baseline. |

## Bài học của Trần Quang Trọng

- **Tôi học được gì khi nghe top 3 của các bạn khác?** Tôi học được rằng sự quen thuộc với pain chưa đủ để một candidate được chọn. Ba bài của tôi gần trải nghiệm sinh viên nhưng vẫn thiếu baseline và có non-AI alternative mạnh. Code smell đến từ domain khác nhưng có actor, workflow review và cách so sánh Rule / Workflow / Agent rõ hơn sau khi được thu hẹp.
- **Nhóm có lúc nào bị solution-first không?** Có, kể cả trong candidate của tôi. Tôi đã mô tả quá sớm các hướng “AI trích xuất checklist”, “RAG trả lời FAQ” và “AI phân loại đề thi” trước khi chứng minh sinh viên hoặc TA đau nhất ở bước nào. Với code smell, nhóm cũng từng nghiêng về agent đọc cả repo. Việc quay lại current workflow giúp nhóm thấy rule đã đủ cho một phần lớn vấn đề.
- **Tôi có thay đổi ý kiến sau khi bị challenge không?** Có. Ban đầu tôi nghĩ gom deadline hoặc FAQ lớp dễ làm và gần người dùng hơn. Sau challenge, tôi thấy chúng cần kiểm tra data access, nguồn nào là source of truth và liệu template/search có đủ hay không. Tôi chuyển sang ủng hộ code smell, nhưng chỉ ở mức Workflow có rule baseline và reviewer duyệt.
- **Tôi đóng góp gì thật sự vào artifact cuối?** Tôi đưa ba candidate về học tập, giúp hình thành cluster A, tham gia challenge metric/evidence của code smell, kiểm tra Quick validation, góp ý workflow fallback, success metric và cách phân biệt Rule / Workflow / Agent.
- **Điều khó nhất khi viết Problem Statement là gì?** Khó nhất là định nghĩa “code smell hợp lệ” và đo chất lượng mà không dùng số comment thô. Một AI có thể tạo nhiều comment nhưng vẫn làm reviewer tốn thời gian. Vì vậy nhóm phải đo tỷ lệ finding được chấp nhận và số smell bị bỏ sót song song với review time.
- **Bài học lớn nhất về AI:** AI hỗ trợ tốt việc cấu trúc và tạo phương án, nhưng dễ biến tên solution thành problem và biến target thành evidence. Tôi phải luôn quay lại actor, workflow hiện tại, non-AI baseline và người chịu trách nhiệm cuối.

Nếu làm lại:

```text
Tôi sẽ phỏng vấn sinh viên và TA trước khi pitch ba candidate của mình, đo xem pain nằm ở gom thông tin, xác minh source hay trả lời lặp lại. Với bài nhóm, tôi sẽ yêu cầu reviewer đo baseline trên vài PR và chạy linter trước khi thảo luận AI. Tôi cũng sẽ challenge solution-first ngay từ tên candidate: mô tả việc người dùng đang gặp trước, chỉ bàn RAG, Workflow hoặc Agent sau khi problem đã đủ rõ.
```

## Kiểm tra hiểu bài cá nhân

Mạch tôi hiểu là: bắt đầu từ problem thật của actor, vẽ workflow hiện tại để thấy bottleneck, đặt metric để biết có đáng giải quyết không, xác định boundary để AI không vượt quyền, rồi mới chọn No AI / Rule / Workflow / Agent.

Với bài nhóm, problem không phải là “dùng AI review code”, mà là reviewer mất thời gian gom context và phát hiện maintainability smell trên PR nhỏ. Rule phù hợp với lỗi có pattern rõ như lint hoặc static analysis. Workflow phù hợp hơn Agent vì các bước đã cố định: static scan → gom diff/context → AI draft finding → reviewer kiểm chứng. Agent chưa cần vì AI không được tự chọn hành động, tự sửa code, tự comment hoặc merge.

---
