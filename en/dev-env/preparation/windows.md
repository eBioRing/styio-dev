# Windows

Developing styio compiler on Windows is NOT a wise choice, however, that is my daily life. After suffering from the environment installation, I highly recommend developers using [Docker Container in Visual Studio Code](https://code.visualstudio.com/docs/containers/overview) on Windows.&#x20;

If anyone insists in using MSVC + LLVM, this might be helpful: [MSVC + LLVM](../msvc.md).&#x20;

## Hyper-V

Hyper-V is a virtual machine platform.&#x20;

{% embed url="https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v" %}
Enable Hyper-V
{% endembed %}

It might be well-known that Hyper-V conflicts with many virtual machine platforms, but that is no longer the truth. There are some efforts for the compability:

{% tabs %}
{% tab title="VMware" %}
{% embed url="https://blogs.vmware.com/workstation/2020/05/vmware-workstation-now-supports-hyper-v-mode.html" %}
VMware Workstation with Hyper-V
{% endembed %}
{% endtab %}

{% tab title="VirtualBox" %}
{% embed url="https://docs.oracle.com/en/virtualization/virtualbox/6.0/admin/hyperv-support.html" %}
Oracle VirtualBox with Hyper-V
{% endembed %}
{% endtab %}

{% tab title="Android" %}
{% embed url="https://developer.android.com/studio/run/emulator-acceleration#hypervisors" %}
Android with Hyper-V
{% endembed %}
{% endtab %}

{% tab title="BlueStack" %}
{% embed url="https://support.bluestacks.com/hc/en-us/articles/4412148150157-How-to-enable-Hyper-V-on-Windows-for-BlueStacks-5" %}
BlueStack with Hyper-V
{% endembed %}
{% endtab %}
{% endtabs %}

## WSL2

The 2nd generation of Windows Subsystem for Linux (WSL). There are many Linux distros available.&#x20;

{% embed url="https://learn.microsoft.com/en-us/windows/wsl/install" %}
Install WSL2
{% endembed %}

#### Ubuntu

Ubuntu provides a tutorial for WSL2 installation, which might be the most popular choice:

{% embed url="https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#1-overview" %}
Official Tutorial
{% endembed %}

{% embed url="https://www.omgubuntu.co.uk/how-to-install-wsl2-on-windows-10" %}
Community Tutorial
{% endembed %}

#### Debian

Debian is **free**, and for people who don't like [Canonical](https://canonical.com/).

{% embed url="https://wiki.debian.org/InstallingDebianOn/Microsoft/Windows/SubsystemForLinux" %}
Debian Tutorial
{% endembed %}

#### openSUSE

openSUSE provides an official tutorial, and is up-to-date.

{% embed url="https://en.opensuse.org/openSUSE:WSL" %}
OpenSUSE Tutorial
{% endembed %}

#### RHEL / Fedora / CentOS

Red Hat on Windows, are you serious?&#x20;

#### Arch Linux

One of us has gone insane, not me.

#### Gentoo

Gentoo provides an official tutorial on Gentoo Wiki.

{% embed url="https://wiki.gentoo.org/wiki/Gentoo_in_WSL" %}

## Docker Desktop

{% embed url="https://docs.docker.com/desktop/install/windows-install/" %}
Docker Tutorial: Installation on Windows
{% endembed %}

{% hint style="info" %}
You don't have to use command line, this is the link of installer: [Docker Desktop](https://desktop.docker.com/win/main/amd64/Docker%20Desktop%20Installer.exe).
{% endhint %}
