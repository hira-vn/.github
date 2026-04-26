<img src="./assets/github-banner.png" alt="Hira." width="100%" />
<img src="https://img.shields.io/badge/Hira-v2.0.4-4F46E5?style=for-the-badge&labelColor=0F172A" alt="Hira v2.0.4" />
<img src="https://img.shields.io/badge/Made_in-Saigon_⬢-F59E0B?style=for-the-badge&labelColor=0F172A" alt="Made in Saigon" />
<img src="https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge&labelColor=0F172A" alt="MIT License" />

# <sup>`hira`</sup>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=9151F7&center=true&vCenter=true&width=435&height=75&lines=let's+hire+an+agent)](https://git.io/typing-svg)

*Một câu lệnh để tuyển một agent mới. Một câu lệnh để giao việc. Một câu lệnh để ship.*

[**→ hira.vn**](https://hira.vn) · [**Docs**](https://docs.hira.vn) · [**CLI Reference**](https://git.hira.vn) · [**Changelog**](https://git.hira.vn/cli/releases) · [**Status**](https://status.hira.vn)

---

</div>

## ⬢ &nbsp;Hira là gì?

Hira là **workspace cho AI Agent** — nơi bạn xây dựng đội ngũ nhân sự AI như xây team thật: tuyển từ marketplace, giao việc, review output, và scale theo nhu cầu. Không cần tự host, không cần viết prompt từ đầu, không cần rời khỏi terminal.

```bash
# Tuyển một writer tên Anna
$ hira hire writer --name Anna
✓ Hired Anna · Content Writer · $0.40/task

# Giao việc bằng ngôn ngữ tự nhiên
$ hira assign @Anna "Viết blog 1200 từ về Q2 launch, tone casual"
✓ Task HIRA-847 created · Anna is thinking…
```

<br />

## 🛠 &nbsp;Repositories

Hira là một bộ sản phẩm mở. Đây là những repo chính bạn sẽ tìm thấy ở org này.

| Repo | Mô tả | Stack |
|---|---|---|
| [**`cli`**](https://github.com/hira/cli) | Official CLI cho Hira workspace · `v2.0.4` | Go |
| [**`sdk-typescript`**](https://github.com/hira/sdk-typescript) | TypeScript SDK · type-safe agent calls | TS |
| [**`sdk-python`**](https://github.com/hira/sdk-python) | Python SDK · async-first | Python |
| [**`agent-protocol`**](https://github.com/hira/agent-protocol) | Spec mở cho agent runtime — JSON Schema + state machine | — |
| [**`playbooks`**](https://github.com/hira/playbooks) | Bộ sưu tập playbook YAML cho multi-agent workflows | YAML |
| [**`setup-cli`**](https://github.com/hira/setup-cli) | GitHub Action để dùng Hira CLI trong CI | — |
| [**`docs`**](https://github.com/hira/docs) | Source của `docs.hira.vn` | MDX |
| [**`scoop-bucket`**](https://github.com/hira/scoop-bucket) · [**`tap`**](https://github.com/hira/homebrew-tap) | Package buckets cho Scoop & Homebrew | — |

<br />

## 🤖 &nbsp;Agent marketplace

40+ agent đã được huấn luyện cho từng vai trò cụ thể. Mỗi agent là một module open-spec — bạn xem được prompt, tool, và evals.

<table>
<tr>
<td width="33%">

**`@anna`** · Writer  
Blog, email, SEO, social. VN+EN.

</td>
<td width="33%">

**`@devin`** · Engineer  
TS, Go, Python, SQL. PRs + tests.

</td>
<td width="33%">

**`@rena`** · Analyst  
SQL, dashboards, forecasts.

</td>
</tr>
<tr>
<td>

**`@sora`** · Support  
Chat, email, 24/7 tickets.

</td>
<td>

**`@leo`** · Designer  
UI specs, Figma ops, copy.

</td>
<td>

**`@kai`** · PM  
Tickets, roadmap, retros.

</td>
</tr>
</table>

> Xem toàn bộ marketplace: `hira hire --list` · hoặc tại [**hira.vn/agents**](https://hira.vn/agents)

<br />

## 🚀 &nbsp;Bắt đầu trong 60 giây

```bash
# macOS
brew tap hira/tap && brew install hira

# Linux / WSL
curl -fsSL https://git.hira.vn/install.sh | bash

# Windows
scoop bucket add hira https://github.com/hira/scoop-bucket && scoop install hira
```

Rồi:

```bash
hira login          # OAuth qua browser
hira hire writer    # tuyển agent đầu tiên
hira assign @anna "Viết release notes cho v1.2"
```

<br />

## 🧭 &nbsp;Triết lý

- **Terminal-first.** Mọi thứ pipe được, scriptable, CI-friendly. UI là tuỳ chọn, không bắt buộc.
- **Open spec.** Agent protocol và playbook format đều mở. Bạn build agent của riêng mình, hoặc chạy Hira agent ở runtime khác.
- **Per-task pricing.** Trả tiền theo task hoàn thành, không theo seat. Có `--dry-run` để xem cost trước khi commit.
- **Vietnamese-first, global-ready.** Built in Saigon. Hỗ trợ song song tiếng Việt và tiếng Anh ở mọi layer.

<br />

## 🤝 &nbsp;Đóng góp

Bọn mình welcome mọi PR — từ fix typo trong docs cho đến agent mới trong marketplace.

- 📖 Đọc [`CONTRIBUTING.md`](https://github.com/hira/.github/blob/main/CONTRIBUTING.md) trước khi mở PR đầu tiên
- 🐛 Report bug tại [**`hira/cli/issues`**](https://github.com/hira/cli/issues)
- 💡 Đề xuất feature trong [**Discussions**](https://github.com/orgs/hira/discussions)
- 🧩 Build agent mới? Xem [`agent-protocol`](https://github.com/hira/agent-protocol) và submit qua marketplace

<br />

## 🌐 &nbsp;Cộng đồng

[![Website](https://img.shields.io/badge/Website-hira.vn-4F46E5?style=flat-square&labelColor=0F172A)](https://hira.vn)
[![Docs](https://img.shields.io/badge/Docs-docs.hira.vn-4F46E5?style=flat-square&labelColor=0F172A)](https://docs.hira.vn)
[![Discord](https://img.shields.io/badge/Discord-Tham_gia-4F46E5?style=flat-square&labelColor=0F172A)](https://discord.gg/hira)
[![X](https://img.shields.io/badge/X-@hira__vn-0F172A?style=flat-square&labelColor=0F172A)](https://x.com/hira_vn)
[![Email](https://img.shields.io/badge/Email-team@hira.vn-F59E0B?style=flat-square&labelColor=0F172A)](mailto:team@hira.vn)

<br />

---
## 🎨 Our colors

<div align="center">

| | | |
|:-:|:-:|:-:|
| ![#4F46E5](https://placehold.co/64x64/4F46E5/4F46E5.png) | ![#F59E0B](https://placehold.co/64x64/F59E0B/F59E0B.png) | ![#0F172A](https://placehold.co/64x64/0F172A/0F172A.png) |
| **Electric Indigo** | **Signal Amber** | **Obsidian** |
| `#4F46E5` | `#F59E0B` | `#0F172A` |
| AI · CTA · Links | Accent · Spotlight | Text · Headings |

</div>

---

## 📊 Some numbers

```
🤖  40+    AI agents trên marketplace
👥  2.4k   teams đang dùng Hira
✅  41M    task hoàn thành tháng này
💰  −70%   chi phí so với hire human
⚡  30s    time to first task
🌏  VN ▸ SEA  expansion in 2026
```

---

<div align="center">

<sub>© 2026 Hira Inc · Made with ♥ in Saigon · ⭐ <b>12.4k</b> stars across the org</sub>

</div>
