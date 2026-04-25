<div align="center">
  <h1>Mole</h1>
  <p><em>Deep clean and optimize your Mac.</em></p>
</div>

## Features

- [x] **All-in-one toolkit**: CleanMyMac, AppCleaner, DaisyDisk, and iStat Menus combined into a **single binary**
- [x] **Deep cleaning**: Scans and removes caches, logs, and browser leftovers to **reclaim gigabytes of space**
- [x] **Smart uninstaller**: Thoroughly removes apps along with launch agents, preferences, and **hidden remnants**
- [x] **Disk insights**: Visualizes usage, manages large files, **rebuilds caches**, and refreshes system services
- [x] **Live monitoring**: Real-time stats for CPU, GPU, memory, disk, and network to **diagnose performance issues**

## Quick Start

### **Install via `Homebrew`:**

```bash
brew install mole
```

### **via script:**

```bash
# Optional args: -s latest for main branch code, -s 1.17.0 for specific version
curl -fsSL https://raw.githubusercontent.com/tw93/mole/main/install.sh | bash
```

#### **Windows**

`Mole` is designed for macOS, but we offer an experimental Windows version based on user demand. See the [windows branch](https://github.com/tw93/Mole/tree/windows) — **early adopters only**.

<details>
  <summary>Commands listing</summary>
  
```bash
mo                           # Interactive menu
mo clean                     # Deep cleanup
mo uninstall                 # Remove apps + leftovers
mo optimize                  # Refresh caches & services
mo analyze                   # Visual disk explorer
mo status                    # Live system health dashboard
mo purge                     # Clean project build artifacts
mo installer                 # Find and remove installer files

mo touchid                   # Configure Touch ID for sudo
mo completion                # Set up shell tab completion
mo update                    # Update Mole
mo remove                    # Remove Mole from system
mo --help                    # Show help
mo --version                 # Show installed version

mo clean --dry-run           # Preview the cleanup plan
mo clean --whitelist         # Manage protected caches
mo clean --dry-run --debug   # Detailed preview with risk levels and file info

mo optimize --dry-run        # Preview optimization actions
mo optimize --debug          # Run with detailed operation logs
mo optimize --whitelist      # Manage protected optimization rules
mo purge --paths             # Configure project scan directories
```
</details>

## Tips

- **Terminal**: iTerm2 has known compatibility issues; we recommend Alacritty, kitty, WezTerm, Ghostty, or Warp.
- **Safety**: Built with strict protections. See [Security Audit](SECURITY_AUDIT.md). Preview changes with `mo clean --dry-run`.
- **Be Careful**: Although safe by design, file deletion is permanent. Please review operations carefully.
- **Debug Mode**: Use `--debug` for detailed logs (e.g., `mo clean --debug`). Combine with `--dry-run` for comprehensive preview including risk levels and file details.
- **Navigation**: Supports arrow keys and Vim bindings (`h/j/k/l`).
- **Status Shortcuts**: In `mo status`, press `k` to toggle cat visibility and save preference, `q` to quit.
- **Configuration**: Run `mo touchid` for Touch ID sudo, `mo completion` for shell tab completion, `mo clean --whitelist` to manage protected paths.
