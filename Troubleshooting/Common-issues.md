## Issue 1 : Loopback interfaces were unreachable.
Cause : Missing OSPF advertisements.
Resolution: Advertised the loopback networks in OSPF.

## Issue 2 : Leaf Router could not reach Spine Router.
Cause : Incorrect IP addressing.
Resolution : Verified interface addressing and corrected subnet configuration.

## Issue 3 : OSPF neighbors remained in Down state.
Cause : Interface configuration mismatch.
Resolution : Verified interface status and OSPF network statements.

## Issue 4 : Packet Tracer limitation.
Cause : VXLAN EVPN features are not supported.
Resolution : Implemented the Layer 3 underlay while studying VXLAN architecture conceptually.
