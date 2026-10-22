# EIGRP Neighbor Down: AS Mismatch

Two routers share a working link and ping each other, but no EIGRP neighbor ever appears, and neither router logs a single message about it. Find the setting that keeps them apart.

![The EIGRP AS mismatch lab open in PNETLab: R1 and R2 linked on Ethernet1/0, plus symptom, objectives and checklist cards](../../images/eigrp-neighbor-as-mismatch-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/eigrp-neighbor-as-mismatch-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (46 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/eigrp-neighbor-as-mismatch-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Bring up a point-to-point EIGRP adjacency between two routers
- Read show ip eigrp neighbors and verify neighbor state
- Understand the EIGRP Autonomous System requirement
- Correct a mismatched AS number on an EIGRP router instance
- Verify adjacency and EIGRP-learned loopback reachability

## What's in the file

- The topology, with every node and cable in place
- Startup configs with the fault already in them
- Canvas notes: symptom, objectives, investigation checklist and topology facts
- A step-by-step walkthrough workbook

## Node image

The file does not include node images. It expects your own licensed copy of:

- `L3-ADVENTERPRISEK9-M-15.4-2T.bin`

If your copy has a different name, open each node's Edit dialog after importing and pick your image from the list.

## Setup

Replace `<your-server>` with the IP address or hostname of your EVE-NG or PNETLab server.

```bash
scp eigrp-neighbor-as-mismatch-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNP · ENARSI · Platform: IOL L3 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
