======================================================================
                  Large Vocabulary Continuous Speech
                          Recognition Engine

                                Julius

						(Rev 4.5   2019/01/02)
						(Rev 4.4.2 2016/09/12)
						(Rev 4.4   2016/08/30)
                                                (Rev 4.3.1 2014/01/15)
                                                (Rev 4.3   2013/12/25)
                                                (Rev 4.2.3 2013/06/30)
                                                (Rev 4.2.2 2012/08/01)
                                                (Rev 4.2.1 2011/12/25)
                                                (Rev 4.2   2011/05/01)
                                                (Rev 4.1.5 2010/06/04)
                                                (Rev 4.1   2008/10/03)
                                                (Rev 4.0.2 2008/05/27)
                                                (Rev 4.0   2007/12/19)
                                                (Rev 3.5.3 2006/12/29)
                                                (Rev 3.4.2 2004/04/30)
                                                (Rev 2.0   1999/02/20)
                                                (Rev 1.0   1998/02/20)

 Copyright (c) 1991-2019 ���s��w �͌�������
 Copyright (c) 1997-2000 ��񏈗��U�����Ƌ���(IPA)
 Copyright (c) 2000-2005 �ޗǐ�[�Ȋw�Z�p��w�@��w ���쌤����
 Copyright (c) 2005-2019 ���É��H�Ƒ�w Julius�J���`�[��
 All rights reserved
======================================================================

Julius �ɂ���
=================

Julius �́C�����F���V�X�e���̊J���E�����̂��߂̃I�[�v���\�[�X�̍����\
�Ȕėp���b�A�������F���G���W���ł��D������b�̘A�������F������ʂ�PC
��łقڎ����ԂŎ��s�ł��܂��D�܂��C�����ėp���������C���������⌾�ꃂ
�f���E�������f���Ȃǂ̉����F���̊e���W���[����g�ݑւ��邱�ƂŁC�l�X��
���L���p�r�ɉ��p�ł��܂��D ����v���b�g�t�H�[���� Linux, Windows, iOS,
Android, ���̑��̊��ł��D


GitHub �ւ̈ڍs�ɂ���
========================

Julius��2016�N��� GitHub �ֈڍs���܂����D
�ŐV�̃\�[�X�R�[�h�E�e����s�L�b�g�E�J�����̌��J�E���L�����
�J���Ҍ����̃t�H�[�����^�c�� GitHub �ɂčs���Ă��܂��D

        Julius on GitHub
        https://github.com/julius-speech/julius

���z�[���y�[�W�ɂ� 4.3.1 �ȑO�̏�񂪌f�ڂ���Ă��܂��D
������������p�������D

        �� Julius Web �T�C�g
        http://julius.osdn.jp/


What's new in Julius-4.5
==========================

VAD�̋����̂��߂� WebRTC �x�[�X�� VAD �A���S���Y�����ǉ�����܂����B
�������ꂽ�͈̂ȉ��̃R�[�h�ł��B

  https://github.com/dpirch/libfvad

4.5�ȍ~��Julius�ɂ�2��VAD���W���[��������܂��B�P�͏]�����炠��U
���ƃ[���������x�[�X�̃��W���[���A�����ЂƂ�4.5�œ������ꂽ libfvad
�i���f���x�[�X�j�B�����W���[���͓����I�[�f�B�I���͂ɑ΂��ĕ��񂵂ē���
���A���񓮍쎞�́u�����W���[���Ƃ��g���K�����m�����Ƃ��v�������͂����m
���܂��B�V���W���[���̓f�t�H���g�ł� OFF �ŁA�I�v�V���� "-fvad �l" ��
�L���ɂȂ�܂��B

DNN-HMM�̌v�Z��CPU�}���`�X���b�h���ǉ�����܂����B�}���`�X���b�h��L��
�ɂ��邱�Ƃő�K�͂�DNN�ł̌v�Z���Ԃ������팸����܂��B�X���b�h����
dnnconf ���� "num_threads" �Ŏw�肵�܂��B�f�t�H���g�l�� 2 �ł��B

���W���[�����[�h��XML�`���o�͂� XML special character �̃G�X�P�[�v��
�s���悤�ɂȂ�܂����B�]���o�[�W�������� "<s>", "</s>" ���̏o�͂�
"&lt;s&gt;" �̂悤�ɕς���Ă��܂��̂ł����ӂ��������B�]���̓����
�߂������ꍇ�� "-noxmlescape" ���w�肵�ĉ������B

�S�Ă̕ύX�_�Ǝg�����ɂ��Ă� Release-ja.txt ���������������B


UTF-8�ւ̈ڍs�ɂ���
======================

�e�L�X�g�G���R�[�f�B���O�Ƃ��� SJIS�� EUC �����݂��Ă��܂������A
�o�[�W����4.5����ȍ~�A�\�[�X�R�[�h�̃e�L�X�g�G���R�[�f�B���O��
UTF-8�ɕϊ�����܂����B�ȍ~�̍X�V�� UTF-8 �x�[�X�ōs���܂��B

�R�[�h�̕ύX��ǂ�����ȑO�̃o�[�W�����Ƃ̍������`�F�b�N���₷���悤�A
�o�[�W����4.5�̎��_�ł̃e�L�X�g�G���R�[�h�ϊ��O�̃R�[�h��
"master-4.5-legacy" �u�����`�ŕۑ����Ă���܂��B4.5 �����[�X�ȑO��
�R�[�h���� 4.5 �܂ł̍���������ꍇ�͂�����̃u�����`�� checkout ����
���������B


Julius-4.5�̃t�@�C���̍\��
=============================

	00readme-ja.txt		�ŏ��ɓǂޕ����i���̃t�@�C���j
	LICENSE.txt		���C�Z���X����
	Release-ja.txt		�����[�X�m�[�g/�ύX����
	00readme-DNN.txt	DNN-HMM �̎g��������
	configure		configure�X�N���v�g
	configure.in		
	Sample.jconf		jconf �ݒ�t�@�C���T���v��
	Sample.dnnconf		DNN �ݒ�t�@�C���̃T���v��
	julius/			Julius �\�[�X
	libjulius/		JuliusLib �R�A�G���W�����C�u���� �\�[�X
	libsent/		JuliusLib �ėp���C�u���� �\�[�X
	adinrec/		�^���c�[�� adinrec
	adintool/		�����^��/����M�c�[�� adintool
	generate-ngram/		N-gram�������c�[��
	gramtools/		���@�쐬�c�[���Q
	jcontrol/		�T���v���l�b�g���[�N�N���C�A���g jcontrol
	mkbingram/		�o�C�i��N-gram�쐬�c�[�� mkbingram
	mkbinhmm/		�o�C�i��HMM�쐬�c�[�� mkbinhmm
	mkgshmm/		GMS�p�������f���ϊ��c�[�� mkgshmm
	mkss/			�m�C�Y���σX�y�N�g���Z�o�c�[�� mkss
	support/		�J���p�X�N���v�g
	jclient-perl/		A simple perl version of module mode client
	plugin/			�v���O�C���\�[�X�R�[�h�̃T���v���Ǝd�l����
	man/			�}�j���A����
	msvc/			Microsoft Visual Studio 2013 �p�t�@�C��
	dnntools/		Sample programs for dnn and vecnet client
	binlm2arpa/		�o�C�i��N-gram����ARPA�ւ̕ϊ��c�[��


���C�Z���X
===========

Julius �̓I�[�v���\�[�X�\�t�g�E�F�A�ł��D
�w�p�p�r�E���p���܂߁C���p�Ɋւ��ē��ɐ����͂���܂���D
���p�����ɂ��ẮC�����̕��� "LICENSE.txt" �����ǂ݉������D

�܂��ȉ��̃t�@�C����f�B���N�g������ Copyright �����Q�Ɖ������B

  libjulius/libfvad/
  gramtools/gram2sapixml/gram2sapixml.pl.in
  libsent/src/wav2mfcc/wav2mfcc-*.c
  libsent/src/adin/pa/
  msvc/portaudio/
  msvc/zlib/


�A����
===========

Julius �J���Ɋւ��邲����E���₢���킹�� GitHub �ŏ����Ă���܂��B

        Julius on GitHub
        https://github.com/julius-speech/julius

���邢�͉��L�̃��[���A�h���X�܂ł��₢���킹������
('at' �� '@' �ɓǂݑւ��Ă�������)

	julius-info at lists.sourceforge.jp

�ȏ�
