# 🛠️ Developer Tools Mastery

> The tools you use 8 hours a day. Master them or be mastered by them.

---

## 🔀 Git (Beyond `git add . && git commit`)

| Resource | Link |
|----------|------|
| Pro Git Book (free) | [git-scm.com/book](https://git-scm.com/book/en/v2) |
| Git Flight Rules (problem → solution) | [github.com/k88hudson/git-flight-rules](https://github.com/k88hudson/git-flight-rules) |
| Oh Shit, Git!?! | [ohshitgit.com](https://ohshitgit.com/) |
| Learn Git Branching (interactive) | [learngitbranching.js.org](https://learngitbranching.js.org/) |
| Git Internals (how it actually works) | [YouTube](https://www.youtube.com/results?search_query=git+internals+how+git+works) |
| Conventional Commits | [conventionalcommits.org](https://www.conventionalcommits.org/) |

### Advanced Git

| Technique | When |
|-----------|------|
| `git rebase -i` | Clean up history before PR |
| `git bisect` | Find which commit introduced a bug |
| `git worktree` | Work on multiple branches simultaneously |
| `git reflog` | Recover "lost" commits |
| `git stash` | Temporarily shelve changes |
| `git cherry-pick` | Apply specific commits across branches |
| `git blame -w -M -C` | Ignore whitespace, detect moves/copies |

---

## 🐳 Docker (Beyond `docker run`)

| Resource | Link |
|----------|------|
| Docker Curriculum | [docker-curriculum.com](https://docker-curriculum.com/) |
| Docker Best Practices | [docs.docker.com/develop/develop-images/dockerfile_best-practices](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/) |
| Multi-stage Builds | [docs.docker.com/build/building/multi-stage](https://docs.docker.com/build/building/multi-stage/) |
| Docker Security | [snyk.io/blog/10-docker-image-security-best-practices](https://snyk.io/blog/10-docker-image-security-best-practices/) |
| Dive (inspect image layers) | [github.com/wagoodman/dive](https://github.com/wagoodman/dive) |

---

## 🖥️ Terminal & Shell

| Tool | What | Link |
|------|------|------|
| tmux | Terminal multiplexer | [github.com/tmux/tmux/wiki](https://github.com/tmux/tmux/wiki) |
| zsh + Oh My Zsh | Enhanced shell | [ohmyz.sh](https://ohmyz.sh/) |
| starship | Cross-shell prompt | [starship.rs](https://starship.rs/) |
| fzf | Fuzzy finder (Ctrl+R on steroids) | [github.com/junegunn/fzf](https://github.com/junegunn/fzf) |
| ripgrep (rg) | Fast grep | [github.com/BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep) |
| fd | Fast find | [github.com/sharkdp/fd](https://github.com/sharkdp/fd) |
| bat | cat with syntax highlighting | [github.com/sharkdp/bat](https://github.com/sharkdp/bat) |
| eza | Modern ls | [github.com/eza-community/eza](https://github.com/eza-community/eza) |
| zoxide | Smarter cd | [github.com/ajeetdsouza/zoxide](https://github.com/ajeetdsouza/zoxide) |
| lazygit | Git TUI | [github.com/jesseduffield/lazygit](https://github.com/jesseduffield/lazygit) |
| lazydocker | Docker TUI | [github.com/jesseduffield/lazydocker](https://github.com/jesseduffield/lazydocker) |

---

## 📝 Editors & IDEs

| Editor | Best For | Link |
|--------|----------|------|
| Vim/Neovim | Speed, remote, everywhere | See [dotvim repo](https://github.com/GauravAgarwalGarg/dotvim) |
| VS Code | General development | [code.visualstudio.com](https://code.visualstudio.com/) |
| JetBrains (Community) | Java, Python, C++ (free editions) | [jetbrains.com](https://www.jetbrains.com/community/education/) |
| Helix | Modal editor (modern Vim alternative) | [helix-editor.com](https://helix-editor.com/) |
| Zed | Fast, collaborative | [zed.dev](https://zed.dev/) |

---

## 🔍 Debugging & Profiling

| Tool | Language | Link |
|------|----------|------|
| GDB | C/C++ | [sourceware.org/gdb](https://sourceware.org/gdb/) |
| Valgrind | Memory (C/C++) | [valgrind.org](https://valgrind.org/) |
| AddressSanitizer | Memory (C/C++) | [clang.llvm.org/docs/AddressSanitizer](https://clang.llvm.org/docs/AddressSanitizer.html) |
| perf | Linux profiling | [perf.wiki.kernel.org](https://perf.wiki.kernel.org/) |
| strace | Syscall tracing | [strace.io](https://strace.io/) |
| pdb / ipdb | Python | Built-in |
| Chrome DevTools | JavaScript | Built-in |
| Wireshark | Network | [wireshark.org](https://www.wireshark.org/) |

---

## 📦 Package Managers & Build Tools

| Tool | Language/Ecosystem | Link |
|------|-------------------|------|
| CMake | C/C++ | [cmake.org](https://cmake.org/) |
| Conan | C/C++ packages | [conan.io](https://conan.io/) |
| pip / Poetry / uv | Python | [python-poetry.org](https://python-poetry.org/) |
| npm / pnpm / bun | JavaScript | [pnpm.io](https://pnpm.io/) |
| Cargo | Rust | [doc.rust-lang.org/cargo](https://doc.rust-lang.org/cargo/) |
| Go modules | Go | [go.dev/ref/mod](https://go.dev/ref/mod) |
| Maven / Gradle | Java | [gradle.org](https://gradle.org/) |
| Nix | Reproducible builds | [nixos.org](https://nixos.org/) |
| Bazel | Monorepo builds | [bazel.build](https://bazel.build/) |

---

## 📓 From Learning Log

| Course | Platform | Link |
|--------|----------|------|
| The Missing Semester (Shell, Git, Vim, etc.) | MIT (YouTube) | [YouTube Playlist](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J) |
| Build Apps with Windsurf's AI Coding Agents | DeepLearning.AI | [deeplearning.ai](https://www.deeplearning.ai/short-courses/build-apps-with-windsurfs-ai-coding-agents/) |
| How Anthropic Built Claude Code | YouTube | [YouTube](https://www.youtube.com/watch?v=PQU9o_5rHC4) |
| Prompt Driven Development Series (9 videos) | YouTube | [YouTube Playlist](https://www.youtube.com/playlist?list=PLj6YeMhvp2S6SxK3u_W5oN5neaZUpYK3O) |
| Debug Python inside Docker using debugpy | YouTube | [YouTube](https://www.youtube.com/watch?v=ywfsLKRLmf4) |
| Technical Writing One | Google | [developers.google.com](https://developers.google.com/tech-writing/one) |

---
*Cross-references: [Bash](../languages/bash.md) · [Cloud Track](../tracks/cloud-devops.md) · [Best Practices](best-practices.md)*
