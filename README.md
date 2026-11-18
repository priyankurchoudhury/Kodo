# 🧠 Kodo

**A free, private AI coding assistant for VS Code that runs entirely on your computer.**
One-click setup installs Ollama and an open AI model; includes an agent with auto-compaction, web search and GitHub tools. Works offline after setup.

> ⚠️ **Preview.** Tested on macOS with Apple chips (M-series). Windows and Linux are not tested yet.

---

## ⬇️ Install Kodo in VS Code

### Step 1: Download the file
Download **[kodo-1.0.3.vsix](https://github.com/priyankurchoudhury/Kodo/raw/main/kodo-1.0.3.vsix)** (about 4 MB).
Your browser saves it in your **Downloads** folder.

### Step 2: Add it to VS Code
1. Open **VS Code**.
2. Open the **Extensions** panel: click the four-squares icon on the left, or press **⌘⇧X** (Mac) / **Ctrl+Shift+X** (Windows/Linux).
3. Click the **`···`** menu at the top right of the Extensions panel.
4. Choose **Install from VSIX…**
5. Select **kodo-1.0.3.vsix** from your Downloads folder and click **Install**.
6. When VS Code asks, click **Reload** (or close and reopen VS Code).

<details>
<summary>Prefer the terminal?</summary>

```bash
code --install-extension ~/Downloads/kodo-1.0.3.vsix
```
(This needs VS Code's `code` command. In VS Code: ⌘⇧P → "Shell Command: Install 'code' command in PATH".)
</details>

### Step 3: Set up Kodo (first time only)
1. The **Kodo setup** window opens by itself. If it doesn't, click the 🧠 **Kodo** icon in the left bar.
2. Click **Let's build my AI sidekick** and follow the short steps. Kodo checks your computer, installs the free [Ollama](https://ollama.com) engine and downloads the AI "brain" that fits your computer. The brain download is the long part (5–25 GB). You need internet **only for this step**.
3. When it's done, click **＋ New session** in the Kodo sidebar (or press **⌘⌥A** / **Ctrl+Alt+A**) and start chatting with the agent.

### Updating to a newer version
Download the newer `.vsix` file and repeat **Step 2**. Your settings, brain and sessions are kept.

### Uninstalling
In Kodo's sidebar, click ⚙️ → **Remove everything** (frees the brain's disk space), then uninstall **Kodo** from the Extensions panel.

---

## ✨ What you get

| | |
|---|---|
| 🤖 **The Agent** (Claude Code style) | Plans, edits files, runs commands and tests, and remembers your project (`AGENTS.md` / `CLAUDE.md`). Long sessions **auto-compact** so they keep going. Permission modes (plan / ask first / auto-edit), checkpoints, slash commands, session history and diffs. |
| 🧠 **A local AI brain** | Free, open models picked to fit your computer, running in Ollama. Working memory of 128K, 256K or (experimental) 512K tokens. |
| 🔎 **Free web search** | The AI can search the web and read pages through a separate Chrome window (no paid search service). Optional, off until you turn it on. |
| 🐙 **GitHub** | Open any repository in one click; the AI can read your repositories, issues and pull requests (read-only unless you allow changes). |
| 🔒 **Private** | Your code never leaves your computer. No accounts, no subscriptions, no data collection. |

### Which AI models?
| Brain | Model | For computers with |
|---|---|---|
| Mini | Qwen 3.5 (4B) | 8 GB memory |
| Light | Ornith 1.5 (9B) | 16 GB+ |
| **Smart** ⭐ tested | Ornith 1.5 (35B, mixture-of-experts) | 48 GB+ Macs |
| Smart (dense) | Qwen 3.8 (27B) | 32 GB Macs |
| Expert | Ornith 1.5 (122B) | 128 GB+ |

Kodo recommends the right one for your computer during setup.

## 💻 Computer requirements
- macOS 14+ with an Apple chip (recommended). Windows 10/11 and Linux are untested.
- 8 GB memory minimum (16 GB+ recommended; 48 GB+ for the Smart brain)
- 10–80 GB free disk space, depending on the brain
- Internet **once**, for the downloads

## 💡 Agent tips
| Do this | To… |
|---|---|
| **Shift+Tab** | Switch between *plan* (read-only), *ask first*, and *auto-edit* modes |
| `@file` | Point the agent at a file |
| `/new` | Start a fresh conversation |
| `/compress` | Compact the conversation now (it also happens automatically) |
| `/init` | Create an `AGENTS.md` memory file for your project |
| `/restore` | Undo the agent's file changes |
| `/help` | See every command |

## 🛠️ Troubleshooting
Press **⌘⇧P** / **Ctrl+Shift+P** and run **Kodo: Check My Setup**. Each problem shows what to do. **Kodo: Show Logs** shows details.

## 🔐 Verify the download (optional)
SHA-256 of `kodo-1.0.3.vsix`:
```
2c64d6d05e40903b2f9514e513ee0828a16d82d6f73f72af9c07ae7e7c0eb257
```
Mac: `shasum -a 256 ~/Downloads/kodo-1.0.3.vsix` · Windows: `certutil -hashfile kodo-1.0.3.vsix SHA256`

## 📄 License and credits
Kodo is MIT licensed. It is an independent project, not affiliated with the projects it connects to: [Ollama](https://ollama.com), [Qwen Code](https://github.com/QwenLM/qwen-code) (the agent engine, Apache-2.0), [Continue](https://continue.dev), [llama.cpp](https://github.com/ggml-org/llama.cpp), GitHub's MCP server and Google's Chrome DevTools MCP. AI models are downloaded directly from their publishers under their own licenses.
