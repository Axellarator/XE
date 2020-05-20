V129M 2020/05/17 
(A)Automake �p�b�P�[�W �����菇�B

    �f�B�X�g���r���[�V�����ɂ���Ă͓�����t�H���_�[��ύX����K�v�����邩������܂���B
    ./configure �����s����O��configure���C�����Ă��������B
        html �w���v��  "packagehelpdir",                ���ݒl�� /usr/local/share/gnome/help/gxe
        icon ��        "packagepixmapsdir",             ���ݒl�� /usr/local/share/pixmaps/gxe
        bins ��        ./configure --bindir=PATH�Ŏw��B���ݒl�� /usr/local/bin

    (1)tar -zxvf gxe-v.rr.tar.gz    (v.rr : version)
    (2)cd gxe-v.rr
    (3)./configure
    (4)make
    (5)make install (root�Ŏ��s�Aubuntu�ł� "sudo make install")

       ���O�̋���������邽�ߎ���bin��������������܂��B����ȊO�̃c�[���͎����ŃR�s�[���Ă��������B
         gxe, xe, xprint, gxp, xfc, xdc
    (6)gnome-terminal �Ȃ��� konsole ���J���� gxe �Ȃ��� xe �Ɠ��͂���B
       �w���vhtml�͗����グ�� ��2�s�� "help" �Ȃ��� "?" ����͂���ƃu���E�U�[����ς邱�Ƃ��o���܂��B
    (7)ssh
       �����[�g��xe�N������ꍇ�Assh(d)�̐ݒ���`�F�b�N�B
           local :/etc/ssh/ssh_config
                      set "SendEnv LANG LC_*"
           remote:/etc/ssh/sshd_config
                      set "AcceptEnv LANG LC_*"
                      set "X11Forwarding yes"
                      xhost +local:username    local=local ip addr, username=your user id
                  xauth �͓����ς݂� ?

       �����[�g��gxe�N������ꍇ -X �I�v�V�������w�肷��B
           ssh -X uid@remotehost

(B)�g���u���V���[�e�B���O
    ���̃f�X�g���r���[�V�����Ńe�X�g���܂����B
        RH9, FC5, Kubuntu6, Ubuntu7, openSUSE10, Vine4, TurbolinuxFUJItrial
        Debian4.0r2(2008/01/25)
        ubuntu8, FC12

  (B1) ./configure �G���[

    (1) no acceptable C compiler found in $PATH
        ===> install gcc
             on debian8.10: apt-get install build-essential
    (2) crt1.o no such file   (Debian 4.0)
        (development �p�b�P�[�W�̃T�t�B�b�N�X�̓f�X�g���r���[�V�������ƂɈقȂ�܂�)
        ===> install libglib2.0-dev
        ===> install libc6-dev (ubuntu8)
    (3) "term.h" not found
        ===> install ncurses-develop. 
        ncursesw/ncurses.h not found.
        ===> install ncursesw-develop. 
             (debian8.10)
                 apt-get install libncurses5-dev
                 apt-get install libncursesw5-dev
    (4) cups/cups.h not found.
        ===> apt-get install libncursesw5-dev
        ===> install cups-devel
        ===> install libgnomecups1.0.dev (ubuntu8)
        ===> install libcupsys2-dev      (ubuntu9)
    (5) No package libgnomeui-2.0 found
        No package gnome-vfs-module-2.0 found
        No package libgnomeprint-2.2 found
        ===> install libgnomeui-devel
             install libgnomeprint-devel
        ===> install libgnomeui-dev
             install libgnomeprint2.2-dev  (ubuntu8)
    (6) pkg-config was not found
        ===> install pkg-config
    (7) CHK_INSTALL_GTK3...no and  CHK_INSTALL_GTK2..no
        ==>apt-file --package-only search gtk+-2.0
           apt-file --package-only search gtk+-3.0
           apt-get install libgtk2.0-dev
             or 
           apt-get install libgtk-3-dev
    (8) CHK_EXIST_GTK3_LIBGNOME2... no
        ===> install libgnome2-dev
    (9) can not find -lncursesw
        ===> apt-get install libncursesw5-dev

  (B2) make�̃G���[�B

    (1) "term.h" not found
        ===> install ncurses-develop. 
    (2) Cannot find the librarly libssl (On TurbolinuxFUJI trial version)
        ===> install openssp
    (3) Cannot find the librarly libpopt.la
        ===> install popt from ftp site
    (4) X error'BadDevice invalid or uninitialized device 168  (Ubuntu-7)
        :        major 145 .. minor 3 resource 0x00
        Failed to open Device
        ===> /etc/X11/xorg.conf was changed.

        Following lines are comment out

        ##Section "InputDevice"
        ##  Driver        "wacom"
        ##  Identifier    "stylus"
        ##  Option        "Device"        "/dev/wacom"          # Change to
        ##                                                      # /dev/input/event
        ##                                                      # for USB
        ##  Option        "Type"          "stylus"
        ##  Option        "ForceDevice"   "ISDV4"               # Tablet PC ONLY
        ##EndSection

        ##Section "InputDevice"
        ##  Driver        "wacom"
        ##  Identifier    "eraser"
        ##  Option        "Device"        "/dev/wacom"          # Change to
        ##                                                      # /dev/input/event
        ##                                                      # for USB
        ##  Option        "Type"          "eraser"
        ##  Option        "ForceDevice"   "ISDV4"               # Tablet PC ONLY
        ##EndSection

        ##Section "InputDevice"
        ##  Driver        "wacom"
        ##  Identifier    "cursor"
        ##  Option        "Device"        "/dev/wacom"          # Change to
        ##                                                      # /dev/input/event
        ##                                                      # for USB
        ##  Option        "Type"          "cursor"
        ##  Option        "ForceDevice"   "ISDV4"               # Tablet PC ONLY
        ##EndSection

                And in Section "ServerLayout"

        ##    InputDevice     "stylus" "SendCoreEvents"
        ##    InputDevice     "cursor" "SendCoreEvents"
        ##    InputDevice     "eraser" "SendCoreEvents"

    (5) /bin/sh' /usr/bin/esd: not found (Ubuntu-7)
        ===> install esound

  (B3) execution

    (1)  WARNING **:Could'nt find pixmap file gxe/wxe.png
        ===> "make install" �� root �Ŏ��s. (A)�̓�����t�H���_�[���`�F�b�N�B

    (2) WARNING **: IPP request failed with status 1030
        ===> CUPS �v�����^�[���Z�b�g�A�b�v����B�v�����^�[���Ȃ����ĂȂ��ꍇ�ł������ݒ肷��B

    (3) WARNING **: IPP request failed with status 1280
        ===> CUPS �T�[�r�X�f�[�������J�n.

    (4) ??? xe:serach for gnome-terminal by "which" cmd failed ???
        ===> "xe: use konsole for shell terminal" �������Ă���Ζ��Ȃ��B
             �����łȂ���� gnome-terminal �� konsole �𓱓�����B

    (5) Gdk-WARNING **: gdk_property_get(): length value has wrapped in calculation (did you pass G_MAXLONG)
        ===> ����.
             (imlib call gdk_property_get with length=MAX_INT,callee issue warning length+3>G_MAXLONG,then use G_MAXLONG as length.)

    (6) WARNING **: failed request with status 200
        ===> ����.
             ���R�͕�����Ȃ������Q�̂悤���B

    (7) GnomePrintCupsPlugin-WARNING **: failed iconv dose not support ppd character encoding: ISOLatin1, trying CSISOLatin1
        ===> ����.
             ���R�͕�����Ȃ������Q�̂悤���B

    (8) WARNING ***: Owner of /tmp/xx-username is not the current user
                     Failed to initialize Panel Agent!
        ===> UserID �ԍ� ��ύX�����B �\�����ꂽ�t�H���_�[���폜�B
             �� UserID�� /tmp/scim-panel-socket-username... ���폜�B

    (9) GnomePrint-CRITICAL ... assertion face != NULL failed
        ===> ����t�H���g���Ƀt�F�C�X��(Regular,Bold,Italic �Ȃ�) �������Ă���B
             xe�͍ŏ���ʃt�H���g���������t�H���g����ݒ肷�邪xe�͂��̃P�[�X�̎�Regular��⊮����̂�
             �ȍ~�͏o�Ȃ��͂��B

    (10) xe help command ���s
         (MIME �^�C�v text/html�ɏȗ����A�N�V����(�u���E�U�[�̋N��)����`����Ă��Ȃ��B
          Gnome �f�X�N�g�b�v�̏ꍇ����� /usr/share/mime-info/gnome-vfs-keys �ɂ���)
        ===> install desktop-file-utils
             /usr/share/applications/defaults.list-->/etc/gnome/defaults.list is installed.

    (11) Gtk WARNING : Cannot open display   (Debian 4.0 when started from console)
        confirm  xauth("apt-get install xauth" on Debian9.3) is installed
        (check also environment variable DISPLAY= on remote)
        chk ssh option "ssh -X"
        X11Forwarding=yes on ssh.config(local)/sshd.config(remote)

    (12) Gtk WARNING : Locale not supported by C library at debian/390
        ===>"setlocale" �����s����ꍇ locale ��ǉ�����B
                 "locale -a" �Ŏg�p�\��locale ���`�F�b�N�A���X�g�ɂȂ����
                 "dpkg-reconfigure locales"

    (13)��������(debian/390)
        ===>unifont �𓱓�
                "aptitude install unifont"

    (14)Gconf err, scim failed to load frontend module
        ===>root���[�U�[�� gxe ���N�����Ă���B������ /root/gconf(d) ���Ȃ��B
            "su" �ł͂Ȃ� "su -"  ��root�ɂȂ�Bsudo �Ȃ� "sudo -i"

    (15)"(�X�[�p�[���[�U��)" ���^�C�g���ɏo��B
        s390x�� "ssh -X" ���� X-appl���N���������B
        ===>�����B������root�ɂȂ��Ă��Ȃ��B
            metacity �Ƃ����p�b�P�[�W���o���Ă���炵�����AX-�T�[�o�[(local����daemon�j��
            root ������ł͂Ȃ����Ǝv���B

    (16)ssh �� X-APPL �ŕ��������B(s390x)
        ssh�̃��P�[���� /etc/ssh/ssh(d).conf �� AcceptEnv/SendEnv�� local �̃��P�[���� 
        �p�����邱�Ƃ��o���Assh��͓��{��\������邪�A
        Xappl�p�ɂ͓������K�v�炵��
        ===> yum install "@Japanese Support" ���邢�� yum groupinstall "Japanese Support"

    (17)"Gtk WARNING ** cannnot open display"
        ==> "export DISPLAY=localhost:10.0"   (10 may be 11, 12..., �����[�g��sshd_config:X11DisplayOffset(�ȗ��l:10)���m�F)
        "su" ����Ƃł�B�ʏ�� DISPLAY �� ssh �������Ŋ��蓖�Ă�B
        �ʏ�DISPLAY��ssh�����䂷��̂ŕK�v�Ȃ��͂�����
        �����[�g��xauth �͓����ς݂�?

(C) FC11.s390x �A�b�v�O���[�h�g���u���V���[�e�B���O

 !!! (E)-FC14 �̕����V�����̂ł���������ĉ����� !!!

    FC11�����ς݂�DASD�C���[�W(http://secondary.fedoraproject.org/pub/alt/spins/S390/)
    ���g�p���K�v�ȃp�b�P�[�W�𓱓�����B
            �Q��url       http://katzkichi-katzkichi.blogspot.com/2010/01/linux.html   (���{��y�[�W)
            pkg-download  //s390.koji.fedoraproject.org/koji

    (1) yum -y install libgnomeprint22-devel.s390x ("yum upgrade" �̃v���e�X�g)
          --> UnicodeDecodeError: 'ascii' codec can't decode byte 0xe5 in position 154: ordinal not in range(128)
              ==> �V�K�t�@�C���쐬
                      /usr/lib/python2.6/site-packages/sitecustomize.py
                         import sys
                         sys.setdefaultencoding("utf-8")
          (yum install)
          --> Destination Host Prohibit
              ==> firewall ����
                      "iptables -F"
          (yum install)
          --> ERROR with rpm_check_debug vs depsolve
              //..koji..���� xz 4.999.8-0.7.beta �� rpm 4.7.1-2 ��T��debuginfo�ȊO�͓����y�[�W�̂���rpm���_�E�����[�h��
              ��������B(scp �� FC11��Up����,ssh�œ���rpm����)
                scp fnm root@192.168.200.3:/root
                xz-libs:  rpm  -ivh   rpm*.rpm
                rpm    :  rpm  -Uvh   xz*.rpm
    (2) yum upgrade
          --->
             createrepo-0.9.8-2.fc12.noarch from fedora has depsolving problems
               --> Missing Dependency: python-deltarpm is needed by package createrepo-0.9.8-2.fc12.noarch (fedora)
             system-config-network-tui-1.5.99-1.fc12.noarch from fedora has depsolving problems
               --> Missing Dependency: python-iwlib is needed by package system-config-network-tui-1.5.99-1.fc12.noarch (fedora)
             Error: Missing Dependency: python-iwlib is needed by package system-config-network-tui-1.5.99-1.fc12.noarch (fedora)
             Error: Missing Dependency: python-deltarpm is needed by package createrepo-0.9.8-2.fc12.noarch (fedora)
              You could try using --skip-broken to work around the problem
              You could try running: package-cleanup --problems
                                     package-cleanup --dupes
                                     rpm -Va --nofiles --nodigest

        ===>yum install deltarpm
        ===>iwlib �����B //..koji.. ���� rpm install
        ---> libiw, wireless-tools required.
        ===>yum install wiress-tools
        (yum upgrade�͐����Ԃ�������(core4))

    (3) ���X�^�[�g

        Hercules �R���\�[���ł� kernel �I�� �� new(FC12) ��I��
        --->"No root device" ��boot�o�����B===>give-up
        old(FC11)��I��
        --->CTC �G���[
        ===>/etc/rc.sysinit �� 3�s(@@@�̍s)�ǉ� (upgrade�O�ɂ͂�������upgrade�Ŏ���ꂽ) 
                # /bin/bash
                #
                # /etc/rc.d/rc.sysinit - run once at boot time
                #
                # Taken in part from Miquel van Smoorenburg's bcheckrc.
                #

                HOSTNAME=`/bin/hostname`

                set -m

                if   -f /etc/sysconfig/network !; then
                    . /etc/sysconfig/network
                fi
                if   -z "$HOSTNAME" -o "$HOSTNAME" = "(none)" !; then
                    HOSTNAME=localhost
                fi

            @@@ modprobe ctcm
            @@@ echo "0.0.0600,0.0.0601" > /sys/bus/ccwgroup/drivers/ctcm/group
            @@@ echo 1 > /sys/bus/ccwgroup/drivers/ctcm/0.0.0600/online
        (restart)
        --->"udevd error geting buffer for inotify"
        ===>yum -Uvh *udev*145-14* (release-7����X�V)
        --->Completed!   

(D) sshfs �̓���

   .sshfs ���p�b�P�[�W�}�l�[�W�����g���ē�������B
   .fusermount�Ɏ��s���������邩�m�F����A�Ȃ���� chmod +x /usr/bin/fusermount. 
   .�}�E���g�|�C���g�� 777 �� ���  (mkdir /mountpoint; chmod 777 /mountpoint)
   .�g�p���郆�[�U�[�h�c�� �O���[�v fuse �̃����o�[�ɂ���Breboot ���K�v.
   ./dev/fuse�̃I�[�i�[�O���[�v��fuse�ɂȂ��Ă��邩�m�F�A�����łȂ���� chgrp fuse /dev/fuse�B 

   �g�p�@:
     sshfs [-o uid=nnn] [-o gid=nnn] user@remotehost:/remotedir /mountpoint
   
     Windows�ł�Dokan sshfs �� GUI�Ńh���C�u�h�c�����蓖�Ă�悤�ɂȂ��Ă���̂ŁB
     "e N:\"�̂悤�ɃA�N�Z�X����B

(E) �C���X�g�[�����O�Ffc14.s390x           2011/11/10
   00). (Linux)
        -IPL�C���[�W�� "fedora-14-s390x-20100925"
         (fedora-14-s390x.img �̓T�C�Y������������DiskFull�ɂȂ�) 
        -Herclese �� "hercules-3.07-1.i686.rpm"
        -"hercles.cnf" �̏C��
          0120 3390 image-file-name
          (000C 3505 files(generic.prm,kernel..) �� IPL 120 �ł͎g�p���Ȃ�)
        -hosts�o�^("/etc/hosts")
           192.168.200.3 s390x
        	
   01). (s390x)
        #adduser useruser
        #asswd  useruser
   02). (s390x)
        -DNS �T�[�o�[�C��("/etc/resolv.conf")
          search example.com
          nameserver xxx.xxx.xxx.xxx 
          nameserver yyy.yyy.yyy.yyy    <--if secondary exists
            (/etc/resolv.conf �� IPL �Ō��ɖ߂�
             �Œ肷��ꍇ /etc/sysconfig/network-scripts/ifcfg-ctc0 ���C��
               DNS1=xxx.xxx.xxx.xxx
               DNS2=yyy.yyy.yyy.yyy
            )
        -ssh��X�T�[�o�[�ݒ�("/etc/ssh/sshd_config")
          X11Forwarding yes
   03). (s390x)
        -yum ���|�W�g���[�C��(http://fedoraproject.org/wiki/Architectures/s390x�̋L�q�ɏ]��)
          [fedora]
          name=Fedora $releasever - $basearch
          baseurl=http://s390.koji.fedoraproject.org/mash/rawhide/s390x/os/
          enabled=1
          gpgcheck=0
   ==> yum ���s,ping �� "host prohibit"
   04). (Linux)
        -iptable�� REJECT �w�������
          #iptables -S         ->�G���g���[�ԍ��̊m�F
          #iptables -D INPUT n1  (n1 �� INPUT �`�F�C���̃G���g���[�ԍ�(1����n�܂�))
          #iptables -D FORWARD n2  (n2 �� FORWARD�`�F�C���̃G���g���[�ԍ�)
          #iptables -S         ->�폜�̊m�F
   05). (Linux)
        -gxe-vvv-tar.gz �� s390 �ɑ���
		  scp $SRCPATH/gxe-vvv.tar.gz useruser@s390x:gxe-vvv.tar.gz
   06). (s390x)
        -tgz��W�J��configure
          $tar -zxvf gxe-vvv.tar.gz        �i/home/useruser�� �Ɖ���j
          $cd  gxe-vvv
          $./configure
   ==> no acceptable C compiler
        -C �̓���
          #yum install gcc.s390x
   ==> term.h not found
        -ncurses�̓���
          #yum install ncurses-devel.s390x
   ==> yum WARNING: refresh-packagekit" inport failed
          #yum install PackageKit-yum-plugin.s390x
   ==> cups/cups.h not found
        -cups�̓���
          #yum install cups-devel.s390x
   ==> no package libgnomeui,gnome-vfs-module,libgnomeprint,libgnomeprintui
        -���ꂼ��lib�𓱓�
          #yum install libgnomeui-devel.s390x
          #yum install libgnomeprintui22-devel.s390x
          (�������x�� yum ���n���O������, #yum-complete-transaction)
   06). (s390x)
        -make
   ==> unknown type name ppd_file_t
        -cups/cups.h �� ppd.h�� #include ���ĂȂ��iBug��)
        -gxe's xxecsub2 �F�����I�� ppd.h ��#include ����
   ==> ld fails dlsym@@GLIBC_2.2...
        -ld �̎g�p�� fc13 ����ύX�ɂȂ���
         2.so of "o.o"-->"1.so"-->"2.so" �̃P�[�X�� "2.so" �𖾎��I��link���Ȃ���΂Ȃ�Ȃ�
        -gxe�� Makefile �C�� (-ldl, -lX11)
   ==> WARNING:unused but set
        -gcc4.6 ����̃I�v�V����(-Wunused-but-set-variable:�ȗ��l)
        -configure.in�C����(gcc �̃o�[�W����>=4.6�̂Ƃ�-Wno-unused-but-set ���w��
         �K�v�Ȃ� "./configure --enable-unused-but-set=yes" ��configure ���Ă�������
   07). (Linux)
        -gxe�̃e�X�g
   ==> cannot open display:
        #yum install xorg-x11-xauth.s390x
        (linux�ł�xhost�R�}���h s390x �ł� DISPLAY=�ݒ�� ssh �̏ꍇ�s�v)
   ==> ���{�ꂪ�\������Ȃ�
        #yum groupinstall "Japanese Support"
   ==> GConf WARNING client failed to connect to the D-BUS deaemon
        #yum install dbus-x11.s390x
   ==> failed to load module pk-gtk-module
        #yum install PackageKit-gtk-module.s390x
   ==> xe: search for gnome-terminal failed
        #yum install gnome-terminal.s390x
   ==> IPP request failed with status 1280
        -libgnomeprint �� CUPS�|�[�����O�����p�\�ȃv�����^�[�Ȃ��Ŏ��s
        -����͖�������
   ==> �|�b�v�A�b�v�_�C�A���O:An error occurred while loading or saving configuration information.
        -���[�g���[�U�[�̂Ƃ��ɏo��A"su" �o�͂Ȃ� "su -"���g��
   ==> GnomeUI-Warning:While connecting to session manager:None of authentication protocols specified are supported.
        -���[�g���[�U�[�̂Ƃ��ɏo��A"su" �o�͂Ȃ� "su -"���g��
   ==> Gtk-Message: Failed to load module "gnomebreakpad"
        -yum install bug-buddy (/usr/lib64/gtk-2.0/libgnomebreakpad)
        ���� bug-buddy ���Ȃ���Ζ����B(�o�O���|�[�g�p)

(F) Ubunto11.10_x64 �C���X�g�[���e�X�g      2011/11/21
   make
   ==> undefined symbol gnome_vfs_mime_get_default...
        libgnomevfs2-extra ���C���X�g�[��
   ==> dlopen@@GLIBC_2.1 undefined 
        �������������� MAkefile �� LDFLAG �𒲐����Ă�������("-ldl" �Ȃ�)
   gxe ���s
   ==> Gtk-WARNING: Funable to locate theme engine in gtk-modules "pixbuf"
        "aptitude install gtk-engine-pixbuf"

(G) OpenSuse12.1_x64 �C���X�g�[���e�X�g 2011/11/22
	cups-devel, libgnomeui-devel, libgnomeprintui-devel �𓱓�
    (DVD ���� os �𓱓��� ���|�W�g���[���X�V:"download.opensuse.org/distribution/12.1/repo/oss/suse")

(H) Deb Debian jessie 3.10 xfce �C���X�g�[���e�X�g 2014/02/14
    xfce4-terminal
    	�V���[�g�J�b�g�L�[�ύX F1=�w���v, F11=�S���, F10=���j���[
        	xfce4-appearance-settings�����s�A �ݒ�, "���j���[�̃V���[�g�J�b�g�L�[��ύX�\�ɂ���" ���`�F�b�N
        	xfce4-appearance-settings�����s�A �ݒ�, "���j���[�̃V���[�g�J�b�g�L�[��ύX�\�ɂ���" ���`�F�b�N
        	xfce4-terminal �̃��j���[��
            	�w���v-->�ڎ�("F1" ���\������Ă���)���j���[���ڂ̏��"Del"�L�[������
            	�\��-->�S��ʕ\��("F11"���\������Ă���)���j���[���ڏ��"Del"������
                (���̑���� ~/.config/xfce4/terminal/accels.scm ���쐬s���)
                �ҏW-->�ݒ�(E)-->�㋉��(V), "���j���[�V���[�g�J�b�g�L�[�𖳌��ɂ���"���I���ɂ���
	WARNING **: Couldn't register with accessibility bus: Did not receive a reply. Possible causes include: the remote application did not send a reply, the message bus security policy blocked the reply, the reply timeout expired, or the network connection was broken.
            -->�ǂ����� export NO_AT_BRIDGE=1 �Ŋ��ϐ���ݒ肷��

    Gtk-WARNING **: Calling IsInhibited failed: GDBus.Error:org.freedesktop.DBus.Error.ServiceUnknown: The name org.gnome.SessionManager was not provided by any .service files
            -->���Q�Ȃ̂Ŗ�������
(I) Rspberry PI  2020/05/16
   configure �G�~�����[�^�[�Ńe�X�g���܂����iimage:"2020-02-13-raspbian-full" on QEMU3.1.0�j
     ./configure �ňȉ��̃G���[������܂���
        term.h not found
        -->#apt-get install libncurses-dev
        cups/cups.h not found
        -->#apt-get install libcups2-dev
        install GTK2 or GTK3
        -->#apt-get install libgtk-3-dev
        select libgnome2 or glib-2.0
        -->#apt-get install glib-2.0
        ==>./configure ����
