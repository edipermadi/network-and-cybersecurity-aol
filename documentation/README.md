# Documentation

## Topology

### Hosts

| Level | Name         | IP           | Network        | Gateway     |
|-------|--------------|--------------|----------------|-------------|
| 1     | Shop PC      | 192.168.1.10 | 192.168.1.1/24 | 192.168.1.1 |
| 2     | Dev 1        | 192.168.2.10 | 192.168.2.1/24 | 192.168.2.1 |
| 2     | Dev 2        | 192.168.2.11 | 192.168.2.1/24 | 192.168.2.1 |
| 2     | Build Server | 192.168.2.12 | 192.168.2.1/24 | 192.168.2.1 |
| 3     | Admin 1      | 192.168.3.10 | 192.168.3.1/24 | 192.168.3.1 |
| 3     | Admin 2      | 192.168.3.11 | 192.168.3.1/24 | 192.168.3.1 |
| 3     | Printer      | 192.168.3.12 | 192.168.3.1/24 | 192.168.3.1 |

## Security

- Floor isolation (No cross talk between floors)
- Each host can access internet (port 80/443 only)
- Block port scanning

## Proof of Concept

### Level 1 PC Can Access Internet

![Level 1 PC Can Access Internet](level1-pc-can-access-internet.png)

### Level 1 PC Cannot Access Gitlab

![Level 1 PC Cannot Access Gitlab](level1-pc-cannot-access-gitlab.png)

### Level 2 PC Can Cross Talk

![Level 2 PC Can Cross Talk](level2-pc-can-cross-talk.png)

### Level 2 PC Can Access Internet

![Level 2 PC Can Access Internet](level2-pc-can-access-internet.png)

### Level 2 PC Can Access Gitlab

![Level 2 PC Can Access Gitlab](level2-pc-can-access-gitlab.png)

### Level 2 PC Cannot Access Printer

![Level 2 PC Cannot Access Printer](level2-pc-cannot-access-printer.png)

### Level 3 PC Can Cross Talk

![Level 3 PC Can Cross Talk](level3-pc-can-cross-talk.png)


### Level 3 PC Can Access Internet

![Level 3 PC Can Access Internet](level3-pc-can-access-internet.png)

### Level 3 PC Can Access Printer

![Level 3 PC Can Access Printer](level3-pc-can-access-printer.png)

### Level 3 PC Cannot Access Gitlab

![Level 3 PC Cannot Access Gitlab](level3-pc-cannot-access-gitlab.png)
