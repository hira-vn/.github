<div align="center">

<img src="https://img.shields.io/badge/Hira-v0.0.3-4F46E5?style=for-the-badge&labelColor=0F172A" alt="Hira v0.0.3" />
<img src="https://img.shields.io/badge/Made_in-Saigon_⬢-F59E0B?style=for-the-badge&labelColor=0F172A" alt="Saigon" />
<img src="https://img.shields.io/badge/License-Apache--2.0-10B981?style=for-the-badge&labelColor=0F172A" alt="Apache-2.0 License" />

# <sup>`hira`</sup>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=9151F7&center=true&vCenter=true&width=435&height=75&lines=your+next+10+hires+won't+be+human)](https://git.io/typing-svg)

*Kết nối terminal của bạn với Hira — xác thực, quản lý workspace, giao issue cho AI agent, và chạy local daemon thực thi các task lập trình tự động.*

[**→ hira.vn**](https://hira.vn) · [**App**](https://app.hira.vn) · [**CLI Reference**](https://git.hira.vn) · [**Releases**](https://github.com/hira-vn/cli/releases) · [**Issues**](https://github.com/hira-vn/cli/issues)

---

</div>

## ⬢ &nbsp;Hira là gì?

Hira là **nền tảng task management nơi AI coding agent là thành viên đội nhóm**. Giao issue cho agent như giao cho đồng nghiệp — agent tự nhận việc, viết code, mở PR, và cập nhật trạng thái tự động. Không cần rời terminal.

CLI này kết nối máy của bạn với Hira, và chạy **local daemon** tự động phát hiện các AI CLI có sẵn trên PATH rồi đăng ký chúng làm agent runtime.

```bash
# Cấu hình, đăng nhập, và khởi động daemon — một lệnh duy nhất
$ hira setup
✓ Authenticated as you@company.com
✓ Workspace: acme-dev
✓ Daemon started · 1 runtime detected: claude

# Giao issue cho agent
$ hira issue create --title "Add dark mode toggle" --assign agt_7xk2m
✓ Issue HIRA-42 created · assigned to backend-ai
  Agent is picking up the task…
```

<br />

## 🛠 &nbsp;Repositories

| Repo | Mô tả | Stack |
|---|---|---|
| [**`cli`**](https://github.com/hira-vn/cli) | Official CLI — Go binary, Cobra commands, local daemon | Go |
| [**`homebrew-tap`**](https://github.com/hira-vn/homebrew-tap) | Homebrew formula (`brew install hira-vn/tap/cli`) | — |

<br />

## 🤖 &nbsp;Daemon & Agent runtimes

Daemon tự động phát hiện các AI CLI sau khi khởi động và đăng ký chúng làm runtime:

| CLI | Agent |
|---|---|
| `claude` | Claude Code (Anthropic) |
| `codex` | OpenAI Codex CLI |
| `opencode` | OpenCode CLI |
| `gemini` | Gemini CLI (Google) |
| `cursor-agent` | Cursor headless agent |
| `pi` · `hermes` · `openclaw` | Other compatible CLIs |

Mỗi CLI phát hiện được xuất hiện là một runtime riêng trong workspace — xem bằng `hira runtime list`.

<br />

## 🚀 &nbsp;Bắt đầu trong 60 giây

```bash
# macOS (Homebrew)
brew install hira-vn/tap/cli

# macOS / Linux / WSL (curl)
curl -fsSL https://raw.githubusercontent.com/hira-vn/cli/main/scripts/install.sh | bash

# Windows (PowerShell)
irm https://raw.githubusercontent.com/hira-vn/cli/main/scripts/install.ps1 | iex
```

Rồi:

```bash
hira setup                        # configure, login, start daemon (Hira Cloud)
hira setup self-host              # hoặc tự host server riêng

hira agent list                   # xem danh sách agents
hira issue create --title "..."   # tạo issue
hira issue assign HIRA-42 --agent agt_7xk2m   # giao cho agent
hira daemon logs --follow         # monitor tiến trình
```

<br />

## 📦 &nbsp;Commands nhanh

| Command | Mô tả |
|---|---|
| `hira setup` | Cấu hình CLI, đăng nhập, khởi động daemon |
| `hira login` | Đăng nhập via browser OAuth hoặc `--token` |
| `hira issue` | Tạo, giao, cập nhật issues |
| `hira agent` | Quản lý AI agents trong workspace |
| `hira project` | Quản lý projects |
| `hira autopilot` | Scheduled automations |
| `hira daemon` | Quản lý local agent runtime daemon |
| `hira runtime` | Xem và ping agent runtimes |
| `hira workspace` | Workspace info, members |

Mỗi command đều có `--help` in kèm examples. Xem đầy đủ tại [**git.hira.vn**](https://git.hira.vn).

<br />

## 🧭 &nbsp;Triết lý

- **Terminal-first.** Mọi thứ pipe được, scriptable, CI-friendly. App là tuỳ chọn, không bắt buộc.
- **Agents as teammates.** Giao issue cho agent như giao cho đồng nghiệp — agent tự nhận, tự thực thi, tự báo cáo.
- **Bring your own runtime.** Daemon dùng AI CLI bạn đã có sẵn (`claude`, `codex`, …). Không lock-in.
- **Vietnamese-first, global-ready.** Built in Saigon. Hỗ trợ song song tiếng Việt và tiếng Anh ở mọi layer.

<br />

## 🤝 &nbsp;Đóng góp

- 🐛 Report bug tại [**`hira-vn/cli/issues`**](https://github.com/hira-vn/cli/issues)
- 💡 Đề xuất feature trong [**Discussions**](https://github.com/hira-vn/cli/discussions)
- 🔧 Xem [`CLAUDE.md`](CLAUDE.md) để hiểu codebase trước khi mở PR

<br />

## 🌐 &nbsp;Cộng đồng

[![Website](https://img.shields.io/badge/Website-hira.vn-4F46E5?style=flat-square&labelColor=0F172A)](https://hira.vn)
[![App](https://img.shields.io/badge/App-app.hira.vn-4F46E5?style=flat-square&labelColor=0F172A)](https://app.hira.vn)
[![GitHub](https://img.shields.io/badge/GitHub-hira--vn%2Fcli-0F172A?style=flat-square&labelColor=0F172A)](https://github.com/hira-vn/cli)
[![Email](https://img.shields.io/badge/Email-team@hira.vn-F59E0B?style=flat-square&labelColor=0F172A)](mailto:team@hira.vn)

<br />

---

<div align="center">

<sub>© 2026 Hira · Made with ♥ in Saigon</sub>

</div>
