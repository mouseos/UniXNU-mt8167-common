# UniXNU MT8167 common support
Unqualified schema2 migration source for MediaTek MT8167. The Cortex-A35 topology, GICv2, UART0 and MSDC0 resources retain the running a04br3 port's values. Board policy stays in UniXNU-a04br3.

Sources: https://github.com/mouseos/UniXNU-a04br3/tree/1b13730dde947738f57802bc58105f723116f31b and https://github.com/mouseos/uefi-a04br3/tree/8dbdd50713b8fbb79a5f5837a032b46a4a939723. The vendor source tree is CT3_GPL_LGPL_Src/kernel-4.4; this is source provenance, not a new chip qualification.

Select the reviewed commit through a device feed and include dts/mt8167.dtsi. Run the device resolver, DTS compiler and ADT comparison before building. No main-branch or hardware success is claimed.
