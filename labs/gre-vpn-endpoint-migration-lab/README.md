# GRE VPN Endpoint Migration

A site-to-site GRE tunnel has just moved to new ISP addresses. The tunnel comes up, but the two sites still can't reach each other's services. Find what the migration missed.

![The GRE VPN endpoint migration lab open in PNETLab: ChiEdge, ChiFW, ISP, AusFW and AusEdge in a line, plus symptom, objectives, checklist and topology facts cards](../../images/gre-vpn-endpoint-migration-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/gre-vpn-endpoint-migration-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (50 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/gre-vpn-endpoint-migration-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Audit the two-site GRE topology and find the loopbacks that stand in for each site's services
- Verify tunnel source and destination after the move to new ISP IPs
- Re-establish the routing adjacency that runs across the tunnel
- Verify overlay route propagation and tunnel MTU
- Confirm cross-site reachability between the service loopbacks after cutover

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
scp gre-vpn-endpoint-migration-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: Cisco · SVPN · Platform: IOL L3 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
