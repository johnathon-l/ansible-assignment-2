# ansible-assignment-2

**Author**: Johnathon Laun

## Description

This playbook automates the configuration and verification of networking features on a set of routers. Specifically, it will:

1. Configure **THREE loopback interfaces** on each router:
   - **Loopback0:** 10.0.0.X/32 (where X = router number)
   - **Loopback1:** 10.1.1.X/32
   - **Loopback2:** 10.2.2.X/32
2. Configure **EIGRP autonomous system 100**
3. **Advertise all networks** (loopbacks and management network) into EIGRP
4. **Verify** EIGRP neighbors are forming
5. **Display** the configured loopback interfaces

## Usage

To run the playbook, use the following command:

```
ansible-playbook -i inventory.ini assignment2.yaml
```

---
