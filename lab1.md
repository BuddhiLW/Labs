# Laboratory with a VM - Lab 1 (221113112226-03)

## Tasks

- Install `docker`.
- Run latest `Fedora` in a container.
- Start a interactive mode shell.
- Explore `/etc/os-release`.
- Issue `uname -r`.
- Disconnect from `container`, without shutting it down.

## Commands

- `docker run -it fedora:latest bash`

- `docker run -d fedora:latest`
- `docker exec -it $CNAME /bin/bash `

- `cat /etc/os-release`

```sh
NAME="Fedora Linux"
VERSION="36 (Container Image)"
ID=fedora
VERSION_ID=36
VERSION_CODENAME=""
PLATFORM_ID="platform:f36"
PRETTY_NAME="Fedora Linux 36 (Container Image)"
ANSI_COLOR="0;38;2;60;110;180"
LOGO=fedora-logo-icon
CPE_NAME="cpe:/o:fedoraproject:fedora:36"
HOME_URL="https://fedoraproject.org/"
DOCUMENTATION_URL="https://docs.fedoraproject.org/en-US/fedora/f36/system-administrators-guide/"
SUPPORT_URL="https://ask.fedoraproject.org/"
BUG_REPORT_URL="https://bugzilla.redhat.com/"
REDHAT_BUGZILLA_PRODUCT="Fedora"
REDHAT_BUGZILLA_PRODUCT_VERSION=36
REDHAT_SUPPORT_PRODUCT="Fedora"
REDHAT_SUPPORT_PRODUCT_VERSION=36
PRIVACY_POLICY_URL="https://fedoraproject.org/wiki/Legal:PrivacyPolicy"
VARIANT="Container Image"
VARIANT_ID=container
```

- `dnf install neofetch`
- `neofetch`

```sh
[root@8ca8164eefb8 /]# neofetch
             .',;::::;,'.                root@8ca8164eefb8
         .';:cccccccccccc:;,.            -----------------
      .;cccccccccccccccccccccc;.         OS: Fedora Linux 36 (Container Image) x86_64
    .:cccccccccccccccccccccccccc:.       Host: VirtualBox 1.2
  .;ccccccccccccc;.:dddl:.;ccccccc;.     Kernel: 5.15.0-52-generic
 .:ccccccccccccc;OWMKOOXMWd;ccccccc:.    Uptime: 1 hour, 23 mins
.:ccccccccccccc;KMMc;cc;xMMc:ccccccc:.   Packages: 347 (rpm)
,cccccccccccccc;MMM.;cc;;WW::cccccccc,   Shell: bash 5.2.2
:cccccccccccccc;MMM.;cccccccccccccccc:   Resolution: 800x600
:ccccccc;oxOOOo;MMM0OOk.;cccccccccccc:   CPU: Intel i5-9300H (1) @ 2.400GHz
cccccc:0MMKxdd:;MMMkddc.;cccccccccccc;   GPU: 00:02.0 VMware SVGA II Adapter
ccccc:XM0';cccc;MMM.;cccccccccccccccc'   Memory: 269MiB / 1976MiB
ccccc;MMo;ccccc;MMW.;ccccccccccccccc;
ccccc;0MNc.ccc.xMMd:ccccccccccccccc;
cccccc;dNMWXXXWM0::cccccccccccccc:,
cccccccc;.:odl:.;cccccccccccccc:,.
:cccccccccccccccccccccccccccc:'.
.:cccccccccccccccccccccc:;,..
  '::cccccccccccccc::;,.

```

- `uname -r`

```sh
5.15.0-52-generic
```

- `C-p C-q`
