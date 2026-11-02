# UniXNU-mt8167-common

Shared UniXNU support for the MediaTek MT8167 SoC (4x Cortex-A35, GIC-400, MSDC eMMC, PowerVR GE8300), selected by
device repositories with `soc_source = "mt8167"` and a `kind = "soc"` entry in their `feeds.toml`.

| Path | Content |
| --- | --- |
| `soc.toml` | SoC identity and the components every MT8167 board selects |
| `dts/mt8167.dtsi` | CPU, PSCI, GIC-400, UART0 and MSDC0 resources exported to the ADT |
| `configs/mt8167.config` | Kernel configuration fragment (GICv2 interrupt path, 16550 console) |
| `patches/xnu/series` | SoC patch series: secondary CPUs (native-smp-secondary), the original-PMGR hook (sheng-platform-power), the MSDC eMMC personality (mt8167-msdc-personality) |

Boards: [UniXNU-a04br3](https://github.com/mouseos/UniXNU-a04br3) (Benesse TAB-A04-BR3).
See https://unixnu.com/porting/soc-support.
