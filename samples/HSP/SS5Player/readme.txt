�ESS5Player for HSP
���T�v
	Sprite Studio 5 �ō쐬�����A�j���[�V������HSP�ōĐ�����T���v���v���O�����ł��B
	
	SpriteStudio5-SDK(https://github.com/SpriteStudio/SpriteStudio5-SDK)�Ɋ܂܂��
	Ss5Converter���g�p����sspj����sspb���쐬���܂��B
	
	�쐬����ssbp�Ɖ摜�t�@�C�����Q�[���̃��\�[�X�t�H���_�ɒu��SS5PlayerDll���g�p���ēǂݍ��݂܂��B
	SS5PlayerDll����A�j���[�V�����̃X�e�[�^�X���擾����HSP���ŕ\�����s���܂��B
	
	DLL�����ɂ�32�̃A�j���v���C���[�������Ă���A�v���C���[�ԍ����w�肵�Ċe�v���C���[�𑀍삵�܂��B
	�v���C���[���𑝂₷�ꍇ��SS5PlayerDll.cpp�ɒ�`����Ă���SSPLAYER_MAX��ύX���Ă��������B
	
	���T���v���v���O�����̐���
	���Ή��A�g���r���[�g
	�@X��]�AY��]�A�J���[�u�����h�A���_�ό`�AX�T�C�Y(�o�͂��Ă��邪�T���v���v���O���������Ή�)�AY�T�C�Y(�o�͂��Ă��邪�T���v���v���O���������Ή�)
	�@UXX�ړ��AUVY�ړ��AUV��]�AUXX�X�P�[���AUVY�X�P�[���A���[�U�[�f�[�^�A�C���X�^���X�A�j��
	�T���v���ł̓p�[�c�̃u�����h���@�ɂ͑Ή����Ă��܂���B
	�f�[�^�͏o�͂��Ă���̂ŁA�K�v�ł���Ίe���Ή����Ă��������B

	�T���v���ł�32bit��png���g�p���Ă��܂����A16bit���̉摜���g�p��HSP�̕W�����߂ŕ\������Γ��쑬�x�͊i�i�ɑ����Ȃ�Ǝv���܂��B
	�K�v�ɉ����ăX�e�[�^�X����\�������쐬���Ă��������B

	png�̕\����Artlet2D���g�p���Ă��܂��B

	SS5PlayerDll.dll��Visual Studio Express for Windows Desktop�ō쐬����Ă��܂��B
	�K�v�ɍ��킹��DLL���Ɋ֐���ǉ����Ă��������B

��SS5PlayerDll.dll�֐����t�@�����X

	#cfunc SSPlayer_initlize			"SSPlayer_initlize"
		�E�@�\
			SS5PlayerDll.dll�̏��������܂�
			�g�p�O�ɕK���Ăяo���Ă��������B

		�E����
			�Ȃ�

		�E�߂�l
			���0

	#cfunc SSPlayer_setFps				"SSPlayer_setFps"				int
		�E�@�\
			SSPlayer_update���Ăяo�����Ƃ��ɃA�j�����i�ޑ��x���w�肵�܂��B
			60FPS�œ��삷��ꍇ��60��ݒ肵�Ă��������B

		�E����
			int 	�FFPS

		�E�߂�l
			���0

	#cfunc SSPlayer_addData				"SSPlayer_addData"				str 
		�E�@�\
			ssbp�t�@�C����ǂݍ���DLL�����ɕێ����܂��B
			������ssbp�t�@�C����ǂݍ��ݕێ����邱�Ƃ��ł��܂��B
			���݂��Ȃ��t�@�C�����w�肷��ƃG���[1���������܂��B

		�E����
			str 	�Fssbp�t�@�C���̃p�X

		�E�߂�l
			���0

	#cfunc SSPlayer_getPlayerNum		"SSPlayer_getPlayerNum"		 
		�E�@�\
			DLL�œ����ɐ���ł���v���C���[�̐����擾���܂��B
			32�܂œ����ɃA�j�����Đ����鎖���ł��܂��B

		�E����
			�Ȃ�

		�E�߂�l
			�����ɐ���ł���v���C���[��

	#cfunc SSPlayer_get_texureIndex		"SSPlayer_get_texureIndex" 		int
		�E�@�\
			�ǂݍ���sspb�Ŏg�p���Ă���e�N�X�`���ԍ����擾���܂��B
			�e�N�X�`���ԍ���DLL���Ŋ��蓖�Ă��ԍ��ƂȂ�A�`����s���Ƃ��ɂ��̔ԍ��ŕ\������摜�����肵�܂��B
			100���܂Ńe�N�X�`���f�[�^�ɕێ����鎖���ł��A������0�Ԃ��珇�Ƀe�N�X�`���ԍ����擾���Ă��������B
			�e�N�X�`���ԍ���0�Ԃ��犄�蓖��܂��A�擾�����ԍ��̃X�N���[���ɑΉ�����摜��ǂݍ���ł��������B

		�E����
			int 	�FDLL�ŕێ����Ă���e�N�X�`���f�[�^�̔ԍ��i0�`99�j

		�E�߂�l
			�e�N�X�`���Ɋ��蓖�������ԍ��i0�`99�j

	#cfunc SSPlayer_get_texureName		"SSPlayer_get_texureName"		int,sptr
		�E�@�\
			�ǂݍ���sspb�Ŏg�p���Ă���e�N�X�`�������擾���܂��B
			DLL�ŕێ����Ă���e�N�X�`���f�[�^����t�@�C�������擾���܂��B
			100���܂ŕێ����鎖���ł��A������0�Ԃ��珇�Ƀe�N�X�`�������擾���Ă��������B
			SSPlayer_get_texureIndex�Ŏ擾�����ԍ��̃X�N���[����SSPlayer_get_texureName�Ŏ擾�����摜��ǂݍ���ł��������B

		�E����
			int 	�FDLL�ŕێ����Ă���e�N�X�`���f�[�^�̔ԍ��i0�`99�j
			pstr	�F�e�N�X�`���Ɋ��蓖�������t�@�C����

		�E�߂�l
			���0

	#cfunc SSPlayer_play				"SSPlayer_play"					int,str,str 
		�E�@�\
			�A�j���[�V�������Đ����܂��B
			sspb���i�g���q�Ȃ��j��ssae��/���[�V�������Ŏw�肵�܂��B
			���SSPlayer_addData��ssbp��ǂݍ���ł����K�v������܂��B
			�w�肵��ssbp��DLL�ɓǂݍ��܂�Ă��Ȃ��ꍇ�A�G���[�P���������܂��B
			�Đ�����SSPlayer_play���Ăяo�����ƂŁA�����v���C���[�ŕʂ̃A�j�����Đ����鎖���ł��܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			str		�Fssbp���i�g���q�Ȃ��j
			str		�Fssae��/���[�V�������i�Ԃ�/�����Ďw�肵�Ă��������B�j

		�E�߂�l
			���0

	#cfunc SSPlayer_update				"SSPlayer_update"			 
		�E�@�\
			DLL�ŕێ����Ă���32�̃v���C���[�̃X�e�[�^�X���X�V���܂��B
			SSPlayer_update���SSPlayer_get_partStatus�Ńp�[�c�̃X�e�[�^�X���擾���A
			�X�e�[�^�X�̓��e�ŕ`����s���̂���{�̗���ɂȂ�܂��B

		�E����
			�Ȃ�

		�E�߂�l
			���0

	#cfunc SSPlayer_get_partNum			"SSPlayer_get_partNum"			int 
		�E�@�\
			�A�j���Ɋ܂܂��p�[�c�����擾���܂��B
			�p�[�c���̓p�[�c�X�e�[�^�X���擾����ꍇ�Ɏg�p���܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j

		�E�߂�l
			�A�j���Ɋ܂܂��p�[�c��

	#cfunc SSPlayer_get_partStatus		"SSPlayer_get_partStatus"		int,int,var 
		�E�@�\
			�p�[�c�̃X�e�[�^�X���擾���܂��B
			�p�[�c�͗D��x���Ƀ\�[�g����Ă���A0�Ԃ̃p�[�c����ԉ��ɂȂ�܂��B
			SSPlayer_get_partNum�Ŏ擾�����p�[�c�������[�v���ăX�e�[�^�X���擾���Ă��������B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			int 	�F�p�[�c�ԍ�
			var		�F�X�e�[�^�X���󂯎��z��̃|�C���^�idim partstate, 18�j
						 0�F�e�N�X�`���ԍ�
						 1�F��\���t���O
						 2�F�\���ʒuX
						 3�F�\���ʒuY
						 4�F�e�N�X�`�����̊J�n�ʒuX
						 5�F�e�N�X�`�����̊J�n�ʒuY
						 6�F�摜�̕�
						 7�F�摜�̍���
						 8�F�g�嗦X
						 9�F�g�嗦Y
						10�F��]�p�x
						11�F�����x
						12�F�u�����h���[�h
						13�F�����]�t���O
						14�F�c���]�t���O
						15�FX�T�C�Y
						16�FY�T�C�Y
						17�F�����蔼�a

		�E�߂�l
			���0

	#cfunc SSPlayer_setPosition			"SSPlayer_setPosition"			int,int,int 
		�E�@�\
			�v���C���[�̈ʒu��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			int 	�F�\���ʒuX
			int		�F�\���ʒuY

		�E�߂�l
			���0

	#cfunc SSPlayer_setRotation			"SSPlayer_setRotation"			int,double,double,double 
		�E�@�\
			�v���C���[�̉�]��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			double	�FX��]�p�x�i���Ή��ł��������I�ɂ͌v�Z����Ă���̂ŁA0�ȊO��ݒ肷��ƕ\��������܂��j
			double	�FY��]�p�x�i���Ή��ł��������I�ɂ͌v�Z����Ă���̂ŁA0�ȊO��ݒ肷��ƕ\��������܂��j
			double	�FZ��]�p�x�i0�`360�j

		�E�߂�l
			���0

	#cfunc SSPlayer_setScale			"SSPlayer_setScale"				int,double,double 
		�E�@�\
			�v���C���[�̊g�嗦��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			double	�FX�g�嗦�i1.0�����{�j
			double	�FY�g�嗦�i1.0�����{�j

		�E�߂�l
			���0

	#cfunc SSPlayer_setAlpha			"SSPlayer_setAlpha"				int,int 
		�E�@�\
			�v���C���[�̓����x��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			int		�F�����x�i0�`255�j

		�E�߂�l
			���0

	#cfunc SSPlayer_setFlip				"SSPlayer_setFlip"				int,int,int 
		�E�@�\
			�v���C���[�̔��]��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			int		�FX���]�i0���]�Ȃ��A0�ȊO���]�j
			int		�FY���]�i0���]�Ȃ��A0�ȊO���]�j

		�E�߂�l
			���0

	#cfunc SSPlayer_pause				"SSPlayer_pause"				int 
		�E�@�\
			�v���C���[�̃A�j���Đ����ꎞ��~���܂��B
			SSPlayer_pause�ňꎞ��~�����v���C���[��SSPlayer_resume�ōĊJ���鎖���ł��܂��B
			�ꎞ��~��ԂŁASSPlayer_setFrameNo���s���Đ��t���[�����w�肷��ƃQ�[�����ŕ\���t���[�����Ǘ����鎖���ł��܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j

		�E�߂�l
			���0

	#cfunc SSPlayer_resume				"SSPlayer_resume"				int 
		�E�@�\
			�v���C���[�̃A�j���Đ����ĊJ���܂��B
			SSPlayer_pause�ňꎞ��~�����v���C���[��SSPlayer_resume�ōĊJ���鎖���ł��܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j

		�E�߂�l
			���0

	#cfunc SSPlayer_setFrameNo			"SSPlayer_setFrameNo"			int,int 
		�E�@�\
			�A�j���̍Đ��ʒu��ݒ肵�܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			int		�F�Đ����s���t���[��

		�E�߂�l
			���0

	#cfunc SSPlayer_getMaxFrame			"SSPlayer_getMaxFrame"			int 
		�E�@�\
			�A�j���̑��t���[�����擾���܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j

		�E�߂�l
			�A�j���̑��t���[��

	#cfunc SSPlayer_getFrameNo			"SSPlayer_getFrameNo"			int 
		�E�@�\
			���ݍĐ����Ă���t���[�����擾���܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j

		�E�߂�l
			���ݍĐ����Ă���t���[��

	#cfunc SSPlayer_get_namePartStatus	"SSPlayer_get_namePartStatus"	int,str,int,var 
		�E�@�\
			�p�[�c������p�[�c�X�e�[�^�X���擾���܂��B
			�Đ����Ă���A�j���ɑ��݂��Ȃ��p�[�c�������Ă������ꍇ�A�e�N�X�`���ԍ���-1�ɂȂ�܂��B
			���W��T�C�Y���擾���ăG�t�F�N�g���o������R���W�����Ƃ��Ďg�p���l�����܂��B

		�E����
			int		�F�v���C���[�ԍ��i0�`31�j
			str		�F�p�[�c��
			int		�F�擾����t���[���i-1�Ō��݂̃t���[���̃X�e�[�^�X���擾����j
			var		�F�X�e�[�^�X���󂯎��z��̃|�C���^�idim partstate, 18�j

		�E�߂�l
			���0

	#cfunc SSPlayer_Delete				"SSPlayer_Delete"				 
		�E�@�\
			DLL���ŕێ����Ă������������܂��B
			�A�v���P�[�V�����̏I�����ɌĂяo���Ă��������B
			�摜�̉���̓Q�[�����ōs���Ă��������B

		�E����
			�Ȃ�

		�E�߂�l
			���0





