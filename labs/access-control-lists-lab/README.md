# Access Control Lists: Configuring & Verifying

PC1 pings a server through R1 and gets an explicit deny back, even though the ACL looks like it permits PC1's subnet. Find out what the router actually stored.

![The access control lists lab open in PNETLab: R1 between PC1 and SRV1 with the ACL applied inbound on Ethernet1/0, plus symptom, objectives, checklist and topology facts cards](../../images/access-control-lists-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/access-control-lists-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (49 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/access-control-lists-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Configure an extended ACL with permit/deny entries and wildcard masks
- Apply an ACL to an interface in the correct direction (in vs out)
- Read show access-lists and show ip interface to verify ACL placement
- Understand wildcard masks and how they differ from subnet masks
- Diagnose a host caught by an ACL's implicit deny

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
scp access-control-lists-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNA · 200-301 · Platform: IOL L3 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
