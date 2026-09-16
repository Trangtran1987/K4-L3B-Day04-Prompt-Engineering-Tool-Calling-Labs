# TEAM — Day04, K4-L3B

**Làm nhóm.** Mỗi người tự viết và commit phần INDIVIDUAL của mình.

## Thông tin bài nộp

- Tên nhóm: Độc lập
- Người đại diện : Trần Thị Thu Trang / MSSV:2A202602581
- Tên repo: `K4-L3-DAY04-Tranthithutrang-2A202602581-PromptEngineeringToolCalling`
- URL repo, nhánh nộp, commit chốt: URL: https://github.com/Trangtran1987/K4-L3B-Day04-Prompt-Engineering-Tool-Calling-Labs ; nhánh: `main` ; commit chốt: CHỜ COMMIT SAU CÙNG
- Deadline áp dụng và link thông báo đổi hạn nếu có:

## Thành viên

| Họ và tên | MSSV | GitHub | Vai trò và công việc | File/commit/PR |
| Trần Thị Thu Trang | 2A202602581 | trang1987 | Làm toàn bộ project: prompt, tool declarations, eval, report và evidence | `starter_v0/artifacts/system_prompt.md`; `starter_v0/artifacts/tools.yaml`; `starter_v0/artifacts/version_log.csv`; `starter_v0/data/eval_group.json`; `starter_v0/artifacts/REPORT.md`; commit: CHỜ COMMIT SAU CÙNG; PR: N/A |

## Nhận xét chung

- Kết quả và bằng chứng: Base v3 đạt 30/30, group eval đạt 10/10; adversarial run mới nhất đạt 10/12. Evidence nằm trong `starter_v0/runs/`, `starter_v0/artifacts/version_log.csv` và `starter_v0/artifacts/REPORT.md`.
- Thay đổi hiệu quả nhất: Làm rõ routing giữa service/device/user/KB, bắt buộc tham số quan trọng và thêm boundary cho confirmation, prompt injection, credential và external search.
- Giới hạn còn lại: Adversarial vẫn còn lỗi A05 và A12 trong run mới nhất; cần review thủ công tool results và filesystem trước khi nộp.
- Cách phân công và tích hợp: Làm cá nhân; prompt, tools, eval, report và evidence được tích hợp trong cùng repository.

## INDIVIDUAL

Sao chép mục này cho từng thành viên.

### Trần Thị Thu Trang — 2A202602581

- Phần việc và file/commit/PR: Cải thiện `starter_v0/artifacts/system_prompt.md` và `starter_v0/artifacts/tools.yaml`; tạo `starter_v0/data/eval_group.json`; cập nhật `starter_v0/artifacts/version_log.csv` và `starter_v0/artifacts/REPORT.md`; commit: CHỜ COMMIT SAU CÙNG; PR: N/A.
- Quyết định, khó khăn và cách xử lý: Dùng run v0 để xác định lỗi routing, argument, missing information và confirmation; chạy lại v1-v3 cùng bộ base; loại các run có provider error khỏi evidence.
- Điều đã học: Cần phân biệt provider error với lỗi hành vi model; phải đọc cả expected, actual tool calls và tool results; confirmation phải gắn với đúng payload hiện tại.
- AI/công cụ đã dùng và cách kiểm tra: GitHub Copilot, Python, OpenRouter; kiểm tra bằng `run_eval.py`, JSON run artifacts, provider error count và metric summary.
- Thời điểm đã tự nộp URL repo chung trên VLearn: 
