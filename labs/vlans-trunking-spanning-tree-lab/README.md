# VLANs, Trunking & Spanning Tree

A distribution switch, two access switches and four hosts in VLANs 10 and 20. PC1 can't reach PC2 or its gateway: work through the trunks, the native VLAN and spanning tree.

![The VLANs, trunking and spanning tree lab open in PNETLab: SW-DIST trunked to SW-ACC1 and SW-ACC2 with four hosts, plus symptom, objectives and checklist cards](../../images/vlans-trunking-spanning-tree-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/vlans-trunking-spanning-tree-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (50 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/vlans-trunking-spanning-tree-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Configure 802.1Q trunks and verify dot1q encapsulation
- Identify and fix a native VLAN mismatch across switch trunks
- Verify VLAN creation and access port assignments (VLAN 10 and 20)
- Inspect spanning tree root bridge election and port states
- Verify inter-VLAN routing and host reachability across all switches

## What's in the file

- The topology, with every node and cable in place
- Startup configs with the fault already in them
- Canvas notes: symptom, objectives, investigation checklist and topology facts
- A step-by-step walkthrough workbook

## Node image

The file does not include node images. It expects your own licensed copy of:

- `i86bi_Linux-L2-Adventerprisek9-ms.SSA.high_iron_20190423.bin`

If your copy has a different name, open each node's Edit dialog after importing and pick your image from the list.

## Setup

Replace `<your-server>` with the IP address or hostname of your EVE-NG or PNETLab server.

```bash
scp vlans-trunking-spanning-tree-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNA · 200-301 · Platform: IOL L2 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
