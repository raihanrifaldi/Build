# Build
Build Minecraft Server wit Google Cloud 100% FREE

```sh-session

```

**Task 1. Create the VM**
Define a VM using advanced options
1. In the Cloud Console, on the Navigation menu (Navigation menu), click **Compute Engine** > **VM instances**.
2. Click **Create Instance**.
3. Specify the following and leave the remaining settings as their defaults:

| Name | mc-server |
| --- | --- |
| Region | `REGION` |
| Zone | `ZONE` |
| Boot disk | Debian GNU/Linux 12 (bookworm) |
| Identity and API access > Access scopes | Set access for each API |
| Storage | Read Write |

4. Click **Advanced options.**
5. Click **Disks**. You will add a disk to be used for game storage.
6. Click **Add new disk**.
7. Specify the following and leave the remaining settings as their defaults: