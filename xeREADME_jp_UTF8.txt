||*CID:||+129BR~:  2017/06/24                update#=  797;           ||+129BR~
######################################################################
[Japanese]    v1.29B                                                  ||+129BR~

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
