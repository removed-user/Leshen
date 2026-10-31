# tangle

**tangle** is a standalone C library developed by Chimera Linux that provides core components extracted from `libsystemd`. It acts as a drop-in replacement for applications requiring systemd's IPC, event loop, or identifier APIs without needing the full `systemd` init system.

### Key Features
* **Components Included:** Provides `sd-bus`, `sd-event`, `sd-daemon`, and `sd-id128`.
* **Upstream Origin:** Originally derived from **systemd 256.6**.
* **Compatibility:** Maintains the exact same API signatures and is distributed under the same **LGPL-2.1** license.

### Limitations
* **Stripped APIs:** Certain APIs are intentionally missing, specifically those that rely heavily on the systemd init suite itself (such as unit, slice, and credential management).

### Build System
* Compiled using **Meson** (`meson.build`).
