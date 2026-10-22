# DHCP Snooping: Trust Boundary Misconfiguration

Three switches run DHCP snooping. PC1 gets a lease, PC2 never does. Trace the trust boundary to the port dropping the server's replies.

![The DHCP snooping lab open in PNETLab: SW-CORE with two access switches and PCs, the untrusted uplink marked, plus symptom, objectives and checklist cards](../../images/dhcp-snooping-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/dhcp-snooping-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (45 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/dhcp-snooping-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Confirm DHCP snooping is enabled consistently across a small switched network
- Read show ip dhcp snooping and identify a switch's trusted interfaces
- Use show ip dhcp server statistics to prove the server is answering
- Recognize a DHCP snooping trust boundary problem from those two outputs together
- Apply ip dhcp snooping trust on the correct uplink and verify the fix

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
scp dhcp-snooping-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNA · 200-301 · Platform: IOL L2 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
