# DailyHot for LazyCat

DailyHot trending dashboard: web v1.2.0 (built locally from imsyy/DailyHot, embedded via contentdir) + API v2.0.8 (ghcr.io/imsyy/dailyhotapi mirror delivery).

## Architecture

- upstream `/api/` -> API container (prefix trimmed, default behavior)
- upstream `/` -> file:///lzcapp/pkg/content/dist/ (prebuilt static web, hash router, VITE_GLOBAL_API=/api baked at build)

## Publication

MiaoMiao community store app 666, APPROVED, version 2.0.8. Build run 41104373084, mirror verification passed for ghcr.io/imsyy/dailyhotapi:v2.0.8 (digest sha256:3d950077...). LPK 1280512 bytes, SHA256 f4b13bbe5c391bf089158c7e1a684b2f6e8fddecadae3b88d04a4f008c0921ef downloaded independently and matched at submission.

Build history: 2 failures (content/ directory excluded by .gitignore; fixed with force-add). Full duplicate check (dailyhot query) returned 0 before submission.

No smoke job, no file-chooser interceptor. Configuration and synthetic checks only; per-source trending availability not verified on a live device.
