||*CID:||+129FR~:  2018/01/23                update#=  804;           ||+129FR~
######################################################################
[Japanese]    v1.29F                                                  ||+129FR~

���C���t���[��(SPF�t�@�C���̕ҏW�ɂ��֗�) �� PC �� �����d�����Ă���l�Ɏg���Ղ��G�f�B�^�[�B
�z�X�g��SPF���x�[�X��PC��EDITOR�֗̕��ȃL�[������n�C�u���b�h�B

    .Windows�ŁALinux�ł���
    .���s�R�[�h�Ȃ��̌Œ蒷���R�[�h/�ϒ��t�@�C���T�|�[�g�B
    .UTF8�t�@�C���AEBCDIC(ICU�̓������K�v)�t�@�C���ҏW�B
    .�o�C�i���[�G�f�B�^�[(�c2�iHEX����HEX�\���j
    .�t�@�C���[(�t�H���_�[�\���A�폜�A�����A���ʁA���s...)
    .�����[�g�A�N�Z�X�B
       ftp,samba,rsh,ssh,fuse
    .�I�v�V�����ŕύX�s�ɏC���^�O�������t�^�B

  ���C�Z���X:GNU GPL �ɏ]���B

                                   By �����}�` (sakachin2@yahoo.co.jp)

                                   http://hp.vector.co.jp/authors/VA010562
                                   http://www.geocities.jp/sakachin2/index.htm
                                   GitHub: sakachin2/XE

WIN�ł�GUI�ł�WIN32�R���\�[���A�v���P�[�V�����ł�����܂��B
   Console��:xe.exe �̓R�}���h�v�����v�g�œ����}�E�X�̓T�|�[�g���Ă��܂���B
   GUI��:wxe.exe ��WTL/ATL��(MFC�s�g�p)��vs2010Express�ŃR���p�C���������̂ł�
   w64binGit.zip����
Linux�ł�GUI��:gxe ��TerminalEmulator��:xe ������܂��B
   gxe-x.xx.tar.gz �� �𓀂� ./configure && make �ŃC���X�g�[��
�ȉ��̃R���\�[���Ńc�[�����܂܂�Ă��܂�
   xads         (Win�ł̂�)NTFS�t�@�C���V�X�e����ADS(Alternative Data Stream)�A�N�Z�X�B
   xbc          �ȈՌv�Z�c�[���B
   xci          C/C++/Java�e�L�X�g�t�@�C���̃C���f���e�[�V����
   xcv          �R�[�h�ϊ��c�[���B(SJIS,EUC,Unicode,UTF-8,EBCDIC,�C�ӂ̃R�[�h�y�[�W)
   xcvsjisc     �\�[�X�t�@�C������SJIS�R�[�h���W�i�\�L�ɕϊ�����B
   xdc          �f�B���N�g���[��r�c�[��
   xdd          �f�B���N�g���[�폜�c�[��
   xdig         �f�B���N�g���[�E�H�[�N�c�[��
                �f�B���N�g���[���̑S�T�u�f�B���N�g���[/�t�@�C���Ɏw���
                �R�}���h����p������v���O����.
   xds          �f�B���N�g���[�T�C�Y�\���c�[��
   xfc          �t�@�C����r�c�[��
   xff          �T�C�Y�A�^�C���X�^���v�ɂ��t�@�C���T�[�`
   xfg          �e�L�X�g/�o�C�i���|(Recursive)�t�@�C��������T��
   xfmt         �t�@�C���t�B�[���h�t�H�[�}�b�^�[
   xfs          �t�@�C���̕���/����.�傫�ȃt�@�C���̃f�B�X�P�b�g�ւ�
                �o�b�N�A�b�v/���X�g�A�[�Ɏg���܂�
   xkp          (WIN)�v���Z�XID�̕\���ƃv���Z�X��kill
   xlow         �啶���t�@�C�������������ɉ����B
   xmj          2 �t�@�C���}�b�`���O�B
   xpe          errno(libc�̃G���[�ԍ�)�̐�����\������B
   xts          �t�@�C���̃^�C���X�^���v�̕\��/�ύX
   xver         OS�o�[�W��������ERRORLEVEL��ݒ�

   xprint       �e�L�X�g�t�@�C���v�����g���[�e�B���e�B
   gxp          Linux GTKPrint�� xprint


���̑��̃t�H���_�[�̓��e
  xehelp:
    Browser�p�w���v�t�@�C��
    ���[�N�f�B���N�g���[�ɒu�����Axehelp���ϐ�
    ���邢��/hd�R�}���h���C���p�����[�^�ňʒu�w�肷��B
    Linux�łł̂���ȊO�̒u���ꏊ��xelnxj.txt���Q�Ƃ��Ă�������
  sample\doc:
    �e�L�X�g�t�@�C���`���̃}�j���A��
      xej.txt/xee.txt
      xereadmj.txt/xereadme.txt
      xelnxj.txt/xelnxe.txt(Linux�ŗp)
      xewxej.txt/xewxee.txt(GUI��:wxe/gxe�p)
  sample\data:
      xehosts      �����[�g�t�@�C���A�N�Z�X�p�T���v���z�X�c�t�@�C���B
      xesynw.cfg   (Win)�V���^�b�N�X�n�C���C�g�p�ݒ�t�@�C���B
      xeebc.map    EBCDIC �ϊ��p�ݒ�t�@�C��

  sample\staff:�O���c�[����p�ӂł��Ȃ��ꍇ�͈ȉ��̂��̂����g����������

      grep.exe     �R�}���h�s�� GREp �R�}���h�A=3.14 ��ʂŎg�p���܂�

      �V���^�b�N�X�n�C���C�g�Ŏg�p���܂��A���̂ǂ��炩��I��� xesynw.cfg �Ŏw�肵�܂�
        �g������ xej.txt �� xesynw.cfg �����Ă�������
        gnu-source-highlight.zip
                     (Win)GNU source-highlight v2.9 �� MinGW��ŃR���p�C�����܂����B
        WinHighlight31.copies2.zip
                     andre simon's highlight v3.1
                     exe �� dll �̃t�H���_�[�𗣂��Ȃ��ł�������
      putty063.zip
                     �����[�g�A�N�Z�X�� putty ���g�p����ꍇ�ɕK�v�ł�


�N�����@

  (Windows��)

  �D���[�N�t�H���_�[���쐬����A�ȗ��l��c:\xe_wd���� c:\�͕ی삳��Ă���\��������̂Ŕ����Ă�������
    �Ⴆ��  "mkdir d:\xe_wd"
  �D���[�N�t�H���_�[�� zip�t�@�C����u��,�����ŉ𓀂���
      �K�v�ɉ����� sample\data �t�H���_�[����xehosts �Ȃǂ̐ݒ�p�t�@�C�������[�N�t�H���_�[�ɃR�s�[���C�����Ă�������
      �����̋@�\���g�p���Ȃ��ꍇ�� �R�����g�s("#") 1�s�̃t�@�C���ɂ��Ă�������
  . ���s�\�t�@�C���� PATH ��ʂ�.
      Windows10�̏ꍇ�A�R���g���[���p�l��-->�V�X�e���ƃZ�L�����e�B-->�V�X�e��-->�V�X�e���̏ڍאݒ�-->���ϐ�:PATH
  . ���|�N�f�B���N�g���[�������ϐ�:xe �ɃZ�b�g����
      ���邢�� �C�ӂɍ쐬���� xe �N���p�R�}���h�t�@�C�����쐬����
      �Ⴆ�� xe.bat
               set xe=d:\xe010
               xe.exe
            �����
               xe.exe /wd:\xe010
  �Dxe [�t�@�C����] �ŋN������
      �R�}���h���C�� �p�����[�^��  xe /? �ŕ\������܂�
  . wxe �������ł�

  (Linux��)
  .�^�[�~�i���G�~�����[�^�[���J���A�K���ȏꏊ�ŉ𓀂�configure/make/install
      tar -zxvf gxe-1.xx.tar.gz
      cd
      ./configure
      make
      sudo make install   -->/usr/local/bin�ɃC���X�g�[��
    ��肪����������sample�t�H���_�[�� READMEj.txt ���Q�Ƃ��Ă�������
    �K�v�Ȃ�/usr/local/bin�ɃC���X�g�[������Ȃ��R�}���h���C���c�[����
    src/xsub �t�H���_�[����蓮�ŃR�s�[���Ă�������
  .���[�N�t�H���_�[�� home �ɍ쐬
      mkdir ~/xe_wdnnnnn     nnnnn �� ���[�U�[ID�ԍ�
    �K�v�ɉ����� sample �t�H���_�[����xehosts �Ȃǂ̐ݒ�p�t�@�C�������[�N�t�H���_�[�ɃR�s�[���C�����Ă�������
    �����̋@�\���g�p���Ȃ��ꍇ�� �R�����g�s("#") 1�s�̃t�@�C���ɂ��Ă�������
  �Dxe [�t�@�C����] �ŋN������
      �R�}���h���C�� �p�����[�^��  xe -? �ŕ\������܂�
      F1�AF10 �� �C���L�[(Shift/Alt/Ctrl)�Ƃ̑g�ݍ��킹�̓^�[�~�i���G�~�����[�^�[��
      �V���[�g�J�b�g�L�[�ɐݒ肳��Ă���ꍇ������܂�
      xe �� F1�AF10 �Ȃǂ��g�p����ꍇ�^�[�~�i���G�~�����[�^�̐ݒ�ŃV���[�g�J�b�g�𖳌��ɂ���K�v������܂�
  . gxe �̓^�[�~�i���G�~�����[�^�̃V���[�g�J�b�g�L�[�̉e���͂���܂���

######################################################################
�C������.
  .v010 (95/06/04)
        ����                                                          
######################################################################
  .v129A<--129:(2017/06/24)

     1.BUGs
       -(Windows:64)"&"(�o�C�i���[�t�@�C���񓯊����s) �f�B���N�g���[���X�g�R�}���h���N���b�V������
       -(64Bit) =3.14 ���N���b�V������

     3.���̑�
       -(Windows)�g���q:"msi" �����s�\�t�@�C���̊g���q�ɒǉ�

  .v129B<--129A:(2017/07/10)

     1.BUGs

       -(Win64) �f�[�^�^�C�v X(Hex),O(octal) �̌v�Z���ʂ̌��
       -(Win64) ������ʊԂ̃h���b�O�h���b�v(�t�@�C���̃R�s�[)���N���b�V��

     2.�@�\�ǉ�

       -�����p�X���ɒZ�k�����`
        .SP { edit | refresh | add sp-name { file-spec | *\\ | ^*\\ } }
            edit   : ��`�t�@�C��(::xe.shortpath) ��ҏW�\��
                     �C�����ĕۑ�����΁A���񂩂�L���ɂȂ�
                     ���邢�͕ۑ��� "refresh" ����ΗL���ɂȂ�܂�
                     ��`�t�@�C���̊e�s��"�Z�k�� �t���p�X��" �̌`��
                     �R�����g�s�͐擪�� "#"
                     ��) srctest1 d:\eclipse-workspace\testproject1\src\com\debug\test
                         ecws  "c:\Program Files\Android\Android Studio\gradle"
            refresh: ��`�t�@�C�����C�������ꍇ�ɁA���̏C���𔽉f������
                     "sp edit" ��ʂŏC���A�ۑ��� ���邢�͒��� ::xe.shortpath �t�@�C����
                     ���̃v���Z�X�ŏC��������Ɏg�p����
            add    : ��`�t�@�C���� sp-name:�Z�k��, file-spec:�^�[�Q�b�g�t�@�C���� �̍s��ǉ�
                     ���̒�`�͂����g�p�ł���
                     *\ :���݊J���Ă���t�@�C��/�f�B���N�g���[,
                     ^*\:������ʂ̑����Ō��݊J���Ă���t�@�C��/�f�B���N�g���[
                     ���󋵂��K���Ȃ�Ύg�p�ł���
                     ��) sp add srctest1 d:\eclipse-workspace\testproject1\src\com\debug\test
                         sp add ecws  "c:\Program Files\Android\Android Studio\gradle"
        .�Z�k���� "sp:"�v���t�B�b�N�X�Ŏg�p����
         (sp:xxx �� xxx ������`�̏ꍇ�͂��̂܂� "sp:xxx" �Ƃ��Ďg�p�����)
           ��) e sp:srctest1\Main.java
               e sp:ecws
               e "sp:ecws\space embedded name"
               xcopy sp:ecdir\x1 sp.ecdir\x2
               cd sp:ecdir
                                                                      ||~129DI~
  .v129C<--129B:(2017/09/04)                                          ||~129DI~
                                                                      ||~129DI~
     1.BUGs                                                           ||~129DI~
                                                                      ||~129DI~
     2.�@�\�ǉ�                                                       ||~129DI~
       -Find �R�}���h                                                 ||~129DI~
          �f�B���N�g���[���X�g��� ATTR(����)���݂̂�T���I�v�V������ǉ�||~129DI~
          �啶���������̋�ʂ͂��܂���                                ||~129DI~
          �������ɂ͕\������Ă��Ȃ��� �f�B���N�g���[�ɂ� "d"�A�V���{���b�N�����N�ɂ� "L" ���w�肷��||~129DI~
          �܂� "d" �� "L" �͂��ꂼ��P�ƂŎw�肵�Ă�������            ||~129DI~
          ����ȊO�̑����� Windows�ł� �w��̈��̑������ׂĂ��܂ލs����v�s�Ƃ�||~129DI~
          Linux�ł͑����w��̕�������܂ލs����v�s�Ƃ���             ||~129DI~
          Linux�œ���ȑ������̒l��                                   ||~129DI~
            u:setuid, g:setgid, S:setuid+setgid, t:stickey            ||~129DI~
            c:char device, b:block device, p:pipe, s:socket           ||~129DI~
        ��) (Windows) f SH attr ; f R attr & 17-08 ; f D attr & L attr||~129DI~
            (Linux)   f 775 attr ; f u attr                           ||~129DI~
                                                                      ||~129DI~
     3.���̑�                                                         ||~129DI~
       -(Windows)ICU EBCDIC�ϊ����C�u�����[libicuuc.dll��������Ȃ��Ƃ�||~129DI~
        xeebc.map�� ICU_DATA �̎w�肪����΂��̃t�H���_�[�����`�F�b�N����||~129DI~
        �Ȃ���� ���ϐ� ICU_DATA ���`�F�b�N����                     ||~129DI~
        (Linux)/usr/lib �ȂǈȊO�ɂ���ꍇ�� LD_LIBRARY_PATH ���ϐ��� ICU �� so �̃p�X�����Ă��Ă�������||~129DI~
       -xeebc.map �� ICU_DLL_SUFFIX, ICU_APP_SUFFIX �� �Ȃ��Ƃ�       ||~129DI~
        ICU �� uconv(.exe) �� ICU �̃o�[�W������������΂����₤    ||~129DI~
       -CPU8(UTF8)�t�@�C���ł̓��R�[�h���͕s��Ȃ̂�/Mr(���R�[�h���[�h)�I�v�V�����͎󂯕t���Ȃ�||~129DI~
                                                                      ||~129DI~
     4.�c�[���B                                                       ||~129DI~
       -xprint v9.38                                                  ||~129DI~
        ./Tabon: �p�����[�^�T�|�[�g�ǉ�                               ||~129DI~
           DBCS�X�y�[�X�ATAB(0x09)�Ƃ���ɑ������󂯂ɕ\�������֕������w�肷��||~129DI~
           /Tabon:x:y:z ;�e�L�X�g���[�h�̂Ƃ���DBCS�X�y�[�X,�^�u����,�^�u�X�L�b�v��||~129DI~
                        ;��ֈ�������Bx,y,z�� �����A�w�L�T�����܂��̓��j�R�[�h�B||~129DI~
                        ;��) /Tabon:x2020:x18:x1a  /Tabon::u2191:u2192 /Tabon::u25cb||~129DI~
                        ;    /Tabon:u2750                             ||~129DI~
                        ;�ȗ��l�� UTF8/EBCDIC�t�@�C�� /Tabon:u3000:x20:x20||~129DI~
                        ;                        �ȊO /Tabon:x8140:x20:x20||~129DI~
        .EBCDIC �t�@�C���� ICU �ŕϊ����Ĉ������Ƃ��� /BCfilename �̎w�肪�Ȃ��ꍇ||~129DI~
         ICU �� ���L���C�u�����[(DLL �܂��� so)�� PATH �܂��� LD_LIBRARY_PATH �ɂ����||~129DI~
         �T���� ICU �o�[�W������ uconv(.exe) �𔭍s���� �����₤    ||~129DI~
           ��) xprint x1ebc22 -cpeb=cp930 -me -icu                    ||~129DI~
       -xcv 1.20                                                      ||~129DI~
        .EBCDIC �t�@�C���� ICU �ŕϊ�����Ƃ��� /BCfilename �̎w�肪�Ȃ��ꍇ||~129DI~
         ICU �� ���L���C�u�����[(DLL �܂��� so)�� PATH �܂��� LD_LIBRARY_PATH �ɂ����||~129DI~
         �T���� ICU �o�[�W������ uconv(.exe) �𔭍s���� �����₤    ||~129DI~
           ��) xcv x1ebc22 x1ebc22m -b2m -cpeb=cp930 -icu             ||~129DI~
                                                                      ||~129DI~
  .v129D<--129C:(2017/12/03)                                          ||~129DI~
                                                                      ||~129DI~
     1.BUGs                                                           ||~129DI~
       -(Linux)GTK3���̎��Z�b�g�A�b�N�_�C�A���O�ł̃��j���[�A�N�Z�����[�^�[(Ctrl+)�I�v�V������||~129DI~
        �I��/�I�t�������Ȃ�                                           ||~129DI~
       -(Wxe)�t�@�C��-New(�V�K�t�@�C��)�ŃN���b�V��                   ||~129DI~
                                                                      ||~129DI~
     2.�@�\�ǉ�                                                       ||~129DI~
       -SelectAll                                                     ||~129DI~
          .�R�}���h                                                   ||~129DI~
             SEL [all] [col1 col2] [.label1 .label2]                  ||~129DI~
               label1/2 �ōs�͈͎w��Acol1/2 �ŃJ�����͈͎w��         ||~129DI~
               label��1/2�Ƃ������ɂ��s�ԍ��w��ł��悢             ||~129DI~
               col �̎w�肪����ƃu���b�N���[�h�A�Ȃ��Ɨ̈惂�[�h     ||~129DI~
               label/column �̎w�肪�Ȃ��ƑS�I��                      ||~129DI~
               ��jsel; sel .a .b; sel 1 20; sel 10 20 .1 .4;         ||~129DI~
          .Edit��ʂ� �s�I�����ACut/Copy/Paste�ɂȂ��Ă����܂�      ||~129DI~
           �̈惂�[�h�ł͂���Paste �̑Ώۂɂ��Ȃ�܂�                 ||~129DI~
        (Wxe,gxe)                                                     ||~129DI~
          .Edit�T�u���j���[�A�|�b�v�A�b�v���j���[�ɂ� "SelectAll" ���j���[���ڒǉ�||~129DI~
          .�V���[�g�J�b�g��Ctrl+A�ɐݒ� SaveAs(�ʖ��ۑ�)��Ctrl+Shift+A�ɕύX||~129DI~
                                                                      ||~129DI~
     3.���̑�                                                         ||~129DI~
       -File�T�u���j���[�̃��j���[���ڂ���ʂ̏󋵂ɂ���Ă͕s����������||~129DI~
        �Ⴆ�΁A�f�B���N�g���[��ʂł̕ۑ����j���[���ڂȂ�            ||~129DI~
                                                                      ||~129DI~
  .v129E<--129D:(2018/01/09)                                          ||~129DI~||~129ER~
                                                                      ||~129DI~
     1.BUGs                                                           ||~129DI~
                                                                      ||~129EI~
       -Window �R���\�[���ŁF�w�b�_�[�s�̃G���[���b�Z�[�W�������������邱�Ƃ�����||~129EI~
                                                                      ||~129DI~
     2.�@�\�ǉ�                                                       ||~129DI~
       -XML�^�O �y�A�T��                                              ||~129DI~
          .�f�t�H���g�� Alt+"/" �����蓖��                            ||~129DI~
          .�J�[�\���� "<" �܂��� ">" �̈ʒu�ɂ����� "Alt+/" ���g�p    ||~129DI~
          .�R�����g�Ȃ�("<!--" ���� "-->")�͖����A�l�X�g�������A      ||~129DI~
           html ���������c�[���̕s����C������̂ɕ֗��ł�          ||~129DI~
                                                                      ||~129DI~
     3.���̑�                                                         ||~129DI~
                                                                      ||~129DI~
       -Window �R���\�[���ŁFWindows10�ł̓��K�`���[:ON�ɂ���� UTF8 �t�@�C����||~129EI~
        DBCS �\���������ꂷ��̂� Windos7�ȍ~ �R���\�[���łł̓��K�`���[:ON���󂯕t���Ȃ�||~129EI~
                                                                      ||+129FI~
  .v129F<--129E:(2018/01/23)                                          ||+129FI~
                                                                      ||+129FI~
     1.BUGs                                                           ||+129FI~
                                                                      ||+129FI~
       -Edit/Browse �R�}���h                                          ||+129FI~
        .���R�[�h���[�h�Ń��R�[�h�T�C�Y>4096���ŏ��̃��R�[�h�ɐ��䕶��(<0x20)�������||+129FI~
         �Ō�̃��R�[�h�݂̂��\�������B�܂��t�@�C���T�C�Y��128K�����ƃN���b�V������||+129FI~
        .���R�[�h���[�h�̎��v���t�@�C���ɋL�^������CPLC�����������i����CPLC�̎w�肪�K�v�ɂȂ�)||+129FI~
                                                                      ||+129FI~
