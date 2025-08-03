# enable-kvm-action

## Running hardware accelerated emulators on Linux runners

GitHub's [larger Linux runners support running hardware accelerated emulators](https://github.blog/changelog/2023-02-23-hardware-accelerated-android-virtualization-on-actions-windows-and-linux-larger-hosted-runners/) which is [free for public GitHub repos](https://github.blog/2024-01-17-github-hosted-runners-double-the-power-for-open-source/). It is now recommended to use the **Ubuntu** (`ubuntu-latest`) runners which are 2-3 times faster than the **macOS** ones which are also a lot more expensive. Remember to enable KVM in your workflow before running this action:

```
- name: Enable KVM group perms
  uses: ndtp/enable-kvm-action@v1
```
