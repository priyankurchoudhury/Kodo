## 💻 Meet #Kodo: a free AI coding assistant that runs entirely on your own laptop, no internet needed.

**💸 Free: skip the subscriptions**
- A free alternative to paid Claude Code, Codex and Cursor plans
- No API keys, no usage limits, no surprise bills

**📴 Runs without internet**
- Connect once to download & set up, then code on a plane, in a cafe, anywhere.

**⚙️ Setup that sizes up your laptop**
- Detects your chip, memory, GPU (Apple or NVIDIA) and disk space
- Recommends the model your machine runs smoothly, or CPU mode if there's no GPU

**🔎 Always up to date with web search**
- Looks up the latest releases in Web so no retraining needed
- Free, with no paid search API

**🤖 What it does**
- Claude Code-style agent: plans, edits files, runs tests, fixes bugs
- Up to 512K-Context Window (about 40,000 lines of code), with auto-compaction
- No network round trips or server queues; Kodo also pre-loads the LLM while you type
- Session History stored in your local for future reference

**🧠 Which LLM models does it support?**
- Mini: Qwen 3.5 (4B), for 8 GB laptops
- Light: Ornith 1.5 (9B), for 16 GB+ machines
- Smart: Ornith 1.5 (35B, mixture-of-experts), for Macs with 48 GB+ tested
- Smart (dense): Qwen 3.8 (27B), an option for 32 GB Macs
- Expert: Ornith 1.5 (122B), for 128 GB+ machines

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
