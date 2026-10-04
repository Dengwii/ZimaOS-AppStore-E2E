# ZimaOS AppStore E2E Source

"
    "This public repository is a dedicated ZimaOS App Store v2 fixture. It is not a general-purpose community store.

"
    "## Included applications

"
    "- ddns-go
"
    "- Vaultwarden
"
    "- Gitea
"
    "- Sure
"
    "- Monica

"
    "## Test model

"
    "The stable `main` branch is the initial-version baseline. Each E2E run creates a unique temporary branch, rewrites the store ID and base URL for that branch, adds the branch's `store.json` through the real ZimaOS WebUI, and publishes controlled version changes only to that temporary branch. The run removes the source and deletes the temporary branch after cleanup.

"
    "Source Compose files copied from `Dengwii/CasaOS-AppStore` are kept under `source/Apps/`; the WebUI-consumable v2 output is under `apps/` with `store.json` and `index.json` at the repository root.

"
    "## 中文说明

"
    "这是专用于 ZimaOS WebUI 自动化测试的公开 v2 应用源，不是普通社区商店。稳定的 `main` 分支保存初始版本；每轮测试使用唯一临时分支模拟升级，测试完成后删除设备中的测试源和远程临时分支，不修改正式应用源。
"
    