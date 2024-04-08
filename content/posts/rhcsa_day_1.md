---
created_date: 2024-04-08
id: RHCSA Bootcamp Day 1
link: "https://learning.oreilly.com/live-events/red-hat-certified-system-administrator-rhcsa-rhel-9-crash-course/0636920077845/0790145072881/"
type: lecture
updated_date: 2024-04-08
---

# 📚 RHCSA Bootcamp Day 1

- **🏷️Tags** : \#04-2024 \#lecture
  \## Other days
- [RHCSA Bootcamp Day 2](RHCSA Bootcamp Day 2 "wikilink")
- [RHCSA Bootcamp Day 3](RHCSA Bootcamp Day 3 "wikilink")
- [RHCSA Bootcamp Day 4](RHCSA Bootcamp Day 4 "wikilink")
  \## Slides
  ![](rhcsa911711116394427.pdf "wikilink")

## Templates

#### moduleName

##### Commands

``` bash
#commands

```

##### Output

``` bash
#output
```

## 📝 Notes

### Getting Started

- Setup two VMs
  - [rhel9-01](rhel9-01 "wikilink") - This is my primary VM for learning
  - [rhcsa-student01](rhcsa-student01 "wikilink") - Used from the start of todays course following Sander's instructions.
    \#### Tasks
    \##### Task 1
    Use tar to create a gzipped archive that contains the contents of the /etc directory as relative file names, and write the archive to /root/archive.tgz

``` bash
#command
tar czvf /root/archive.tgz -C / etc
```

Let's break down the options used in the command:

- `c`: Create a new archive.
- `z`: Compress the archive using gzip.
- `v`: Verbose mode, which displays the filenames as they are archived.
- `f`: Use the archive file specified as the next argument (`/root/archive.tgz` in this case).
- `-C /`: This option changes to the root directory (`/`) before performing any operations. This ensures that the paths stored in the archive are relative to the root directory.
  \###### Output

``` bash
#output
[student@rhel9-01 rhcsa]$ sudo tar czvf /root/archive.tgz -C / etc
[sudo] password for student:
etc/
etc/mtab
etc/fstab
etc/crypttab
etc/lvm/
etc/lvm/devices/
etc/lvm/devices/system.devices
etc/lvm/archive/
etc/lvm/archive/rhel_00000-1391670426.vg
etc/lvm/backup/
etc/lvm/backup/rhel
etc/lvm/cache/
etc/lvm/lvm.conf
etc/lvm/lvmlocal.conf
etc/lvm/profile/
etc/lvm/profile/cache-mq.profile
etc/lvm/profile/cache-smq.profile
etc/lvm/profile/command_profile_template.profile
etc/lvm/profile/lvmdbusd.profile
etc/lvm/profile/metadata_profile_template.profile
etc/lvm/profile/thin-generic.profile
etc/lvm/profile/thin-performance.profile
etc/lvm/profile/vdo-small.profile
etc/resolv.conf
etc/dnf/
etc/dnf/modules.d/
etc/dnf/aliases.d/
etc/dnf/dnf.conf
etc/dnf/modules.defaults.d/
etc/dnf/plugins/
etc/dnf/plugins/copr.conf
etc/dnf/plugins/copr.d/
etc/dnf/plugins/debuginfo-install.conf
etc/dnf/plugins/kpatch.conf
etc/dnf/plugins/product-id.conf
etc/dnf/plugins/subscription-manager.conf
etc/dnf/protected.d/
etc/dnf/protected.d/dnf.conf
etc/dnf/protected.d/redhat-release.conf
etc/dnf/protected.d/setup.conf
etc/dnf/protected.d/systemd.conf
etc/dnf/protected.d/grub2-tools-minimal.conf
etc/dnf/protected.d/sudo.conf
etc/dnf/protected.d/yum.conf
etc/dnf/protected.d/grub2-pc.conf
etc/dnf/vars/
etc/fonts/
etc/fonts/conf.d/
etc/fonts/conf.d/31-cantarell.conf
etc/fonts/conf.d/65-0-google-noto-sans-cjk-ttc.conf
etc/fonts/conf.d/65-google-noto-cjk-fonts.conf
etc/fonts/conf.d/65-1-lohit-devanagari.conf
etc/fonts/conf.d/59-liberation-mono.conf
etc/fonts/conf.d/65-0-google-noto-serif-cjk-ttc.conf
etc/fonts/conf.d/61-adobe-source-code-pro.conf
etc/fonts/conf.d/65-0-jomolhari-fonts.conf
etc/fonts/conf.d/20-unhint-small-dejavu-sans-mono.conf
etc/fonts/conf.d/65-google-noto-sans-gurmukhi.conf
etc/fonts/conf.d/57-dejavu-sans-mono-fonts.conf
etc/fonts/conf.d/65-google-noto-sans-sinhala-vf.conf
etc/fonts/conf.d/20-unhint-small-dejavu-sans.conf
etc/fonts/conf.d/65-0-lohit-gujarati.conf
etc/fonts/conf.d/57-dejavu-sans-fonts.conf
etc/fonts/conf.d/61-julietaula-montserrat.conf
etc/fonts/conf.d/65-google-droid-sans-fonts.conf
etc/fonts/conf.d/65-0-khmer-os-system-fonts.conf
etc/fonts/conf.d/61-urw-fallback-backwards.conf
etc/fonts/conf.d/65-0-lohit-kannada.conf
etc/fonts/conf.d/10-hinting-slight.conf
etc/fonts/conf.d/30-lohit-odia.conf
etc/fonts/conf.d/10-scale-bitmap-fonts.conf
etc/fonts/conf.d/65-0-lohit-odia.conf
etc/fonts/conf.d/11-lcdfilter-default.conf
etc/fonts/conf.d/65-0-lohit-tamil.conf
etc/fonts/conf.d/20-unhint-small-vera.conf
etc/fonts/conf.d/65-0-lohit-telugu.conf
etc/fonts/conf.d/25-no-bitmap-fedora.conf
etc/fonts/conf.d/65-0-paktype-naskh-basic.conf
etc/fonts/conf.d/25-unhint-nonlatin.conf
etc/fonts/conf.d/58-pt-sans-fonts.conf
etc/fonts/conf.d/30-metric-aliases.conf
etc/fonts/conf.d/40-nonlatin.conf
etc/fonts/conf.d/45-generic.conf
etc/fonts/conf.d/45-latin.conf
etc/fonts/conf.d/48-spacing.conf
etc/fonts/conf.d/49-sansserif.conf
etc/fonts/conf.d/50-user.conf
etc/fonts/conf.d/51-local.conf
etc/fonts/conf.d/60-generic.conf
etc/fonts/conf.d/60-latin.conf
etc/fonts/conf.d/66-sil-abyssinica-fonts.conf
etc/fonts/conf.d/65-fonts-persian.conf
etc/fonts/conf.d/65-nonlatin.conf
etc/fonts/conf.d/69-unifont.conf
etc/fonts/conf.d/80-delicious.conf
etc/fonts/conf.d/90-synthetic.conf
etc/fonts/conf.d/README
etc/fonts/conf.d/61-urw-bookman.conf
etc/fonts/conf.d/61-urw-c059.conf
etc/fonts/conf.d/66-sil-nuosu.conf
etc/fonts/conf.d/61-urw-d050000l.conf
etc/fonts/conf.d/61-urw-gothic.conf
etc/fonts/conf.d/65-sil-padauk.conf
etc/fonts/conf.d/61-urw-nimbus-mono-ps.conf
etc/fonts/conf.d/65-0-smc-meera.conf
etc/fonts/conf.d/61-urw-nimbus-roman.conf
etc/fonts/conf.d/65-stix-fonts.conf
etc/fonts/conf.d/61-urw-nimbus-sans.conf
etc/fonts/conf.d/61-urw-p052.conf
etc/fonts/conf.d/65-0-lohit-assamese.conf
etc/fonts/conf.d/61-urw-standard-symbols-ps.conf
etc/fonts/conf.d/61-urw-z003.conf
etc/fonts/conf.d/65-0-lohit-bengali.conf
etc/fonts/conf.d/65-0-thai-scalable-waree.conf
etc/fonts/conf.d/59-liberation-sans.conf
etc/fonts/conf.d/59-liberation-serif.conf
etc/fonts/conf.d/59-lohit-devanagari.conf
etc/fonts/conf.d/20-unhint-small-dejavu-serif.conf
etc/fonts/conf.d/57-dejavu-serif-fonts.conf
etc/fonts/fonts.conf
etc/crypto-policies/
etc/crypto-policies/back-ends/
etc/crypto-policies/back-ends/bind.config
etc/crypto-policies/back-ends/gnutls.config
etc/crypto-policies/back-ends/java.config
etc/crypto-policies/back-ends/javasystem.config
etc/crypto-policies/back-ends/krb5.config
etc/crypto-policies/back-ends/libreswan.config
etc/crypto-policies/back-ends/libssh.config
etc/crypto-policies/back-ends/nss.config
etc/crypto-policies/back-ends/openssh.config
etc/crypto-policies/back-ends/opensshserver.config
etc/crypto-policies/back-ends/openssl.config
etc/crypto-policies/back-ends/openssl_fips.config
etc/crypto-policies/back-ends/opensslcnf.config
etc/crypto-policies/local.d/
etc/crypto-policies/local.d/nss-p11-kit.config
etc/crypto-policies/policies/
etc/crypto-policies/policies/modules/
etc/crypto-policies/state/
etc/crypto-policies/state/current
etc/crypto-policies/state/CURRENT.pol
etc/crypto-policies/config
etc/skel/
etc/skel/.mozilla/
etc/skel/.mozilla/extensions/
etc/skel/.mozilla/plugins/
etc/skel/.bash_logout
etc/skel/.bash_profile
etc/skel/.bashrc
etc/rhsm/
etc/rhsm/ca/
etc/rhsm/ca/redhat-entitlement-authority.pem
etc/rhsm/ca/redhat-uep.pem
etc/rhsm/facts/
etc/rhsm/pluginconf.d/
etc/rhsm/rhsm.conf
etc/rhsm/syspurpose/
etc/rhsm/syspurpose/valid_fields.json
etc/rhsm/syspurpose/syspurpose.json
etc/libreport/
etc/libreport/events/
etc/libreport/events.d/
etc/libreport/events.d/collect_dnf.conf
etc/libreport/events.d/mdadm_event.conf
etc/libreport/plugins/
etc/libreport/workflows.d/
etc/gnupg/
etc/fuse.conf
etc/logrotate.d/
etc/logrotate.d/dnf
etc/logrotate.d/btmp
etc/logrotate.d/wtmp
etc/logrotate.d/samba
etc/logrotate.d/iscsiuiolog
etc/logrotate.d/rsyslog
etc/logrotate.d/wpa_supplicant
etc/logrotate.d/sssd
etc/logrotate.d/bootlog
etc/logrotate.d/kvm_stat
etc/logrotate.d/insights-client
etc/logrotate.d/subscription-manager
etc/logrotate.d/firewalld
etc/logrotate.d/chrony
etc/logrotate.d/psacct
etc/X11/
etc/X11/fontpath.d/
etc/X11/fontpath.d/liberation-mono-fonts
etc/X11/fontpath.d/liberation-sans-fonts
etc/X11/fontpath.d/liberation-serif-fonts
etc/X11/applnk/
etc/X11/xinit/
etc/X11/xinit/xinitrc.d/
etc/X11/xinit/xinitrc.d/localuser.sh
etc/X11/xinit/xinitrc.d/50-systemd-user.sh
etc/X11/xinit/xinput.d/
etc/X11/xinit/xinput.d/ibus.conf
etc/X11/xinit/Xclients
etc/X11/xinit/Xclients.d/
etc/X11/xinit/Xsession
etc/X11/xinit/xinitrc
etc/X11/xinit/xinitrc-common
etc/X11/xinit/xinputrc
etc/X11/Xmodmap
etc/X11/Xresources
etc/X11/xorg.conf.d/
etc/X11/xorg.conf.d/00-keyboard.conf
etc/X11/Xsession.d/
etc/X11/Xsession.d/90xbrlapi
etc/bash_completion.d/
etc/bash_completion.d/tracer
etc/bash_completion.d/authselect-completion.sh
etc/bash_completion.d/vdostats
etc/bash_completion.d/redefine_filedir
etc/bash_completion.d/bpftool
etc/bash_completion.d/iprconfig
etc/hp/
etc/hp/hplip.conf
etc/pki/
etc/pki/swid/
etc/pki/swid/CA/
etc/pki/swid/CA/redhat.com/
etc/pki/swid/CA/redhat.com/redhatcodesignca.cert
etc/pki/product-default/
etc/pki/product-default/479.pem
etc/pki/rpm-gpg/
etc/pki/rpm-gpg/RPM-GPG-KEY-redhat-beta
etc/pki/rpm-gpg/RPM-GPG-KEY-redhat-release
etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-9
etc/pki/tls/
etc/pki/tls/certs/
etc/pki/tls/certs/ca-bundle.crt
etc/pki/tls/certs/ca-bundle.trust.crt
etc/pki/tls/ct_log_list.cnf
etc/pki/tls/fips_local.cnf
etc/pki/tls/misc/
etc/pki/tls/openssl.cnf
etc/pki/tls/private/
etc/pki/tls/cert.pem
etc/pki/ca-trust/
etc/pki/ca-trust/extracted/
etc/pki/ca-trust/extracted/edk2/
etc/pki/ca-trust/extracted/edk2/README
etc/pki/ca-trust/extracted/edk2/cacerts.bin
etc/pki/ca-trust/extracted/README
etc/pki/ca-trust/extracted/java/
etc/pki/ca-trust/extracted/java/README
etc/pki/ca-trust/extracted/java/cacerts
etc/pki/ca-trust/extracted/openssl/
etc/pki/ca-trust/extracted/openssl/README
etc/pki/ca-trust/extracted/openssl/ca-bundle.trust.crt
etc/pki/ca-trust/extracted/pem/
etc/pki/ca-trust/extracted/pem/README
etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem
etc/pki/ca-trust/extracted/pem/email-ca-bundle.pem
etc/pki/ca-trust/extracted/pem/objsign-ca-bundle.pem
etc/pki/ca-trust/README
etc/pki/ca-trust/ca-legacy.conf
etc/pki/ca-trust/source/
etc/pki/ca-trust/source/README
etc/pki/ca-trust/source/anchors/
etc/pki/ca-trust/source/blocklist/
etc/pki/ca-trust/source/ca-bundle.legacy.crt
etc/pki/java/
etc/pki/java/cacerts
etc/pki/rsyslog/
etc/pki/nssdb/
etc/pki/nssdb/cert9.db
etc/pki/nssdb/key4.db
etc/pki/nssdb/pkcs11.txt
etc/pki/fwupd/
etc/pki/fwupd/GPG-KEY-Linux-Foundation-Firmware
etc/pki/fwupd/GPG-KEY-Linux-Vendor-Firmware-Service
etc/pki/fwupd/LVFS-CA.pem
etc/pki/fwupd-metadata/
etc/pki/fwupd-metadata/GPG-KEY-Linux-Foundation-Metadata
etc/pki/fwupd-metadata/GPG-KEY-Linux-Vendor-Firmware-Service
etc/pki/fwupd-metadata/LVFS-CA.pem
etc/pki/consumer/
etc/pki/consumer/key.pem
etc/pki/consumer/cert.pem
etc/pki/entitlement/
etc/pki/entitlement/7516372115803665970-key.pem
etc/pki/entitlement/7516372115803665970.pem
etc/pki/product/
etc/swid/
etc/swid/swidtags.d/
etc/swid/swidtags.d/redhat.com
etc/ostree/
etc/ostree/remotes.d/
etc/issue
etc/issue.d/
etc/issue.d/cockpit.issue
etc/rpm/
etc/udev/
etc/udev/hwdb.d/
etc/udev/rules.d/
etc/udev/udev.conf
etc/udev/hwdb.bin
etc/issue.net
etc/appstream.conf
etc/os-release
etc/libibverbs.d/
etc/libibverbs.d/bnxt_re.driver
etc/libibverbs.d/cxgb4.driver
etc/libibverbs.d/efa.driver
etc/libibverbs.d/hfi1verbs.driver
etc/libibverbs.d/hns.driver
etc/libibverbs.d/irdma.driver
etc/libibverbs.d/mana.driver
etc/libibverbs.d/mlx4.driver
etc/libibverbs.d/mlx5.driver
etc/libibverbs.d/qedr.driver
etc/libibverbs.d/rxe.driver
etc/libibverbs.d/siw.driver
etc/libibverbs.d/vmw_pvrdma.driver
etc/sssd/
etc/sssd/conf.d/
etc/sssd/pki/
etc/redhat-release
etc/gshadow-
etc/lsm/
etc/lsm/pluginconf.d/
etc/lsm/pluginconf.d/sim.conf
etc/lsm/lsmd.conf
etc/system-release
etc/group-
etc/cups/
etc/cups/cups-browsed.conf
etc/cups/classes.conf
etc/cups/client.conf
etc/cups/cups-files.conf
etc/cups/cups-files.conf.default
etc/cups/cupsd.conf
etc/cups/cupsd.conf.default
etc/cups/lpoptions
etc/cups/ppd/
etc/cups/printers.conf
etc/cups/snmp.conf
etc/cups/snmp.conf.default
etc/cups/ssl/
etc/cups/subscriptions.conf.O
etc/cups/subscriptions.conf
etc/system-release-cpe
etc/yum.repos.d/
etc/yum.repos.d/redhat.repo
etc/yum.repos.d/epel-cisco-openh264.repo
etc/yum.repos.d/epel-testing.repo
etc/yum.repos.d/epel.repo
etc/yum.repos.d/gh-cli.repo
etc/sane.d/
etc/sane.d/pieusb.conf
etc/sane.d/airscan.conf
etc/sane.d/dll.d/
etc/sane.d/dll.d/airscan
etc/sane.d/dll.d/hpaio
etc/sane.d/abaton.conf
etc/sane.d/pixma.conf
etc/sane.d/agfafocus.conf
etc/sane.d/apple.conf
etc/sane.d/artec.conf
etc/sane.d/plustek_pp.conf
etc/sane.d/artec_eplus48u.conf
etc/sane.d/plustek.conf
etc/sane.d/avision.conf
etc/sane.d/bh.conf
etc/sane.d/canon.conf
etc/sane.d/qcam.conf
etc/sane.d/canon630u.conf
etc/sane.d/ricoh.conf
etc/sane.d/canon_dr.conf
etc/sane.d/rts8891.conf
etc/sane.d/canon_lide70.conf
etc/sane.d/teco1.conf
etc/sane.d/canon_pp.conf
etc/sane.d/tamarack.conf
etc/sane.d/cardscan.conf
etc/sane.d/teco2.conf
etc/sane.d/coolscan.conf
etc/sane.d/teco3.conf
etc/sane.d/coolscan2.conf
etc/sane.d/test.conf
etc/sane.d/coolscan3.conf
etc/sane.d/dc210.conf
etc/sane.d/dc240.conf
etc/sane.d/dc25.conf
etc/sane.d/u12.conf
etc/sane.d/dell1600n_net.conf
etc/sane.d/dll.conf
etc/sane.d/dmc.conf
etc/sane.d/umax.conf
etc/sane.d/epjitsu.conf
etc/sane.d/epson.conf
etc/sane.d/epson2.conf
etc/sane.d/umax1220u.conf
etc/sane.d/epsonds.conf
etc/sane.d/umax_pp.conf
etc/sane.d/fujitsu.conf
etc/sane.d/v4l.conf
etc/sane.d/genesys.conf
etc/sane.d/xerox_mfp.conf
etc/sane.d/gphoto2.conf
etc/sane.d/gt68xx.conf
etc/sane.d/hp.conf
etc/sane.d/hp3900.conf
etc/sane.d/hp4200.conf
etc/sane.d/hp5400.conf
etc/sane.d/hpsj5s.conf
etc/sane.d/hs2p.conf
etc/sane.d/ibm.conf
etc/sane.d/kodak.conf
etc/sane.d/kodakaio.conf
etc/sane.d/kvs1025.conf
etc/sane.d/leo.conf
etc/sane.d/lexmark.conf
etc/sane.d/ma1509.conf
etc/sane.d/magicolor.conf
etc/sane.d/matsushita.conf
etc/sane.d/microtek.conf
etc/sane.d/microtek2.conf
etc/sane.d/mustek.conf
etc/sane.d/mustek_pp.conf
etc/sane.d/mustek_usb.conf
etc/sane.d/nec.conf
etc/sane.d/net.conf
etc/sane.d/p5.conf
etc/sane.d/pie.conf
etc/sane.d/s9036.conf
etc/sane.d/saned.conf
etc/sane.d/sceptre.conf
etc/sane.d/sharp.conf
etc/sane.d/sm3840.conf
etc/sane.d/snapscan.conf
etc/sane.d/sp15c.conf
etc/sane.d/st400.conf
etc/sane.d/stv680.conf
etc/aliases
etc/security/
etc/security/pwquality.conf
etc/security/pwquality.conf.d/
etc/security/access.conf
etc/security/chroot.conf
etc/security/console.apps/
etc/security/console.apps/config-util
etc/security/console.apps/subscription-manager
etc/security/console.handlers
etc/security/console.perms
etc/security/console.perms.d/
etc/security/faillock.conf
etc/security/group.conf
etc/security/limits.conf
etc/security/limits.d/
etc/security/limits.d/25-pw-rlimits.conf
etc/security/namespace.conf
etc/security/namespace.d/
etc/security/namespace.init
etc/security/opasswd
etc/security/pam_env.conf
etc/security/pwhistory.conf
etc/security/sepermit.conf
etc/security/time.conf
etc/bashrc
etc/pam.d/
etc/pam.d/config-util
etc/pam.d/other
etc/pam.d/login
etc/pam.d/remote
etc/pam.d/runuser
etc/pam.d/runuser-l
etc/pam.d/su
etc/pam.d/su-l
etc/pam.d/systemd-user
etc/pam.d/polkit-1
etc/pam.d/crond
etc/pam.d/passwd
etc/pam.d/vlock
etc/pam.d/sssd-shadowutils
etc/pam.d/sudo
etc/pam.d/sudo-i
etc/pam.d/xserver
etc/pam.d/cups
etc/pam.d/subscription-manager
etc/pam.d/gdm-autologin
etc/pam.d/gdm-fingerprint
etc/pam.d/gdm-launch-environment
etc/pam.d/gdm-password
etc/pam.d/gdm-pin
etc/pam.d/gdm-smartcard
etc/pam.d/cockpit
etc/pam.d/vmtoolsd
etc/pam.d/sshd
etc/pam.d/chfn
etc/pam.d/chsh
etc/pam.d/atd
etc/pam.d/system-auth
etc/pam.d/password-auth
etc/pam.d/fingerprint-auth
etc/pam.d/smartcard-auth
etc/pam.d/postlogin
etc/csh.cshrc
etc/passwd-
etc/csh.login
etc/shadow-
etc/environment
etc/tpm2-tss/
etc/tpm2-tss/fapi-config.json
etc/tpm2-tss/fapi-profiles/
etc/tpm2-tss/fapi-profiles/P_ECCP256SHA256.json
etc/tpm2-tss/fapi-profiles/P_RSA2048SHA256.json
etc/ethertypes
etc/inittab
etc/exports
etc/adjtime
etc/filesystems
etc/rc.d/
etc/rc.d/init.d/
etc/rc.d/init.d/README
etc/rc.d/rc.local
etc/cni/
etc/group
etc/tmpfiles.d/
etc/tmpfiles.d/sos.conf
etc/gshadow
etc/rc.local
etc/host.conf
etc/systemd/
etc/systemd/journald.conf
etc/systemd/logind.conf
etc/systemd/system/
etc/systemd/system/sysinit.target.wants/
etc/systemd/system/sysinit.target.wants/nis-domainname.service
etc/systemd/system/sysinit.target.wants/systemd-network-generator.service
etc/systemd/system/sysinit.target.wants/selinux-autorelabel-mark.service
etc/systemd/system/sysinit.target.wants/iscsi-onboot.service
etc/systemd/system/sysinit.target.wants/lvm2-monitor.service
etc/systemd/system/sysinit.target.wants/lvm2-lvmpolld.socket
etc/systemd/system/sysinit.target.wants/multipathd.service
etc/systemd/system/sysinit.target.wants/systemd-boot-update.service
etc/systemd/system/ctrl-alt-del.target
etc/systemd/system/multi-user.target.wants/
etc/systemd/system/multi-user.target.wants/remote-fs.target
etc/systemd/system/multi-user.target.wants/avahi-daemon.service
etc/systemd/system/multi-user.target.wants/crond.service
etc/systemd/system/multi-user.target.wants/auditd.service
etc/systemd/system/multi-user.target.wants/rsyslog.service
etc/systemd/system/multi-user.target.wants/mdmonitor.service
etc/systemd/system/multi-user.target.wants/NetworkManager.service
etc/systemd/system/multi-user.target.wants/sssd.service
etc/systemd/system/multi-user.target.wants/ModemManager.service
etc/systemd/system/multi-user.target.wants/kdump.service
etc/systemd/system/multi-user.target.wants/libstoragemgmt.service
etc/systemd/system/multi-user.target.wants/cups.path
etc/systemd/system/multi-user.target.wants/cups.service
etc/systemd/system/multi-user.target.wants/insights-client-boot.service
etc/systemd/system/multi-user.target.wants/rhsmcertd.service
etc/systemd/system/multi-user.target.wants/vmtoolsd.service
etc/systemd/system/multi-user.target.wants/firewalld.service
etc/systemd/system/multi-user.target.wants/tuned.service
etc/systemd/system/multi-user.target.wants/sshd.service
etc/systemd/system/multi-user.target.wants/atd.service
etc/systemd/system/multi-user.target.wants/chronyd.service
etc/systemd/system/multi-user.target.wants/mcelog.service
etc/systemd/system/multi-user.target.wants/smartd.service
etc/systemd/system/multi-user.target.wants/irqbalance.service
etc/systemd/system/getty.target.wants/
etc/systemd/system/getty.target.wants/getty@tty1.service
etc/systemd/system/sockets.target.wants/
etc/systemd/system/sockets.target.wants/dbus.socket
etc/systemd/system/sockets.target.wants/avahi-daemon.socket
etc/systemd/system/sockets.target.wants/iscsiuio.socket
etc/systemd/system/sockets.target.wants/iscsid.socket
etc/systemd/system/sockets.target.wants/dm-event.socket
etc/systemd/system/sockets.target.wants/multipathd.socket
etc/systemd/system/sockets.target.wants/cups.socket
etc/systemd/system/sockets.target.wants/sssd-kcm.socket
etc/systemd/system/dbus.service
etc/systemd/system/dbus-org.freedesktop.Avahi.service
etc/systemd/system/graphical.target.wants/
etc/systemd/system/graphical.target.wants/accounts-daemon.service
etc/systemd/system/graphical.target.wants/rtkit-daemon.service
etc/systemd/system/graphical.target.wants/upower.service
etc/systemd/system/graphical.target.wants/switcheroo-control.service
etc/systemd/system/graphical.target.wants/udisks2.service
etc/systemd/system/graphical.target.wants/power-profiles-daemon.service
etc/systemd/system/dbus-org.bluez.service
etc/systemd/system/bluetooth.target.wants/
etc/systemd/system/bluetooth.target.wants/bluetooth.service
etc/systemd/system/timers.target.wants/
etc/systemd/system/timers.target.wants/logrotate.timer
etc/systemd/system/timers.target.wants/dnf-makecache.timer
etc/systemd/system/timers.target.wants/mlocate-updatedb.timer
etc/systemd/system/remote-fs.target.wants/
etc/systemd/system/remote-fs.target.wants/iscsi.service
etc/systemd/system/dbus-org.freedesktop.nm-dispatcher.service
etc/systemd/system/network-online.target.wants/
etc/systemd/system/network-online.target.wants/NetworkManager-wait-online.service
etc/systemd/system/dbus-org.freedesktop.ModemManager1.service
etc/systemd/system/basic.target.wants/
etc/systemd/system/basic.target.wants/low-memory-monitor.service
etc/systemd/system/basic.target.wants/microcode.service
etc/systemd/system/local-fs.target.wants/
etc/systemd/system/local-fs.target.wants/ostree-remount.service
etc/systemd/system/printer.target.wants/
etc/systemd/system/printer.target.wants/cups.service
etc/systemd/system/display-manager.service
etc/systemd/system/vmtoolsd.service.requires/
etc/systemd/system/vmtoolsd.service.requires/vgauthd.service
etc/systemd/system/default.target.wants/
etc/systemd/system/default.target.wants/nvmefc-boot-connections.service
etc/systemd/system/dbus-org.fedoraproject.FirewallD1.service
etc/systemd/system/dev-virtio\\x2dports-org.qemu.guest_agent.0.device.wants/
etc/systemd/system/dev-virtio\\x2dports-org.qemu.guest_agent.0.device.wants/qemu-guest-agent.service
etc/systemd/system/default.target
etc/systemd/system.conf
etc/systemd/user/
etc/systemd/user/timers.target.wants/
etc/systemd/user/timers.target.wants/systemd-tmpfiles-clean.timer
etc/systemd/user/basic.target.wants/
etc/systemd/user/basic.target.wants/systemd-tmpfiles-setup.service
etc/systemd/user/sockets.target.wants/
etc/systemd/user/sockets.target.wants/dbus.socket
etc/systemd/user/sockets.target.wants/pipewire.socket
etc/systemd/user/sockets.target.wants/pipewire-pulse.socket
etc/systemd/user/dbus.service
etc/systemd/user/dbus-org.bluez.obex.service
etc/systemd/user/pipewire-session-manager.service
etc/systemd/user/pipewire.service.wants/
etc/systemd/user/pipewire.service.wants/wireplumber.service
etc/systemd/user.conf
etc/systemd/coredump.conf
etc/systemd/pstore.conf
etc/systemd/sleep.conf
etc/hosts
etc/machine-id
etc/inputrc
etc/dbus-1/
etc/dbus-1/session.conf
etc/dbus-1/session.d/
etc/dbus-1/system.conf
etc/dbus-1/system.d/
etc/dbus-1/system.d/org.freedesktop.PolicyKit1.conf
etc/dbus-1/system.d/avahi-dbus.conf
etc/dbus-1/system.d/org.freedesktop.Accounts.conf
etc/dbus-1/system.d/bluetooth.conf
etc/dbus-1/system.d/org.freedesktop.RealtimeKit1.conf
etc/dbus-1/system.d/wpa_supplicant.conf
etc/dbus-1/system.d/net.hadess.SensorProxy.conf
etc/dbus-1/system.d/org.opensuse.CupsPkHelper.Mechanism.conf
etc/dbus-1/system.d/org.freedesktop.GeoClue2.Agent.conf
etc/dbus-1/system.d/org.freedesktop.GeoClue2.conf
etc/dbus-1/system.d/org.freedesktop.ModemManager1.conf
etc/dbus-1/system.d/org.freedesktop.PackageKit.conf
etc/dbus-1/system.d/net.hadess.SwitcherooControl.conf
etc/dbus-1/system.d/org.selinux.conf
etc/dbus-1/system.d/org.freedesktop.Flatpak.SystemHelper.conf
etc/dbus-1/system.d/org.fedoraproject.SetroubleshootFixit.conf
etc/dbus-1/system.d/org.fedoraproject.SetroubleshootPrivileged.conf
etc/dbus-1/system.d/org.fedoraproject.Setroubleshootd.conf
etc/dbus-1/system.d/cups.conf
etc/dbus-1/system.d/com.redhat.RHSM1.Facts.conf
etc/dbus-1/system.d/com.redhat.RHSM1.conf
etc/dbus-1/system.d/teamd.conf
etc/dbus-1/system.d/net.hadess.PowerProfiles.conf
etc/dbus-1/system.d/com.redhat.NewPrinterNotification.conf
etc/dbus-1/system.d/com.redhat.PrinterDriversInstaller.conf
etc/dbus-1/system.d/gdm.conf
etc/dbus-1/system.d/org.freedesktop.realmd.conf
etc/dbus-1/system.d/dnsmasq.conf
etc/motd
etc/motd.d/
etc/motd.d/insights-client
etc/motd.d/cockpit
etc/dconf/
etc/dconf/db/
etc/dconf/db/distro.d/
etc/dconf/db/distro.d/locks/
etc/dconf/db/distro.d/locks/20-authselect
etc/dconf/db/distro.d/20-authselect
etc/dconf/db/local.d/
etc/dconf/db/local.d/locks/
etc/dconf/db/site.d/
etc/dconf/db/site.d/locks/
etc/dconf/db/ibus.d/
etc/dconf/db/ibus.d/00-upstream-settings
etc/dconf/db/gdm.d/
etc/dconf/db/gdm.d/locks/
etc/dconf/db/distro
etc/dconf/db/local
etc/dconf/db/site
etc/dconf/db/ibus
etc/dconf/db/gdm
etc/dconf/profile/
etc/dconf/profile/user
etc/dconf/profile/ibus
etc/networks
etc/sestatus.conf
etc/passwd
etc/accountsservice/
etc/accountsservice/user-templates/
etc/printcap
etc/bluetooth/
etc/bluetooth/main.conf
etc/profile
etc/profile.d/
etc/profile.d/csh.local
etc/profile.d/lang.csh
etc/profile.d/lang.sh
etc/profile.d/sh.local
etc/profile.d/which2.csh
etc/profile.d/which2.sh
etc/profile.d/gawk.csh
etc/profile.d/gawk.sh
etc/profile.d/colorgrep.csh
etc/profile.d/colorgrep.sh
etc/profile.d/colorxzgrep.csh
etc/profile.d/colorxzgrep.sh
etc/profile.d/less.csh
etc/profile.d/less.sh
etc/profile.d/vte.csh
etc/profile.d/vte.sh
etc/profile.d/colorls.csh
etc/profile.d/colorls.sh
etc/profile.d/colorzgrep.csh
etc/profile.d/colorzgrep.sh
etc/profile.d/debuginfod.csh
etc/profile.d/debuginfod.sh
etc/profile.d/flatpak.sh
etc/profile.d/PackageKit.sh
etc/profile.d/bash_completion.sh
etc/logrotate.conf
etc/protocols
etc/polkit-1/
etc/polkit-1/rules.d/
etc/polkit-1/rules.d/50-default.rules
etc/polkit-1/rules.d/49-polkit-pkla-compat.rules
etc/polkit-1/localauthority/
etc/polkit-1/localauthority/10-vendor.d/
etc/polkit-1/localauthority/20-org.d/
etc/polkit-1/localauthority/30-site.d/
etc/polkit-1/localauthority/50-local.d/
etc/polkit-1/localauthority/90-mandatory.d/
etc/polkit-1/localauthority.conf.d/
etc/services
etc/libuser.conf
etc/shadow
etc/avahi/
etc/avahi/avahi-daemon.conf
etc/avahi/etc/
etc/avahi/hosts
etc/avahi/services/
etc/shells
etc/samba/
etc/samba/lmhosts
etc/samba/smb.conf
etc/samba/smb.conf.example
etc/subgid
etc/grub.d/
etc/grub.d/00_header
etc/grub.d/01_users
etc/grub.d/08_fallback_counting
etc/grub.d/10_linux
etc/grub.d/10_reset_boot_success
etc/grub.d/12_menu_auto_hide
etc/grub.d/14_menu_show_once
etc/grub.d/20_linux_xen
etc/grub.d/20_ppc_terminfo
etc/grub.d/30_os-prober
etc/grub.d/30_uefi-firmware
etc/grub.d/40_custom
etc/grub.d/41_custom
etc/grub.d/README
etc/grub.d/35_fwupd
etc/grub.d/00_tuned
etc/subuid
etc/opt/
etc/opt/chrome/
etc/opt/chrome/native-messaging-hosts/
etc/opt/chrome/native-messaging-hosts/org.gnome.browser_connector.json
etc/opt/chrome/native-messaging-hosts/org.gnome.chrome_gnome_shell.json
etc/pm/
etc/pm/config.d/
etc/pm/power.d/
etc/pm/sleep.d/
etc/rwtab.d/
etc/rwtab.d/logrotate
etc/rwtab.d/sssd
etc/statetab.d/
etc/sysconfig/
etc/sysconfig/nftables.conf
etc/sysconfig/selinux
etc/sysconfig/samba
etc/sysconfig/crond
etc/sysconfig/run-parts
etc/sysconfig/rsyslog
etc/sysconfig/raid-check
etc/sysconfig/wpa_supplicant
etc/sysconfig/network-scripts/
etc/sysconfig/network-scripts/readme-ifcfg-rh.txt
etc/sysconfig/kdump
etc/sysconfig/cpupower
etc/sysconfig/rasdaemon
etc/sysconfig/firewalld
etc/sysconfig/sshd
etc/sysconfig/atd
etc/sysconfig/chronyd
etc/sysconfig/smartmontools
etc/sysconfig/man-db
etc/sysconfig/irqbalance
etc/sysconfig/kernel
etc/sysconfig/anaconda
etc/sysconfig/network
etc/sysconfig/qemu-ga
etc/xdg/
etc/xdg/autostart/
etc/xdg/autostart/xdg-user-dirs.desktop
etc/xdg/autostart/at-spi-dbus-bus.desktop
etc/xdg/autostart/geoclue-demo-agent.desktop
etc/xdg/autostart/tracker-miner-fs-3.desktop
etc/xdg/autostart/gnome-software-service.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.A11ySettings.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Color.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Datetime.desktop
etc/xdg/autostart/spice-vdagent.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Housekeeping.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Keyboard.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.MediaKeys.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Power.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.DiskUtilityNotify.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.PrintNotifications.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Rfkill.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.ScreensaverProxy.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Sharing.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Smartcard.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Sound.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Subscription.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.UsbProtection.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Wacom.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.Wwan.desktop
etc/xdg/autostart/org.gnome.SettingsDaemon.XSettings.desktop
etc/xdg/autostart/gnome-keyring-pkcs11.desktop
etc/xdg/autostart/gnome-keyring-secrets.desktop
etc/xdg/autostart/gnome-keyring-ssh.desktop
etc/xdg/autostart/user-dirs-update-gtk.desktop
etc/xdg/autostart/org.gnome.Evolution-alarm-notify.desktop
etc/xdg/autostart/gnome-shell-overrides-migration.desktop
etc/xdg/autostart/vmware-user.desktop
etc/xdg/autostart/gnome-initial-setup-copy-worker.desktop
etc/xdg/autostart/gnome-initial-setup-first-login.desktop
etc/xdg/autostart/orca-autostart.desktop
etc/xdg/user-dirs.conf
etc/xdg/user-dirs.defaults
etc/xdg/menus/
etc/xdg/menus/applications.menu
etc/xdg/menus/gnome-applications.menu
etc/xdg/systemd/
etc/xdg/systemd/user
etc/xdg/Xwayland-session.d/
etc/xdg/Xwayland-session.d/00-at-spi
etc/xdg/Xwayland-session.d/00-xrdb
etc/terminfo/
etc/cron.hourly/
etc/cron.hourly/0anacron
etc/ld.so.conf
etc/ld.so.conf.d/
etc/ld.so.conf.d/pipewire-jack-x86_64.conf
etc/libpaper.d/
etc/bindresvport.blacklist
etc/cron.monthly/
etc/rpc
etc/rsyslog.d/
etc/ld.so.cache
etc/popt.d/
etc/anacrontab
etc/asound.conf
etc/openldap/
etc/openldap/certs/
etc/openldap/ldap.conf
etc/sos/
etc/sos/cleaner/
etc/sos/extras.d/
etc/sos/groups.d/
etc/sos/presets.d/
etc/sos/sos.conf
etc/libaudit.conf
etc/alternatives/
etc/alternatives/libnssckbi.so.x86_64
etc/alternatives/soelim
etc/alternatives/soelim.1.gz
etc/alternatives/iptables
etc/alternatives/ip6tables
etc/alternatives/iptables-restore
etc/alternatives/iptables-save
etc/alternatives/ip6tables-restore
etc/alternatives/ip6tables-save
etc/alternatives/ebtables
etc/alternatives/ebtables-save
etc/alternatives/ebtables-restore
etc/alternatives/ebtables-man
etc/alternatives/arptables
etc/alternatives/arptables-save
etc/alternatives/arptables-restore
etc/alternatives/arptables-man
etc/alternatives/arptables-save-man
etc/alternatives/arptables-restore-man
etc/alternatives/arptables-helper
etc/alternatives/print
etc/alternatives/print-lp
etc/alternatives/print-lpq
etc/alternatives/print-lprm
etc/alternatives/print-lpstat
etc/alternatives/print-cancel
etc/alternatives/print-lpc
etc/alternatives/print-cancelman
etc/alternatives/print-lpman
etc/alternatives/print-lpcman
etc/alternatives/print-lpqman
etc/alternatives/print-lprman
etc/alternatives/print-lprmman
etc/alternatives/print-lpstatman
etc/alternatives/ld
etc/alternatives/cifs-idmap-plugin
etc/alternatives/xinputrc
etc/alternatives/man
etc/alternatives/apropos
etc/alternatives/whatis
etc/alternatives/man.1.gz
etc/alternatives/apropos.1.gz
etc/alternatives/whatis.1.gz
etc/alternatives/nc
etc/alternatives/nc-man
etc/alternatives/man.7.gz
etc/pkcs11/
etc/pkcs11/modules/
etc/gcrypt/
etc/libnl/
etc/libnl/classid
etc/libnl/pktloc
etc/cron.d/
etc/cron.d/0hourly
etc/xattr.conf
etc/selinux/
etc/selinux/semanage.conf
etc/selinux/config
etc/selinux/targeted/
etc/selinux/targeted/.policy.sha512
etc/selinux/targeted/booleans.subs_dist
etc/selinux/targeted/contexts/
etc/selinux/targeted/contexts/customizable_types
etc/selinux/targeted/contexts/dbus_contexts
etc/selinux/targeted/contexts/default_contexts
etc/selinux/targeted/contexts/default_type
etc/selinux/targeted/contexts/failsafe_context
etc/selinux/targeted/contexts/files/
etc/selinux/targeted/contexts/files/file_contexts
etc/selinux/targeted/contexts/files/file_contexts.homedirs
etc/selinux/targeted/contexts/files/file_contexts.local
etc/selinux/targeted/contexts/files/file_contexts.subs
etc/selinux/targeted/contexts/files/file_contexts.subs_dist
etc/selinux/targeted/contexts/files/media
etc/selinux/targeted/contexts/files/file_contexts.bin
etc/selinux/targeted/contexts/files/file_contexts.homedirs.bin
etc/selinux/targeted/contexts/initrc_context
etc/selinux/targeted/contexts/lxc_contexts
etc/selinux/targeted/contexts/openssh_contexts
etc/selinux/targeted/contexts/removable_context
etc/selinux/targeted/contexts/securetty_types
etc/selinux/targeted/contexts/sepgsql_contexts
etc/selinux/targeted/contexts/snapperd_contexts
etc/selinux/targeted/contexts/systemd_contexts
etc/selinux/targeted/contexts/userhelper_context
etc/selinux/targeted/contexts/users/
etc/selinux/targeted/contexts/users/guest_u
etc/selinux/targeted/contexts/users/root
etc/selinux/targeted/contexts/users/staff_u
etc/selinux/targeted/contexts/users/sysadm_u
etc/selinux/targeted/contexts/users/unconfined_u
etc/selinux/targeted/contexts/users/user_u
etc/selinux/targeted/contexts/users/xguest_u
etc/selinux/targeted/contexts/virtual_domain_context
etc/selinux/targeted/contexts/virtual_image_context
etc/selinux/targeted/contexts/x_contexts
etc/selinux/targeted/logins/
etc/selinux/targeted/policy/
etc/selinux/targeted/policy/policy.33
etc/selinux/targeted/setrans.conf
etc/selinux/targeted/seusers
etc/default/
etc/default/useradd
etc/default/grub
etc/cron.deny
etc/login.defs
etc/cron.daily/
etc/magic
etc/sgml/
etc/sgml/docbook/
etc/sgml/docbook/xmlcatalog
etc/xml/
etc/xml/catalog
etc/xml/mallard/
etc/xml/mallard/catalog
etc/glvnd/
etc/glvnd/egl_vendor.d/
etc/groff/
etc/groff/site-font/
etc/groff/site-tmac/
etc/groff/site-tmac/man.local
etc/groff/site-tmac/mdoc.local
etc/egl/
etc/egl/egl_external_platform.d/
etc/cron.weekly/
etc/GREP_COLORS
etc/vulkan/
etc/vulkan/explicit_layer.d/
etc/vulkan/icd.d/
etc/vulkan/implicit_layer.d/
etc/.pwd.lock
etc/ssh/
etc/ssh/moduli
etc/ssh/ssh_config
etc/ssh/ssh_config.d/
etc/ssh/ssh_config.d/50-redhat.conf
etc/ssh/sshd_config
etc/ssh/sshd_config.d/
etc/ssh/sshd_config.d/50-redhat.conf
etc/ssh/ssh_host_ed25519_key
etc/ssh/ssh_host_ed25519_key.pub
etc/ssh/ssh_host_ecdsa_key
etc/ssh/ssh_host_ecdsa_key.pub
etc/ssh/ssh_host_rsa_key
etc/ssh/ssh_host_rsa_key.pub
etc/gdm/
etc/gdm/Init/
etc/gdm/Init/Default
etc/gdm/PostLogin/
etc/gdm/PostLogin/Default.sample
etc/gdm/PostSession/
etc/gdm/PostSession/Default
etc/gdm/PreSession/
etc/gdm/PreSession/Default
etc/gdm/Xsession
etc/gdm/custom.conf
etc/papersize
etc/crontab
etc/vimrc
etc/iproute2/
etc/iproute2/bpf_pinning
etc/iproute2/ematch_map
etc/iproute2/group
etc/iproute2/nl_protos
etc/iproute2/rt_dsfield
etc/iproute2/rt_protos
etc/iproute2/rt_realms
etc/iproute2/rt_scopes
etc/iproute2/rt_tables
etc/nftables/
etc/nftables/main.nft
etc/nftables/nat.nft
etc/nftables/osf/
etc/nftables/osf/pf.os
etc/nftables/router.nft
etc/pkgconfig/
etc/pkgconfig/personality.d/
etc/libssh/
etc/libssh/libssh_client.config
etc/libssh/libssh_server.config
etc/iscsi/
etc/iscsi/iscsid.conf
etc/DIR_COLORS
etc/sasl2/
etc/libblockdev/
etc/libblockdev/conf.d/
etc/libblockdev/conf.d/00-default.cfg
etc/DIR_COLORS.lightbgcolor
etc/ssl/
etc/ssl/cert.pem
etc/ssl/certs
etc/ssl/ct_log_list.cnf
etc/ssl/openssl.cnf
etc/multipath/
etc/nsswitch.conf.bak
etc/nsswitch.conf
etc/gss/
etc/gss/mech.d/
etc/audit/
etc/audit/audit-stop.rules
etc/audit/auditd.conf
etc/audit/plugins.d/
etc/audit/plugins.d/af_unix.conf
etc/audit/plugins.d/sedispatch.conf
etc/audit/rules.d/
etc/audit/rules.d/audit.rules
etc/audit/audit.rules
etc/krb5.conf
etc/krb5.conf.d/
etc/krb5.conf.d/crypto-policies
etc/krb5.conf.d/enable_sssd_conf_dir
etc/krb5.conf.d/kcm_default_ccache
etc/pulse/
etc/pulse/client.conf
etc/depmod.d/
etc/depmod.d/dist.conf
etc/depmod.d/kvdo.conf
etc/modprobe.d/
etc/modprobe.d/firewalld-sysctls.conf
etc/modprobe.d/tuned.conf
etc/rsyslog.conf
etc/netconfig
etc/favicon.png
etc/wireplumber/
etc/wireplumber/bluetooth.lua.d/
etc/wireplumber/common/
etc/wireplumber/main.lua.d/
etc/wireplumber/policy.lua.d/
etc/authselect/
etc/authselect/custom/
etc/authselect/user-nsswitch.conf
etc/authselect/system-auth
etc/authselect/password-auth
etc/authselect/fingerprint-auth
etc/authselect/smartcard-auth
etc/authselect/postlogin
etc/authselect/nsswitch.conf
etc/authselect/dconf-db
etc/authselect/dconf-locks
etc/authselect/authselect.conf
etc/usb_modeswitch.conf
etc/wpa_supplicant/
etc/wpa_supplicant/wpa_supplicant.conf
etc/binfmt.d/
etc/kernel/
etc/kernel/install.d/
etc/kernel/cmdline
etc/modules-load.d/
etc/sysctl.conf
etc/sysctl.d/
etc/sysctl.d/99-sysctl.conf
etc/NetworkManager/
etc/NetworkManager/NetworkManager.conf
etc/NetworkManager/conf.d/
etc/NetworkManager/dispatcher.d/
etc/NetworkManager/dispatcher.d/no-wait.d/
etc/NetworkManager/dispatcher.d/pre-down.d/
etc/NetworkManager/dispatcher.d/pre-up.d/
etc/NetworkManager/dnsmasq-shared.d/
etc/NetworkManager/dnsmasq.d/
etc/NetworkManager/system-connections/
etc/NetworkManager/system-connections/ens18.nmconnection
etc/UPower/
etc/UPower/UPower.conf
etc/cifs-utils/
etc/cifs-utils/idmap-plugin
etc/sudo-ldap.conf
etc/sudo.conf
etc/sudoers
etc/sudoers.d/
etc/geoclue/
etc/geoclue/geoclue.conf
etc/PackageKit/
etc/PackageKit/PackageKit.conf
etc/PackageKit/Vendor.conf
etc/PackageKit/CommandNotFound.conf
etc/speech-dispatcher/
etc/speech-dispatcher/modules/
etc/speech-dispatcher/modules/espeak-ng.conf
etc/speech-dispatcher/modules/cicero.conf
etc/speech-dispatcher/modules/dtk-generic.conf
etc/speech-dispatcher/modules/epos-generic.conf
etc/speech-dispatcher/modules/ivona.conf
etc/speech-dispatcher/modules/llia_phon-generic.conf
etc/speech-dispatcher/modules/mary-generic-disabled.conf
etc/speech-dispatcher/modules/swift-generic.conf
etc/speech-dispatcher/clients/
etc/speech-dispatcher/clients/emacs.conf
etc/speech-dispatcher/speechd.conf
etc/mke2fs.conf
etc/trusted-key.key
etc/dracut.conf
etc/dracut.conf.d/
etc/plymouth/
etc/plymouth/plymouthd.conf
etc/kdump/
etc/kdump/post.d/
etc/kdump/pre.d/
etc/kdump.conf
etc/makedumpfile.conf.sample
etc/cockpit/
etc/cockpit/machines.d/
etc/cockpit/ws-certs.d/
etc/cockpit/disallowed-users
etc/flatpak/
etc/flatpak/remotes.d/
etc/setroubleshoot/
etc/setroubleshoot/setroubleshoot.conf
etc/fprintd.conf
etc/udisks2/
etc/udisks2/mount_options.conf.example
etc/udisks2/udisks2.conf
etc/fwupd/
etc/fwupd/bios-settings.d/
etc/fwupd/bios-settings.d/README.md
etc/fwupd/daemon.conf
etc/fwupd/msr.conf
etc/fwupd/redfish.conf
etc/fwupd/remotes.d/
etc/fwupd/remotes.d/dell-esrt.conf
etc/fwupd/remotes.d/lvfs-testing.conf
etc/fwupd/remotes.d/lvfs.conf
etc/fwupd/remotes.d/vendor-directory.conf
etc/fwupd/remotes.d/vendor.conf
etc/fwupd/thunderbolt.conf
etc/fwupd/uefi_capsule.conf
etc/insights-client/
etc/insights-client/.exp.sed
etc/insights-client/.fallback.json
etc/insights-client/.fallback.json.asc
etc/insights-client/cert-api.access.redhat.com.pem
etc/insights-client/insights-client.conf
etc/insights-client/insights-client.motd
etc/insights-client/redhattools.pub.gpg
etc/insights-client/rpm.egg
etc/insights-client/rpm.egg.asc
etc/containers/
etc/containers/certs.d/
etc/containers/oci/
etc/containers/oci/hooks.d/
etc/containers/policy.json
etc/containers/registries.conf
etc/containers/registries.conf.d/
etc/containers/registries.conf.d/000-shortnames.conf
etc/containers/registries.conf.d/001-rhel-shortnames.conf
etc/containers/registries.conf.d/002-rhel-shortnames-overrides.conf
etc/containers/registries.d/
etc/containers/registries.d/default.yaml
etc/containers/registries.d/registry.access.redhat.com.yaml
etc/containers/registries.d/registry.redhat.io.yaml
etc/containers/storage.conf
etc/containers/systemd/
etc/brlapi.key
etc/brltty/
etc/brltty/Attributes/
etc/brltty/Attributes/invleft_right.atb
etc/brltty/Attributes/left_right.atb
etc/brltty/Attributes/upper_lower.atb
etc/brltty/Contraction/
etc/brltty/Contraction/af.ctb
etc/brltty/Contraction/am.ctb
etc/brltty/Contraction/countries.cti
etc/brltty/Contraction/de-1998.ctb
etc/brltty/Contraction/de-2015.ctb
etc/brltty/Contraction/de-g0.ctb
etc/brltty/Contraction/de-g1.ctb
etc/brltty/Contraction/de-g2.ctb
etc/brltty/Contraction/de-wort.cti
etc/brltty/Contraction/en-ueb-g2.ctb
etc/brltty/Contraction/en-us-g2.ctb
etc/brltty/Contraction/es.ctb
etc/brltty/Contraction/fr-g1.ctb
etc/brltty/Contraction/fr-g2.ctb
etc/brltty/Contraction/ha.ctb
etc/brltty/Contraction/id.ctb
etc/brltty/Contraction/ipa.ctb
etc/brltty/Contraction/ja.ctb
etc/brltty/Contraction/ko-g1.ctb
etc/brltty/Contraction/ko-g2.ctb
etc/brltty/Contraction/ko.ctb
etc/brltty/Contraction/latex-access.ctb
etc/brltty/Contraction/letters-latin.cti
etc/brltty/Contraction/lt.ctb
etc/brltty/Contraction/mg.ctb
etc/brltty/Contraction/mun.ctb
etc/brltty/Contraction/nabcc.cti
etc/brltty/Contraction/nl.ctb
etc/brltty/Contraction/ny.ctb
etc/brltty/Contraction/pt.ctb
etc/brltty/Contraction/si.ctb
etc/brltty/Contraction/spaces.cti
etc/brltty/Contraction/sw.ctb
etc/brltty/Contraction/th.ctb
etc/brltty/Contraction/zh-tw.ctb
etc/brltty/Contraction/zh-tw.cti
etc/brltty/Contraction/zu.ctb
etc/brltty/Input/
etc/brltty/Input/al/
etc/brltty/Input/al/abt_basic.kti
etc/brltty/Input/al/abt_extra.kti
etc/brltty/Input/al/abt_large.ktb
etc/brltty/Input/al/abt_small.ktb
etc/brltty/Input/al/bc-etouch.kti
etc/brltty/Input/al/bc-smartpad.kti
etc/brltty/Input/al/bc-thumb.kti
etc/brltty/Input/al/bc.kti
etc/brltty/Input/al/bc640.ktb
etc/brltty/Input/al/bc680.ktb
etc/brltty/Input/al/el.ktb
etc/brltty/Input/al/sat_common.kti
etc/brltty/Input/al/sat_large.ktb
etc/brltty/Input/al/sat_nav.kti
etc/brltty/Input/al/sat_small.ktb
etc/brltty/Input/al/sat_speech.kti
etc/brltty/Input/al/sat_tumblers.kti
etc/brltty/Input/al/voyager.ktb
etc/brltty/Input/android-chords.kti
etc/brltty/Input/at/
etc/brltty/Input/at/all.ktb
etc/brltty/Input/ba/
etc/brltty/Input/ba/all.txt
etc/brltty/Input/bd/
etc/brltty/Input/bd/all.txt
etc/brltty/Input/bg/
etc/brltty/Input/bg/all.ktb
etc/brltty/Input/bl/
etc/brltty/Input/bl/18.txt
etc/brltty/Input/bl/40_m20_m40.txt
etc/brltty/Input/bm/
etc/brltty/Input/bm/b2g.ktb
etc/brltty/Input/bm/b9b10.kti
etc/brltty/Input/bm/b9b11b10.kti
etc/brltty/Input/bm/command.kti
etc/brltty/Input/bm/connect.ktb
etc/brltty/Input/bm/conny.ktb
etc/brltty/Input/bm/d6.kti
etc/brltty/Input/bm/default.ktb
etc/brltty/Input/bm/display6.kti
etc/brltty/Input/bm/display7.kti
etc/brltty/Input/bm/dm80p.ktb
etc/brltty/Input/bm/front10.kti
etc/brltty/Input/bm/front6.kti
etc/brltty/Input/bm/horizontal.kti
etc/brltty/Input/bm/inka.ktb
etc/brltty/Input/bm/keyboard.kti
etc/brltty/Input/bm/orbit.ktb
etc/brltty/Input/bm/pro.ktb
etc/brltty/Input/bm/pronto.ktb
etc/brltty/Input/bm/pv.ktb
etc/brltty/Input/bm/rb.ktb
etc/brltty/Input/bm/routing.kti
etc/brltty/Input/bm/routing6.kti
etc/brltty/Input/bm/routing7.kti
etc/brltty/Input/bm/status.kti
etc/brltty/Input/bm/sv.ktb
etc/brltty/Input/bm/ultra.ktb
etc/brltty/Input/bm/v40.ktb
etc/brltty/Input/bm/v80.ktb
etc/brltty/Input/bm/vertical.kti
etc/brltty/Input/bm/vk.ktb
etc/brltty/Input/bm/wheels.kti
etc/brltty/Input/bn/
etc/brltty/Input/bn/all.ktb
etc/brltty/Input/bn/input.kti
etc/brltty/Input/bp/
etc/brltty/Input/bp/all.kti
etc/brltty/Input/cb/
etc/brltty/Input/cb/all.ktb
etc/brltty/Input/ce/
etc/brltty/Input/ce/all.ktb
etc/brltty/Input/ce/novem.ktb
etc/brltty/Input/chords.kti
etc/brltty/Input/cn/
etc/brltty/Input/cn/all.ktb
etc/brltty/Input/ec/
etc/brltty/Input/ec/all.txt
etc/brltty/Input/ec/spanish.txt
etc/brltty/Input/eu/
etc/brltty/Input/eu/all.txt
etc/brltty/Input/eu/braille.kti
etc/brltty/Input/eu/clio.ktb
etc/brltty/Input/eu/common.kti
etc/brltty/Input/eu/esys_large.ktb
etc/brltty/Input/eu/esys_medium.ktb
etc/brltty/Input/eu/esys_small.ktb
etc/brltty/Input/eu/esytime.ktb
etc/brltty/Input/eu/iris.ktb
etc/brltty/Input/eu/joysticks.kti
etc/brltty/Input/eu/routing.kti
etc/brltty/Input/eu/sw12.kti
etc/brltty/Input/eu/sw34.kti
etc/brltty/Input/eu/sw56.kti
etc/brltty/Input/fa/
etc/brltty/Input/fa/all.ktb
etc/brltty/Input/fs/
etc/brltty/Input/fs/bumpers.kti
etc/brltty/Input/fs/common.kti
etc/brltty/Input/fs/focus.kti
etc/brltty/Input/fs/focus1.ktb
etc/brltty/Input/fs/focus14.ktb
etc/brltty/Input/fs/focus40.ktb
etc/brltty/Input/fs/focus80.ktb
etc/brltty/Input/fs/pacmate.ktb
etc/brltty/Input/fs/rockers.kti
etc/brltty/Input/hd/
etc/brltty/Input/hd/mbl.ktb
etc/brltty/Input/hd/pfl.ktb
etc/brltty/Input/hm/
etc/brltty/Input/hm/beetle.ktb
etc/brltty/Input/hm/braille.kti
etc/brltty/Input/hm/common.kti
etc/brltty/Input/hm/contexts.kti
etc/brltty/Input/hm/edge.ktb
etc/brltty/Input/hm/f14.kti
etc/brltty/Input/hm/f18.kti
etc/brltty/Input/hm/fnkey.kti
etc/brltty/Input/hm/left.kti
etc/brltty/Input/hm/letters.kti
etc/brltty/Input/hm/pan.ktb
etc/brltty/Input/hm/pan.kti
etc/brltty/Input/hm/qwerty.ktb
etc/brltty/Input/hm/qwerty.kti
etc/brltty/Input/hm/right.kti
etc/brltty/Input/hm/scroll.ktb
etc/brltty/Input/hm/scroll.kti
etc/brltty/Input/hm/sync.ktb
etc/brltty/Input/ht/
etc/brltty/Input/ht/ab.ktb
etc/brltty/Input/ht/ac4.ktb
etc/brltty/Input/ht/alo.ktb
etc/brltty/Input/ht/as40.ktb
etc/brltty/Input/ht/bb.ktb
etc/brltty/Input/ht/bbp.ktb
etc/brltty/Input/ht/bkwm.ktb
etc/brltty/Input/ht/brln.ktb
etc/brltty/Input/ht/bs.kti
etc/brltty/Input/ht/bs40.ktb
etc/brltty/Input/ht/bs80.ktb
etc/brltty/Input/ht/cb40.ktb
etc/brltty/Input/ht/dots.kti
etc/brltty/Input/ht/easy.ktb
etc/brltty/Input/ht/input.kti
etc/brltty/Input/ht/joystick.kti
etc/brltty/Input/ht/keypad.kti
etc/brltty/Input/ht/mc88.ktb
etc/brltty/Input/ht/mdlr.ktb
etc/brltty/Input/ht/me.kti
etc/brltty/Input/ht/me64.ktb
etc/brltty/Input/ht/me88.ktb
etc/brltty/Input/ht/rockers.kti
etc/brltty/Input/ht/wave.ktb
etc/brltty/Input/hw/
etc/brltty/Input/hw/B80.ktb
etc/brltty/Input/hw/BI14.ktb
etc/brltty/Input/hw/BI32.ktb
etc/brltty/Input/hw/BI40.ktb
etc/brltty/Input/hw/C20.ktb
etc/brltty/Input/hw/M40.ktb
etc/brltty/Input/hw/NLS.ktb
etc/brltty/Input/hw/braille.kti
etc/brltty/Input/hw/command.kti
etc/brltty/Input/hw/joystick.kti
etc/brltty/Input/hw/one.ktb
etc/brltty/Input/hw/routing.kti
etc/brltty/Input/hw/thumb.kti
etc/brltty/Input/hw/touch.ktb
etc/brltty/Input/ic/
etc/brltty/Input/ic/bb.ktb
etc/brltty/Input/ic/chords.kti
etc/brltty/Input/ic/common.kti
etc/brltty/Input/ic/nvda.ktb
etc/brltty/Input/ic/route.kti
etc/brltty/Input/ic/toggle.kti
etc/brltty/Input/ir/
etc/brltty/Input/ir/all.kti
etc/brltty/Input/ir/brl.ktb
etc/brltty/Input/ir/pc.ktb
etc/brltty/Input/lb/
etc/brltty/Input/lb/all.txt
etc/brltty/Input/lt/
etc/brltty/Input/lt/all.txt
etc/brltty/Input/mb/
etc/brltty/Input/mb/all.txt
etc/brltty/Input/md/
etc/brltty/Input/md/common.kti
etc/brltty/Input/md/default.ktb
etc/brltty/Input/md/fk.ktb
etc/brltty/Input/md/fk_s.ktb
etc/brltty/Input/md/fkeys.kti
etc/brltty/Input/md/kbd.ktb
etc/brltty/Input/md/keyboard.kti
etc/brltty/Input/md/status.kti
etc/brltty/Input/menu.kti
etc/brltty/Input/mm/
etc/brltty/Input/mm/common.kti
etc/brltty/Input/mm/pocket.ktb
etc/brltty/Input/mm/smart.ktb
etc/brltty/Input/mn/
etc/brltty/Input/mn/all.txt
etc/brltty/Input/mt/
etc/brltty/Input/mt/bd1_3.ktb
etc/brltty/Input/mt/bd1_3.kti
etc/brltty/Input/mt/bd1_3s.ktb
etc/brltty/Input/mt/bd1_6.ktb
etc/brltty/Input/mt/bd1_6.kti
etc/brltty/Input/mt/bd1_6s.ktb
etc/brltty/Input/mt/bd2.ktb
etc/brltty/Input/mt/status.kti
etc/brltty/Input/no/
etc/brltty/Input/no/all.txt
etc/brltty/Input/np/
etc/brltty/Input/np/all.ktb
etc/brltty/Input/pg/
etc/brltty/Input/pg/all.ktb
etc/brltty/Input/pm/
etc/brltty/Input/pm/2d_l.ktb
etc/brltty/Input/pm/2d_s.ktb
etc/brltty/Input/pm/bar.kti
etc/brltty/Input/pm/c.ktb
etc/brltty/Input/pm/c_486.ktb
etc/brltty/Input/pm/el2d_80s.ktb
etc/brltty/Input/pm/el40c.ktb
etc/brltty/Input/pm/el40s.ktb
etc/brltty/Input/pm/el60c.ktb
etc/brltty/Input/pm/el66s.ktb
etc/brltty/Input/pm/el70s.ktb
etc/brltty/Input/pm/el80_ii.ktb
etc/brltty/Input/pm/el80c.ktb
etc/brltty/Input/pm/el80s.ktb
etc/brltty/Input/pm/el_2d_40.ktb
etc/brltty/Input/pm/el_2d_66.ktb
etc/brltty/Input/pm/el_2d_80.ktb
etc/brltty/Input/pm/el_40_p.ktb
etc/brltty/Input/pm/el_80.ktb
etc/brltty/Input/pm/elb_tr_20.ktb
etc/brltty/Input/pm/elb_tr_32.ktb
etc/brltty/Input/pm/elba_20.ktb
etc/brltty/Input/pm/elba_32.ktb
etc/brltty/Input/pm/front13.kti
etc/brltty/Input/pm/front9.kti
etc/brltty/Input/pm/ib_80.ktb
etc/brltty/Input/pm/keyboard.kti
etc/brltty/Input/pm/keys.kti
etc/brltty/Input/pm/live.ktb
etc/brltty/Input/pm/routing.kti
etc/brltty/Input/pm/status0.kti
etc/brltty/Input/pm/status13.kti
etc/brltty/Input/pm/status2.kti
etc/brltty/Input/pm/status20.kti
etc/brltty/Input/pm/status22.kti
etc/brltty/Input/pm/status4.kti
etc/brltty/Input/pm/switches.kti
etc/brltty/Input/pm/trio.ktb
etc/brltty/Input/sk/
etc/brltty/Input/sk/bdp.ktb
etc/brltty/Input/sk/ntk.ktb
etc/brltty/Input/tn/
etc/brltty/Input/tn/all.txt
etc/brltty/Input/toggle.kti
etc/brltty/Input/ts/
etc/brltty/Input/ts/nav.kti
etc/brltty/Input/ts/nav20.ktb
etc/brltty/Input/ts/nav40.ktb
etc/brltty/Input/ts/nav80.ktb
etc/brltty/Input/ts/nav_large.kti
etc/brltty/Input/ts/nav_small.kti
etc/brltty/Input/ts/pb.kti
etc/brltty/Input/ts/pb40.ktb
etc/brltty/Input/ts/pb65.ktb
etc/brltty/Input/ts/pb80.ktb
etc/brltty/Input/ts/pb_large.kti
etc/brltty/Input/ts/pb_small.kti
etc/brltty/Input/ts/routing.kti
etc/brltty/Input/tt/
etc/brltty/Input/tt/all.txt
etc/brltty/Input/vd/
etc/brltty/Input/vd/all.txt
etc/brltty/Input/vo/
etc/brltty/Input/vo/all.ktb
etc/brltty/Input/vo/all.kti
etc/brltty/Input/vo/bp.ktb
etc/brltty/Input/vr/
etc/brltty/Input/vr/all.txt
etc/brltty/Input/vs/
etc/brltty/Input/vs/all.txt
etc/brltty/Input/xw/
etc/brltty/Input/xw/all.txt
etc/brltty/Keyboard/
etc/brltty/Keyboard/braille.ktb
etc/brltty/Keyboard/braille.kti
etc/brltty/Keyboard/desktop.ktb
etc/brltty/Keyboard/desktop.kti
etc/brltty/Keyboard/keypad.ktb
etc/brltty/Keyboard/kp_say.kti
etc/brltty/Keyboard/kp_speak.kti
etc/brltty/Keyboard/laptop.ktb
etc/brltty/Keyboard/sun_type6.ktb
etc/brltty/Text/
etc/brltty/Text/no-generic.ttb
etc/brltty/Text/alias.tti
etc/brltty/Text/no-oup.ttb
etc/brltty/Text/ar.ttb
etc/brltty/Text/no.ttb
etc/brltty/Text/as.ttb
etc/brltty/Text/kru.ttb
etc/brltty/Text/ascii-basic.tti
etc/brltty/Text/num-alias.tti
etc/brltty/Text/awa.ttb
etc/brltty/Text/num-dot6.tti
etc/brltty/Text/bengali.tti
etc/brltty/Text/num-dot8.tti
etc/brltty/Text/bg.ttb
etc/brltty/Text/num-french.tti
etc/brltty/Text/bh.ttb
etc/brltty/Text/num-nemd8.tti
etc/brltty/Text/blocks.tti
etc/brltty/Text/num-nemeth.tti
etc/brltty/Text/bn.ttb
etc/brltty/Text/nwc.ttb
etc/brltty/Text/bo.ttb
etc/brltty/Text/or.ttb
etc/brltty/Text/boxes.tti
etc/brltty/Text/oriya.tti
etc/brltty/Text/bra.ttb
etc/brltty/Text/pa.ttb
etc/brltty/Text/brf.ttb
etc/brltty/Text/pi.ttb
etc/brltty/Text/common.tti
etc/brltty/Text/pl.ttb
etc/brltty/Text/cs.ttb
etc/brltty/Text/kok.ttb
etc/brltty/Text/ctl-latin.tti
etc/brltty/Text/pt.ttb
etc/brltty/Text/cy.ttb
etc/brltty/Text/punc-alternate.tti
etc/brltty/Text/da-1252.ttb
etc/brltty/Text/punc-basic.tti
etc/brltty/Text/da-lt.ttb
etc/brltty/Text/punc-tibetan.tti
etc/brltty/Text/da.ttb
etc/brltty/Text/mi.ttb
etc/brltty/Text/de-chess.tti
etc/brltty/Text/ro.ttb
etc/brltty/Text/de.ttb
etc/brltty/Text/mg.ttb
etc/brltty/Text/devanagari.tti
etc/brltty/Text/ru.ttb
etc/brltty/Text/dra.ttb
etc/brltty/Text/sa.ttb
etc/brltty/Text/el.ttb
etc/brltty/Text/ml.ttb
etc/brltty/Text/en-chess.tti
etc/brltty/Text/mni.ttb
etc/brltty/Text/en-na-ascii.tti
etc/brltty/Text/mr.ttb
etc/brltty/Text/en-nabcc.ttb
etc/brltty/Text/sat.ttb
etc/brltty/Text/en.ttb
etc/brltty/Text/sd.ttb
etc/brltty/Text/en_CA.ttb
etc/brltty/Text/se.ttb
etc/brltty/Text/en_GB.ttb
etc/brltty/Text/sk.ttb
etc/brltty/Text/en_US.ttb
etc/brltty/Text/sl.ttb
etc/brltty/Text/eo.ttb
etc/brltty/Text/sv-1989.ttb
etc/brltty/Text/es.ttb
etc/brltty/Text/sv-1996.ttb
etc/brltty/Text/et.ttb
etc/brltty/Text/sv.ttb
etc/brltty/Text/fi.ttb
etc/brltty/Text/sw.ttb
etc/brltty/Text/fr-2007.ttb
etc/brltty/Text/mt.ttb
etc/brltty/Text/fr-cbifs.ttb
etc/brltty/Text/ta.ttb
etc/brltty/Text/fr-vs.ttb
etc/brltty/Text/tamil.tti
etc/brltty/Text/fr.ttb
etc/brltty/Text/te.ttb
etc/brltty/Text/fr_CA.ttb
etc/brltty/Text/telugu.tti
etc/brltty/Text/fr_FR.ttb
etc/brltty/Text/tr.ttb
etc/brltty/Text/ga.ttb
etc/brltty/Text/uk.ttb
etc/brltty/Text/gd.ttb
etc/brltty/Text/vi.ttb
etc/brltty/Text/gon.ttb
etc/brltty/Text/win-1252.tti
etc/brltty/Text/greek.tti
etc/brltty/Text/gu.ttb
etc/brltty/Text/mun.ttb
etc/brltty/Text/gujarati.tti
etc/brltty/Text/mwr.ttb
etc/brltty/Text/gurmukhi.tti
etc/brltty/Text/he.ttb
etc/brltty/Text/hi.ttb
etc/brltty/Text/hr.ttb
etc/brltty/Text/hu.ttb
etc/brltty/Text/hy.ttb
etc/brltty/Text/is.ttb
etc/brltty/Text/it.ttb
etc/brltty/Text/kannada.tti
etc/brltty/Text/kha.ttb
etc/brltty/Text/kn.ttb
etc/brltty/Text/lt.ttb
etc/brltty/Text/ne.ttb
etc/brltty/Text/ltr-alias.tti
etc/brltty/Text/new.ttb
etc/brltty/Text/ltr-cyrillic.tti
etc/brltty/Text/nl.ttb
etc/brltty/Text/ltr-dot8.tti
etc/brltty/Text/ltr-latin.tti
etc/brltty/Text/nl_BE.ttb
etc/brltty/Text/ltr-tibetan.tti
etc/brltty/Text/lv.ttb
etc/brltty/Text/nl_NL.ttb
etc/brltty/Text/malayalam.tti
etc/brltty.conf
etc/foomatic/
etc/foomatic/defaultspooler
etc/cupshelpers/
etc/cupshelpers/preferreddrivers.xml
etc/vmware-tools/
etc/vmware-tools/poweroff-vm-default
etc/vmware-tools/poweron-vm-default
etc/vmware-tools/resume-vm-default
etc/vmware-tools/scripts/
etc/vmware-tools/scripts/vmware/
etc/vmware-tools/scripts/vmware/network
etc/vmware-tools/statechange.subr
etc/vmware-tools/suspend-vm-default
etc/vmware-tools/tools.conf.example
etc/vmware-tools/vgauth/
etc/vmware-tools/vgauth/schemas/
etc/vmware-tools/vgauth/schemas/XMLSchema-hasFacetAndProperty.xsd
etc/vmware-tools/vgauth/schemas/XMLSchema-instance.xsd
etc/vmware-tools/vgauth/schemas/XMLSchema.dtd
etc/vmware-tools/vgauth/schemas/XMLSchema.xsd
etc/vmware-tools/vgauth/schemas/catalog.xml
etc/vmware-tools/vgauth/schemas/datatypes.dtd
etc/vmware-tools/vgauth/schemas/saml-schema-assertion-2.0.xsd
etc/vmware-tools/vgauth/schemas/xenc-schema.xsd
etc/vmware-tools/vgauth/schemas/xml.xsd
etc/vmware-tools/vgauth/schemas/xmldsig-core-schema.xsd
etc/vmware-tools/vgauth.conf
etc/chromium/
etc/chromium/native-messaging-hosts/
etc/chromium/native-messaging-hosts/org.gnome.browser_connector.json
etc/chromium/native-messaging-hosts/org.gnome.chrome_gnome_shell.json
etc/nvme/
etc/nvme/discovery.conf
etc/nvme/hostnqn
etc/nvme/hostid
etc/firefox/
etc/firefox/pref/
etc/ras/
etc/ras/dimm_labels.d/
etc/pbm2ppa.conf
etc/pnm2ppa.conf
etc/enscript.cfg
etc/firewalld/
etc/firewalld/firewalld.conf
etc/firewalld/helpers/
etc/firewalld/icmptypes/
etc/firewalld/ipsets/
etc/firewalld/lockdown-whitelist.xml
etc/firewalld/policies/
etc/firewalld/services/
etc/firewalld/zones/
etc/firewalld/zones/public.xml
etc/firewalld/zones/public.xml.old
etc/tuned/
etc/tuned/active_profile
etc/tuned/bootcmdline
etc/tuned/post_loaded_profile
etc/tuned/profile_mode
etc/tuned/recommend.d/
etc/tuned/tuned-main.conf
etc/rhc/
etc/rhc/workers/
etc/rhc/workers/rhc-package-manager.toml
etc/rhc/config.toml
etc/yum/
etc/yum/pluginconf.d
etc/yum/protected.d
etc/yum/vars
etc/yum.conf
etc/grub2.cfg
etc/pinforc
etc/alsa/
etc/alsa/conf.d/
etc/alsa/conf.d/50-pipewire.conf
etc/alsa/conf.d/99-pipewire-default.conf
etc/alsa/state-daemon.conf
etc/alsa/alsactl.conf
etc/at.deny
etc/dhcp/
etc/dhcp/dhclient.d/
etc/dhcp/dhclient.d/chrony.sh
etc/chrony.conf
etc/chrony.keys
etc/mcelog/
etc/mcelog/mcelog.conf
etc/mcelog/triggers/
etc/mcelog/triggers/cache-error-trigger
etc/mcelog/triggers/dimm-error-trigger
etc/mcelog/triggers/page-error-trigger
etc/mcelog/triggers/socket-memory-error-trigger
etc/microcode_ctl/
etc/microcode_ctl/ucode_with_caveats/
etc/updatedb.conf
etc/smartmontools/
etc/smartmontools/smartd.conf
etc/smartmontools/smartd_warning.d/
etc/smartmontools/smartd_warning.sh
etc/dnsmasq.conf
etc/dnsmasq.d/
etc/qemu-ga/
etc/qemu-ga/fsfreeze-hook
etc/qemu-ga/fsfreeze-hook.d/
etc/man_db.conf
etc/rsyncd.conf
etc/wgetrc
etc/nanorc
etc/virc
etc/mailcap
etc/mime.types
etc/localtime
etc/locale.conf
etc/vconsole.conf
etc/hostname
etc/.updated
etc/subuid-
etc/subgid-
etc/machine-info
[student@rhel9-01 rhcsa]$
```

##### Task2

Filter all usernames (in the first column) from /etc/passwd in alphabetical order and with no blank lines in the target file and write them to /var/tmp/users

You got this wrong. The first is yours, the second is th better solution. It minimizes regular expressions, uses cut instead. May be easier moving forward. `grep -v '^$'` removes all empty lines.

``` bash
#command
grep -o '^[^:]*' /etc/passwd | sort | uniq > /var/tmp/users
cut -d : -f 1 /etc/passwd | sort | grep -v '^$' > /var/tmp/users
```

###### Output

``` bash
#output
[student@rhel9-01 rhcsa]$ cat /var/tmp/users
adm
avahi
bin
chrony
clevis
cockpit-ws
cockpit-wsinstance
colord
daemon
dbus
dnsmasq
flatpak
ftp
games
gdm
geoclue
gnome-initial-setup
halt
libstoragemgmt
lp
mail
nobody
operator
pipewire
polkitd
root
rtkit
setroubleshoot
shutdown
sshd
sssd
student
sync
systemd-coredump
systemd-oom
tcpdump
tss
```

##### Task3

Create a user with the name bob. Next, find all files that are owned by user bob and copy them to /root/userfiles

``` bash
#command
sudo useradd bob
mkdir -p /root/userfiles
find / -user bob -type f -exec cp {} /root/userfiles \;
```

###### Output

``` bash
#output
[student@rhel9-01 rhcsa]$ sudo mkdir -p /root/userfiles
[student@rhel9-01 rhcsa]$ sudo find / -user bob -type f -exec cp {} /root/userfiles \;
find: ‘/proc/4003/task/4003/fdinfo/6’: No such file or directory
find: ‘/proc/4003/fdinfo/5’: No such file or directory
[student@rhel9-01 rhcsa]$ sudo ls -lah /root/userfiles
total 12K
drwxr-xr-x. 2 root root  73 Apr  8 09:39 .
dr-xr-x---. 5 root root 176 Apr  8 09:39 ..
-rw-r--r--. 1 root root  18 Apr  8 09:39 .bash_logout
-rw-r--r--. 1 root root 141 Apr  8 09:39 .bash_profile
-rw-r--r--. 1 root root 492 Apr  8 09:39 .bashrc
-rw-r-----. 1 root root   0 Apr  8 09:39 bob
```

### Managing Software

- Slide 55
- During the exam you are on a air-gapped virtual machine.
- The RHEL DVD is mounted as a repository.
- This lab is able setting this up yourself.
- You use `dnf` or `yum` for installing packages
- All installed packages get installed in the RPM database along with dependencies
- A repo is a collection of indexed RPM packages

``` bash
#commands
```

###### Output

``` bash
#output
[root@localhost /]# dd if=/dev/sr0 of=/rhel9.iso bs=4M status=progress
10443816960 bytes (10 GB, 9.7 GiB) copied, 105 s, 99.4 MB/s
2510+1 records in
2510+1 records out
10528882688 bytes (11 GB, 9.8 GiB) copied, 105.767 s, 99.5 MB/s
[root@localhost /]# mkdir /repo
[root@localhost /]# echo "/rhel9.iso /repo iso9660 defaults 0 0" >> /etc/fstab
[root@localhost /]# mount -a
```

#### Adding Repositories

- Slide 60
- This is critical to the exam.
- GPG checks are not needed for the course. Make sure `gpgcheck=0` in the repo.

##### Commands

``` bash
#commands
dnf config-manager --add-repo="file:///repo/AppStream"  
cat >> /etc/yum.repos.d/AppStream.repo <<EOF  
> [AppStream]  
> name=AppStream  
> baseurl=file:///repo/AppStream  
> gpgcheck=0  
EOF
```

##### Output

``` bash
#output
[root@localhost /]
dnf repolist
Updating Subscription Management repositories.
Unable to read consumer identity

This system is not registered with an entitlement server. You can use subscription-manager to register.

Warning: failed loading '/etc/yum.repos.d/AppStream.repo', skipping.
repo id                                repo name
repo_AppStream                         created by dnf config-manager from file:///repo/AppStream
```

#### Labs

Ensure your system is using a repository for base packages as well as application streams
\##### Output

``` bash
#output
[root@localhost /]# dnf repolist
Updating Subscription Management repositories.
Unable to read consumer identity

This system is not registered with an entitlement server. You can use subscription-manager to register.

Warning: failed loading '/etc/yum.repos.d/AppStream.repo', skipping.
repo id                                repo name
repo_AppStream                         created by dnf config-manager from file:///repo/AppStream
```

Find the package that contains the seinfo program file and install it
\##### Output

``` bash
#output
```

Download the httpd package from the repositories without installing it, and query to see if there are any scripts in it
\##### Output

``` bash
#output
```

### su and sudo

- Slide 12
- To add somebody to sudo group `usermod -aG wheel myuser`
- Never enable \`%wheel ALL=(ALL) NOPASSWD:ALL
- You can modify token expiration by editing the \`timestamp_type=global,timestamp_timeout=60"
- Drop files can be added to a user to limit access, `lisa ALL=/sbin/useradd, /usr/bin/passwd`
- This can lock a user down a bit. This is worth exploring with ansible to permit temporary permissions.
  \#### Commands

``` bash
#commands
useradd lisa
useradd linda
passwd linda # set password
su - linda
id # get groups of the member
sudo ls -l /root
# from root type systemctl ...
visudo
# add linda as an example
linda ALL=/usr/bin/passwd, ! /usr/bin/passwd root # this is not good, must have an exclution list to prevent Linda from resetting root
# Now linda can reset all passwords except root and she will be denied
```

### Users and Groups

Processes use system accounts
- People use regular user accounts
- When you create new user the home directory comes from `/etc/skel`
- To lock an account `usernmod -L <user>` and `usermod -U <user>` to unblock
- To expire an account `usernmode -e 2032-01-01 <user>`
- If you mod an account to use `/sbin/nologin` then the user cannot login. Useful for [system accounts](system accounts "wikilink")
- `usermod -s /sbin/nologin myapp`
\##### Commands

``` bash
#commands
useradd # create users
usermod # modify users
userdel # delete users
passwd # set passwords
groupadd
groupdel
lid -g groupName # list all users that are a member of groupName
```

#### Lab: Manage Users and Groups

- Slide 25

### File Ownership

##### Commands

``` bash
#commands
chown user[:group] file to set user-ownership
chgrp <group> file to set group-ownership
```

#### Manage Permissions

|             | On files        | On directories                         |
|-------------|-----------------|----------------------------------------|
| Read (4)    | Open the file   | List files and subdirectories          |
| Write (2)   | Modify the file | Create/Delete files and subdirectories |
| Execute (1) | Run the file    | Use cd to activate the directory       |

##### Commands

    chmod
    chmod 750 myfile
    chmod +x myscript

##### Special X considerations

- When `x` is applied recusively, it would amke all directories and well as files executable
- Only useful if applying executable in a recruisive way

#### Demo

``` bash
mkdir -p /data/profs /data/students
chmown :profs /data/profs
chgroup students /data/students
chmod 770 /data/students
chmod g+w,o-rx /data/profs
```

#### Shared Group Directories

- When members of a single group need to share files in a directory
- Use a Set group ID (SGID) permission ensures that all files in the shared group directory and group owned by the owner of the directory
- A sticky bit permission makes sure that only the user who is owner, or directory, is allowed to delete it
  \##### Shared Group Directories steps

``` bash
chmod g+s mydir  # applies SGID
chmod +t mydir   # assigns sticky bit
chmod 3770 mydir # assigns the SGIDD and sticky bit and +rwx for bot user and group
```

##### SGID demo

    This is in a demo on slide 35.

### Partitions

## Tasks

- ☐ Review repositories lab
- ☐ Users and groups labs
- ☐ Review permissions and understand both 777 and g+w methods
  \## ❓ Questions
- ☐ For managing repositories, for AppStream, why does this mount to the DVD repo I built in the previous lab?
- \[ \]

## 🔗 Related links

**Recommended Preparation**:

- Watch: [*Linux Fundamentals, 2nd Edition*](https://learning.oreilly.com/videos/linux-fundamentals-2nd/9780137929313/) by Sander van Vugt
- Attend: [*Linux Fundamentals Bootcamp*](https://learning.oreilly.com/search/?q=Linux%20Fundamentals%20Bootcamp%20Sander%20van%20Vugt&type=live-event-series&publishers=Pearson) by Sander van Vugt
- Watch: [*Red Hat Certified System Administrator (RHCSA) RHEL 9*](https://learning.oreilly.com/videos/red-hat-certified/9780137931521/) by Sander van Vugt

**Recommended Follow-up**:

- Read: [*Red Hat RHCSA 9 Cert Guide: EX200*](https://learning.oreilly.com/library/view/red-hat-rhcsa/9780138096311/) by Sander van Vugt:
- Watch: [*Bash Shell Scripting, 2nd Edition*](https://learning.oreilly.com/videos/bash-shell-scripting/9780137689064/) by Sander van Vugt
- Attend: [Linux Security from Basics to Guru](https://learning.oreilly.com/search/?q=sander%20van%20vugt%20linux%20security%20from%20basics%20to%20guru&type=live-event-series&publishers=Pearson) by Sander van Vugt
- Attend: [*Mastering Systemd*](https://learning.oreilly.com/search/?q=Mastering%20Systemd%20Sander%20van%20Vugt&type=live-event-series&publishers=Pearson) by Sander van Vugt
- Attend: [*Linux Troubleshooting*](https://learning.oreilly.com/search/?q=Linux%20Troubleshooting%20Sander%20van%20Vugt&type=live-event-series&publishers=Pearson) by Sander van Vugt
- [Red Hat Certified Systems Administrator (RHCSA) Labs](https://learning.oreilly.com/playlists/5eb6cb3b-1f3c-4b67-a3d4-c9a3d4aaaab9/)
- [Red Hat Certified Systems Administrator (RHCSA) Challenge Labs](https://learning.oreilly.com/playlists/b12ad4cc-6ad2-48ba-aecb-00a8158f6255/)
- 
