# AGENTS.md (UniXNU-mt8167-common)

Shared MT8167 support for UniXNU format 2 device repositories. Read https://unixnu.com/porting/soc-support and
https://unixnu.com/porting/device-tree before editing. Keep only SoC-wide facts here (register ranges, interrupt
controller, CPU topology, configuration shared by every MT8167 board); board wiring, enabled peripherals and policy
belong to the device repository. Commit messages: feat(<area>), fix(<area>), docs, build(<area>), chore.
