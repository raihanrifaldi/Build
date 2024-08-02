# Build Minecraft Server with Google Cloud

```sh-session

```

# **Task 1. Create the VM**
Define a VM using advanced options
1. In the Cloud Console, on the Navigation menu (Navigation menu), click **Compute Engine** > **VM instances**.
2. Click **Create Instance**.
3. Specify the following and leave the remaining settings as their defaults:

| Property | Value |
| --- | --- |
| **Name** | mc-server |
| **Region** | `REGION` |
| **Zone** | `ZONE` |
| **Boot disk** | Debian GNU/Linux 12 (bookworm) |
| **Identity and API access > Access scopes** | Set access for each API |
| **Storage** | Read Write |

4. Click **Advanced options.**
5. Click **Disks**. You will add a disk to be used for game storage.
6. Click **Add new disk**.
7. Specify the following and leave the remaining settings as their defaults:

| Property | Value |
| --- | --- |
| **Name** | minecraft-disk |
| **Disk type** | SSD Persistent Disk |
| **Disk Source type** | Blank disk |
| **Size (GB)** | 50 |
| **Encryption** | Google-managed encryption key |

8. Click **Save**. This creates the disk and automatically attaches it to the VM when the VM is created.
9. Click **Networking**.
10. Specify the following and leave the remaining settings as their defaults:

| Property | Value |
| --- | --- |
| **Network tags** | minecraft-disk |
| **Network interfaces** | Click **default** to edit the interface |
| **External IPv4 address** | Reserve Static External IP Address |
| **Name** | mc-server-ip |

11. Click **Reserve**.
12. Click **Done**.
13. Click **Create**.
