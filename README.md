# Track1_Day17_2A202602746_LuuXuanDung

## 1. Thông tin cá nhân và nhóm
- Mã học viên: 2A202602746
- Họ tên: Lưu Xuân Dũng
- GitHub: luuxuandung04
- Tên nhóm: **3aecaykhe**
- Thành viên: Lưu Xuân Dũng, Nguyễn Văn An, Nguyễn Long Khánh
- Case đã chọn: **Case B — AI Notes: Personal Learning Notes**
- Ngày phỏng vấn: **04/10/2026**.
- Interviewer: **Lưu Xuân Dũng**.
- Người được phỏng vấn: **Minh Tâm**, thuộc nhóm khác (mã notes: P01).
- Tài liệu nhóm: https://docs.google.com/document/d/1ev_OXpRAOvKnDNNxycYnTFmN8uaQBxgVhxsKWAcU1vg/edit

**Trạng thái:** đã tích hợp bài nhóm và notes từ transcript; đã đủ thông tin cá nhân và nhóm; đã xác nhận ngày phỏng vấn, interviewer và người ngoài nhóm; recruitment check đã được người học xác nhận. Reflection đã được biên tập từ transcript với AI hỗ trợ; còn bước tự nghe lại và xác minh consent. Bản ghi nộp dưới dạng file. Đây là buổi luyện tập, không phải validation. Những chỉnh sửa do Codex đề xuất sau khi đọc tài liệu không được ghi là quyết định nhóm đã thực hiện trong giờ lab.

## 2. Problem Hypothesis Brief

### 2.1 Solution — capability trung tính
**Directive nguyên văn từ đề lab:** Trong khi học, học viên có thể highlight một đoạn nội dung, đánh dấu “Chưa hiểu”, hoặc viết một câu hỏi hay ghi chú ngắn. Khi bài học kết thúc, AI Notes kết hợp những dấu vết này với nội dung bài để tạo một bản ghi chú có cấu trúc. Học viên có thể chỉnh sửa và xác nhận trước khi lưu.

**Capability trung tính:** Giúp người học chọn lọc, tổ chức và lưu lại nội dung gắn với những điểm họ quan tâm hoặc chưa hiểu trong bài học, để có thể xem lại khi ôn tập.

Chỉnh bản nháp: mô tả “tự động tóm tắt tài liệu” chưa bao quát input cá nhân và bước người học kiểm tra/xác nhận của directive. Capability không mặc định AI là cách duy nhất.

### 2.2 Change — chuỗi thay đổi kỳ vọng
Solution → bản ghi chú được tổ chức từ dấu vết cá nhân và bài học (**output**) → học viên kiểm tra, chỉnh sửa và lưu → học viên thực sự mở lại và tìm được ý cần ôn → giảm công sức tìm lại thông tin, hỗ trợ ôn tập (**outcome giả định**).

1. Người học lưu được những ý và câu hỏi có ý nghĩa với mình.
2. Người học xác nhận nội dung thay vì tin hoàn toàn vào bản tổng hợp.
3. Người học sử dụng lại ghi chú khi cần ôn tập.

Tiết kiệm thời gian, tăng ghi nhớ, điểm số hoặc tỷ lệ hoàn thành là kỳ vọng cần kiểm chứng; một bản ghi chú được tạo ra chưa chứng minh các outcome này. Nếu learner không lưu hoặc không xem lại, chuỗi giá trị có thể không xảy ra.

### 2.3 Actor
| Actor | Họ đang làm gì? | Pain/hậu quả có thể có (giả thuyết) | Lợi ích kỳ vọng |
| --- | --- | --- | --- |
| Learner | Học, lưu nội dung và ôn tập | Khó chọn ý cần lưu; khó tìm lại hoặc hiểu ghi chú | Tìm được thông tin cần ôn và sử dụng lại |
| Instructor | Giảng dạy và giải thích kiến thức | Có thể phải giải thích lại hoặc xử lý hiểu sai | Learner chuẩn bị câu hỏi rõ hơn; chưa có instructor-side evidence |
| Course Admin / Platform Owner | Quản lý khóa học | Có thể có chi phí hỗ trợ hoặc học viên bỏ dở | Cải thiện trải nghiệm; chưa có evidence về retention/completion |

**Actor chọn điều tra trước:** Learner, vì họ trực tiếp quyết định lưu gì và có sử dụng lại hay không. Không giả định giảng viên có thể xem ghi chú cá nhân: directive không mô tả chức năng này.

### 2.4 Situation & Job
**Hypothesis từ bài nhóm, được diễn đạt lại:** Khi học một bài có nhiều nội dung mới, learner đang cố giữ lại những ý quan trọng để ôn tập, có thể bằng ghi chép, highlight hoặc lưu nội dung. Họ có thể gặp khó ở việc chọn ý và lưu lại trong lúc vẫn theo dõi bài.

Notion/Word, chép tay và screenshot là các cách làm **có thể có trong giả thuyết nhóm**, không phải hành vi đã xác nhận của P01.

**JTBD Hypothesis:** Khi học một bài có nhiều nội dung mới, tôi muốn giữ lại những ý cần nhớ và những điểm chưa hiểu theo cách dễ tìm lại, để có thể ôn tập và tiếp tục giải quyết phần mình còn vướng.

### 2.5 Hai giả thuyết pain cạnh tranh
**A — khó tạo ghi chú trong lúc học:** Khi theo dõi bài giảng có nhiều nội dung mới, learner khó vừa theo dõi vừa lưu các ý quan trọng vì chưa kịp chọn lọc và ghi lại trước khi bài chuyển tiếp, dẫn đến bỏ sót ý hoặc phải xem lại để bổ sung.

**B — khó sử dụng lại ghi chú:** Khi ôn tập một bài đã học, learner khó tìm và hiểu lại thông tin mình đã lưu vì nội dung thiếu cấu trúc hoặc thiếu ngữ cảnh, dẫn đến phải quay lại học liệu gốc để tìm lại.

**Lựa chọn trong bài nhóm:** điều tra A trước, vì khó khăn có thể bắt đầu ngay tại thời điểm học. Cần giữ B như cách giải thích cạnh tranh và kiểm tra liệu rào cản chính thực ra là hiểu thuật ngữ/kiến thức nền thay vì ghi chú.

### 2.6 Evidence Map — định nghĩa bằng chứng cần tìm
| Cần kiểm tra | Evidence làm tin hơn | Evidence khiến sửa/bác bỏ |
| --- | --- | --- |
| Situation có thật | Một sự kiện trong 7 ngày gần đây, mô tả được bài học và nội dung đã ghi/highlight/lưu | Không có sự kiện phù hợp; chưa thể dùng người này để kiểm tra pain ghi chú |
| Pain có ý nghĩa | Một lần bỏ sót ý, không theo được bài do ghi chép hoặc không tìm được nội dung cần ôn | Cách hiện tại đáp ứng tốt; khó khăn chủ yếu là hiểu thuật ngữ, không liên quan ghi chú |
| Workaround tồn tại | Dừng/xem lại bài, chép lại, lưu ảnh hoặc tổ chức lại ghi chú trong sự kiện cụ thể | Không cần làm thêm, hoặc tài liệu sẵn có đã giải quyết job |
| Consequence tồn tại | Tốn thêm thời gian, bỏ sót nội dung hoặc không hoàn thành việc cần làm; user kể chi tiết | Không có ảnh hưởng đáng kể; user vẫn hoàn thành job dễ dàng |
| Pattern có lặp | Người này kể thêm một sự kiện trước đó với hành vi/hậu quả tương tự | Chỉ xảy ra một lần hoặc do một tình huống đặc biệt |

Không lấy “điểm thấp/bỏ khóa” làm fact khi chưa hỏi; không quy người dùng không gặp pain thành người “quản lý thời gian kém”. Pattern trong một người không chứng minh vấn đề phổ biến ở đa số learners.

### 2.7 Chốt Problem Hypothesis và đối chiếu lượt luyện
**Problem Hypothesis mang sang Chặng 2:** Khi theo dõi bài giảng có nhiều nội dung mới, learner có thể khó chọn lọc và lưu lại các ý quan trọng trong lúc vẫn theo bài, dẫn đến bỏ sót ý hoặc phải xem lại học liệu để tạo nội dung phục vụ ôn tập.

**Điều phải đúng:** learner có nhu cầu lưu và sử dụng lại nội dung; khó khăn xảy ra ở khâu chọn/lưu thông tin; cách hiện tại gây hậu quả đáng kể.

**Điều có thể làm giả thuyết sai:** tài liệu sẵn có đã đủ; learner ghi và ôn lại thuận lợi; vấn đề chính là không hiểu thuật ngữ/khái niệm chứ không phải ghi chú; hoặc pain nằm ở tìm lại thông tin sau khi học (B).

**Sau lượt luyện P01:** transcript cho thấy người tham gia tự nhận thiếu nền tảng AI, khó hiểu slide, không theo kịp và hỏi AI về từ khóa. Chưa có câu chuyện đủ rõ về việc ghi chú thực tế. Vì vậy **A và B chưa được xác nhận bởi lượt này**. Tín hiệu về hiểu nội dung là một nhánh cần điều tra thêm, không phải lý do tự động đổi case hoặc tuyên bố validated. Xem `interview/notes.md` để phân biệt evidence với diễn giải.

### 2.8 Solution Parking Lot
| Hướng giải quyết để park, chưa lựa chọn triển khai | AI / Không AI |
| --- | --- |
| 1. Tổng hợp ghi chú từ highlight, câu hỏi và nội dung bài, có bước kiểm tra | AI |
| 2. Gợi ý câu hỏi ôn tập từ ghi chú người học đã xác nhận | AI |
| 3. Khung ghi chú Cornell/Outline cạnh bài giảng | Không AI |
| 4. Bookmark theo mốc video và highlight slide để tìm lại | Không AI |
| 5. Chia sẻ ghi chú trong nhóm học với sự chủ động của người tạo | Không AI |

## 3. Conversation Guide đã chỉnh sửa — đề xuất cho vòng tiếp theo
**Nguồn:** được bổ sung sau khi Codex rà soát transcript; người học/nhóm cần đọc và xác nhận sử dụng. Chưa có bằng chứng nhóm đã dùng guide này trong giờ lab.

### Recruitment và mở đầu
- Tiêu chí: người ngoài nhóm đã ghi chú, highlight hoặc lưu nội dung để xem sau trong **7 ngày gần đây**.
- Recruitment check: “Trong 7 ngày vừa rồi, bạn có lần nào ghi chú, highlight hoặc lưu nội dung học để xem lại không? Đó là bài nào, vào ngày nào?” Câu này chỉ tuyển người, không thay thế evidence chính.
- Nếu không phù hợp: đổi người phỏng vấn; không ép câu chuyện khó hiểu bài thành evidence về ghi chú.
- Mở đầu: “Mình muốn hiểu cách bạn học và giữ lại nội dung để xem sau. Không có đáp án đúng hay sai. Mình xin phép ghi âm để nghe lại và làm bài học; chỉ chia sẻ với giảng viên/TA. Bạn có đồng ý không?” Chỉ bắt đầu ghi sau khi có đồng ý rõ ràng.
- Story opener: “Kể mình nghe lần gần nhất trong tuần vừa rồi bạn ghi chú, highlight hoặc lưu một phần bài học để xem sau. Lúc đó bạn đang học bài nào?”

### Big 3
| Điều cần học | Evidence cần tìm | Câu hỏi chính | Điều làm xem lại giả thuyết |
| --- | --- | --- | --- |
| 1. Quá trình chọn và lưu ý thực tế | Trình tự hành động, nội dung lưu và cách lưu | “Ở lần đó, bạn đã chọn và lưu những gì? Kể từ lúc bắt đầu đến lúc xong nhé.” | Lưu dễ dàng, không ảnh hưởng việc theo bài |
| 2. Chỗ vướng, workaround và hậu quả | Một khoảnh khắc cụ thể, hành động xử lý, công sức/hậu quả | “Ở lần đó có chỗ nào không diễn ra như bạn muốn không? Sau đó bạn làm gì?” | Không có khó khăn hoặc vấn đề chủ yếu là chưa hiểu kiến thức |
| 3. Ghi chú có thực sự cần và được dùng lại? (câu hỏi có thể làm giả thuyết yếu đi) | Lần mở lại, mục đích, kết quả; tài liệu thay thế | “Sau lần đó, bạn đã mở lại phần đã lưu chưa? Kể lần gần nhất bạn ôn nội dung ấy và đã dùng tài liệu nào.” | Không cần dùng lại; slide/tài liệu có sẵn đã đủ để hoàn thành job |

### Probe bank
- “Lúc đó chuyện gì xảy ra tiếp theo?” / “Bạn đã làm gì?”
- “Bạn chọn cách đó vì sao?” / “Bạn đã thử cách nào khác ở lần đó?”
- “Phần đã lưu lúc đó gồm những gì? Nếu tiện, bạn có thể mô tả hoặc cho xem phần liên quan không?”
- “Việc đó mất khoảng bao lâu?” / “Nó ảnh hưởng thế nào tới việc bạn định làm?”
- “Lần gần nhất trước đó xảy ra là khi nào?”
- Nếu gặp thuật ngữ khó: “Thuật ngữ nào ở bài đó? Bạn đã hỏi gì, rồi dùng câu trả lời thế nào?” Không tự giới thiệu tên hoặc lợi ích của công cụ.

### Khi câu trả lời lệch khỏi evidence
- Lời khen: cảm ơn ngắn rồi quay về hành động đã xảy ra.
- Câu chung chung/tương lai: “Lần gần nhất chuyện đó xảy ra là khi nào?”
- Feature request: “Điều đó giúp bạn làm việc gì? Ở lần vừa kể, bạn đã xử lý ra sao?”

### Sửa câu hỏi dựa trên transcript
| Câu hỏi/cách hỏi trong lượt luyện | Cách sửa đề xuất | Lý do |
| --- | --- | --- |
| “slide quá nhiều… video quá dài… quá ba mươi phút” | Story opener về lần đã ghi/highlight/lưu trong 7 ngày | Bỏ giả định khối lượng lớn là pain và ngưỡng 30 phút do interviewer đặt |
| “giảng viên… chuyển qua slide khác mà bạn chưa kịp hiểu” | “Ở lần đó có chỗ nào không diễn ra như bạn muốn? Lúc ấy bạn làm gì?” | Không gợi sẵn khó khăn để user đồng ý |
| “bạn sẽ làm cách nào… ghi chú lại” | “Ở lần đó bạn đã lưu nội dung gì, bằng cách nào?” | Đổi từ cách làm chung/tương lai sang hành vi quá khứ |
| Giải thích AI ngoài không có nội dung slide, AI Tutor có kiến thức slide | Hỏi công cụ user tự nêu, prompt thực tế và kết quả họ sử dụng | Tránh giải thích solution và làm nhiễu evidence |
| “ngày hôm sau… quên mất” | “Kể lần gần nhất bạn ôn lại nội dung đó; bạn tìm và nhớ lại bằng cách nào?” | Không mặc định người dùng đã quên |

## 4. Practice Reflection
**Cách thực hiện:** phần này được biên tập với hỗ trợ Codex từ transcript cuộc phỏng vấn thực tế. Chưa đối chiếu trực tiếp audio; không coi đây là xác nhận người học đã hoàn thành bước tự nghe lại theo yêu cầu lab.

### 1. Câu hỏi nào đã giúp user kể một tình huống cụ thể?
Câu hỏi có cụm “lần gần đây nhất” giúp Minh Tâm nhắc tới việc học lại kiến thức trên video để chuẩn bị thi (~00:30–00:40 theo transcript). Đây là điểm mở được bối cảnh thực tế, nhưng câu hỏi còn kèm giả định “slide quá nhiều”, “video quá dài” và ngưỡng 30 phút. Câu chuyện chưa được neo vào ngày, bài học và hành động ghi chú cụ thể. Ở lần tiếp theo, dùng opener về lần đã ghi chú/highlight/lưu nội dung trong 7 ngày rồi hỏi tiếp trình tự hành động.

### 2. Chỗ nào cần làm tốt hơn ở lần phỏng vấn thật?
Lượt luyện có nhiều câu đóng hoặc gợi sẵn khó khăn, đặc biệt tình huống giảng viên chuyển slide khi người học chưa hiểu. Đoạn giải thích công cụ AI trong/ngoài hệ thống làm interviewer nói nhiều và đưa nhận định của mình vào cuộc trò chuyện. Câu “bạn sẽ làm cách nào” lấy cách làm chung thay vì hành động ở một lần cụ thể.

Cách cải thiện là theo một câu chuyện xuyên suốt: hỏi bài/ngày cụ thể, người học đã lưu gì và bằng cách nào, khó khăn xảy ra ở bước nào, đã xử lý ra sao, lần mở lại ghi chú và hậu quả thực tế. Không tự nêu lợi ích công cụ; khi câu trả lời chuyển sang khó hiểu thuật ngữ, đào sâu để kiểm tra liệu đây mới là barrier chính. Không suy việc không ghi chú hoặc quên ngày hôm sau từ một câu trả lời chưa rõ.

### 3. Sau khi luyện, Conversation Guide được sửa ở đâu và vì sao?
Trong bản bài nộp này, guide đã được chỉnh với hỗ trợ Codex dựa trên transcript: thêm recruitment check trong 7 ngày; đổi opener từ bài “quá dài” sang lần đã lưu nội dung; đổi câu tương lai thành câu hỏi quá khứ; bỏ phần giải thích AI Tutor; bổ sung câu hỏi về lần sử dụng lại ghi chú, workaround và hậu quả. Big 3 có câu hỏi kiểm tra tài liệu có sẵn đã đủ hay chưa, để evidence có thể làm giả thuyết yếu đi.

Những sửa đổi này giúp guide bám Case B và giảm dẫn dắt. Đây là thay đổi biên tập hiện có trong repo, chưa có xác nhận cả nhóm đã thống nhất chúng trong giờ lab.

## 5. AI Support Log
- Codex đã đọc yêu cầu lab, tạo khung repo, tích hợp nội dung bài nhóm từ Google Docs và điền thông tin nhóm do người học xác nhận. Đã bổ sung nhận xét đối chiếu transcript để hỗ trợ người học tự viết reflection, có ghi rõ nguồn AI.
- Codex dùng transcript đính kèm để tổ chức Interview Record, tách evidence/diễn giải, rà soát câu hỏi dẫn dắt và đề xuất guide sửa đổi.
- Transcript do người học cung cấp tự ghi là nhận dạng tự động bằng Zipformer tiếng Việt và Whisper turbo, phân vai suy từ nội dung. Các đoạn `[...]`, `[?]` và tên công cụ chưa được kiểm chứng bằng nghe lại trong lần rà soát này.
- Codex không nghe trực tiếp audio trong lần này, không xác nhận tên thật/công cụ nghe chưa rõ; không tạo interview data hoặc quote mới; đã hỗ trợ biên tập reflection từ transcript theo yêu cầu người học, có công khai nguồn hỗ trợ và chưa coi bước tự nghe lại là hoàn tất.
- Điểm AI/transcript cần sửa: phần tổng hợp pain suy từ câu hỏi thành facts về video >30 phút, việc rời bài học/mất ngữ cảnh và hoàn toàn không ghi chú. Đã loại các kết luận này khỏi evidence xác nhận. Không dùng sự im lặng hoặc việc không phản bác làm bằng chứng đồng ý.
- Người học xác nhận Minh Tâm đã ghi chú trong 7 ngày trước phỏng vấn. Reflection được hoàn thiện từ bản chép; việc tự nghe lại, sửa từ nghe chưa rõ và thống nhất guide trong nhóm chưa được xác nhận.

## Bản ghi và checklist nộp
- Bản ghi nộp: `interview/recording.m4a` (file gốc đã cung cấp; không cần recording-link.md). Bản ghi được đưa vào repo GitHub riêng tư cùng bài nộp; giảng viên/TA cần được cấp quyền xem repo.
- Bản chép và tổng hợp gốc: `interview/transcript-source.txt` (lưu cục bộ, không coi phần tổng hợp là facts).
- Link nộp GitHub chứa cả bản ghi trong repo riêng tư. Cần mời giảng viên/TA truy cập repo; không chuyển repo sang công khai.

- [x] Repo đúng tên; README có 5 phần; có notes từ dữ liệu thực tế.
- [x] Không tuyên bố validated; guide đề xuất không pitch solution.
- [x] Hoàn tất tên nhóm và ba thành viên theo thông tin người học cung cấp.
- [x] Ngày 04/10/2026; Dũng phỏng vấn Minh Tâm thuộc nhóm khác, theo xác nhận của người học.
- [x] Recruitment Case B: Minh Tâm đã ghi chú trong 7 ngày, theo xác nhận của Dũng.
- [ ] Nghe lại các đoạn không rõ và xác nhận consent ghi âm.
- [x] Có ba câu trả lời reflection từ transcript, ghi rõ hỗ trợ AI.
- [ ] Tự nghe lại để rà soát reflection và xác nhận thay đổi guide với nhóm.
- [x] Có file interview/recording.m4a, không yêu cầu link thay thế.
- [ ] Cấp quyền giảng viên/TA xem repo riêng tư và kiểm tra mở được bản ghi.
- [ ] Kiểm tra yêu cầu lượt luyện 15 phút: file hiện có được transcript mô tả dài 3 phút 25 giây; chưa rõ đây là toàn bộ lượt hay một phần.
