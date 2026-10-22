# Static Route: Wrong Next Hop

R1's static route to a remote LAN never shows up in the routing table. Find out why, repair it, and prove the remote LAN is reachable.

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/static-route-wrong-next-hop-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (38 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/static-route-wrong-next-hop-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Read a prefix-specific route lookup
- Distinguish a destination network from its next hop
- Replace an invalid static route safely
- Verify both the routing table and end-to-end reachability

## What's in the file

- The topology, with every node and cable in place
- Startup configs with the fault already in them
- Canvas notes: symptom, objectives, investigation checklist and topology facts
- A step-by-step walkthrough workbook

## Node image

The file does not include node images. It expects your own licensed copy of:

- `iosv-159-3-m6`

## Setup

Replace `<your-server>` with the IP address or hostname of your EVE-NG or PNETLab server.

```bash
scp static-route-wrong-next-hop-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNA · 200-301 · Platform: vIOS · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
