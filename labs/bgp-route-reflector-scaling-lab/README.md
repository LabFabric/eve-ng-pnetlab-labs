# BGP Route Reflector Scaling

Two route reflectors serve three clients in one AS, and one client is missing a route every other router has. Trace the reflected route to the loop check that drops it.

![The BGP route reflector lab open in PNETLab: route reflectors R1 and R2 above clients R3, R4 and R5, plus symptom, objectives, checklist and topology facts cards](../../images/bgp-route-reflector-scaling-lab.jpg)

**[Download the .unl from LabFabric](https://labfabric.pro/free-labs/bgp-route-reflector-scaling-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)** (46 KB, free, CC BY 4.0)

No lab server? [Practise it in your browser](https://labfabric.pro/guided-labs/bgp-route-reflector-scaling-lab?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs) instead.

## What you'll practise

- Trace a reflected route from client to route reflector to client
- Read the ORIGINATOR_ID and CLUSTER_LIST a reflector adds
- See how cluster-IDs stop reflection loops between two reflectors
- Verify cluster-ID loop prevention and originator-ID handling
- Troubleshoot a client that isn't receiving reflected routes

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
scp bgp-route-reflector-scaling-lab.unl root@<your-server>:/opt/unetlab/labs/
# then, logged in to the server:
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

Open the lab from the lab list and start the nodes.

---

Exam: CCNP · ENARSI · Platform: IOL L3 · [All free labs](https://labfabric.pro/free-labs?utm_source=github&utm_medium=referral&utm_campaign=eve-ng-pnetlab-labs)
