# Dùng Studio Hub với Codex

Mở đúng checkout của Hub trong Codex để dùng `$nama-studio-router`. Skill định tuyến ca game và nạp tài liệu chuyên môn từ catalog hiện có. Các vai trong `.codex/agents/` là cấu hình subagent riêng của repo, không thay thế vai hoặc script cho Claude đang có.

Ví dụ: “Dùng $nama-studio-router. Với dự án Godot này, giao studio_graph_mapper khảo sát đường đi từ input tới hiệu ứng, studio_pixel_vfx đề xuất một effect nhặt vật phẩm, và studio_qa ghi checklist nghiệm thu. Chỉ nghiên cứu, chưa sửa game.”

Khi làm việc trong một repo game khác, đừng mặc định repo đó đã có các vai này: cấu hình phải hiện diện và được tin cậy trong đúng checkout. Tệp TOML là cấu hình Codex, không phải agent chạy nền. [Tài liệu OpenAI về subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents).
