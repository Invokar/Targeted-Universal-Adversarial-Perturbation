# Targeted Universal adversarial perturbations

This repos extended [Universal Adversarial Perturbation](https://github.com/LTS4/universal) to target attack.

Only Python3.x ver included.

*python*: Python3.x code to generate universal perturbations using [TensorFlow](https://github.com/tensorflow/tensorflow).Required library is written `requirements.txt` .

## Usage

### Get started

To get started, you can run the demo code to apply a pre-computed universal perturbation for Inception on the image of your choice
```
python demo_inception.py -i data/test_img.png	
```
This will download the pre-trained model, and show the image without and with universal perturbation with the estimated labels.
In this example, the pre-computed targeted universal perturbation in `data/universal.npy` is used. This Perturbation targeted kit fox class.

### Computing a universal perturbation for your model

To compute a universal perturbation for your model, please follow the same struture as in `demo_inception.py`.
In particular, you should use the `universal_perturbation` function (see `universal_pert.py` for details), with the set of training images 
used to compute the perturbation, as well as the feedforward and gradient functions.

## Targeted Perturbations

precomputing_perturbations directory include some precomputing targeted universal adversarial perturbations.

## Reference
[1] S. Moosavi-Dezfooli\*, A. Fawzi\*, O. Fawzi, P. Frossard:
[*Universal adversarial perturbations*](http://arxiv.org/pdf/1610.08401), CVPR 2017.


# �^�[�Q�b�g�^�ėp�I�ۓ�(Japanese Docmentation)

���̃��|�W�g����[Universal Adversarial Perturbation](https://github.com/LTS4/universal)���^�[�Q�b�g�^�U���Ɋg���������̂ł��BPython3.x�̃R�[�h�̂݊܂݂܂��B

python3.x:[TensorFlow](https://github.com/tensorflow/tensorflow)���g���������Ă��܂��B���C�u��������`requirements.txt`�Ɍ��؎��Ɏg�p��������񋟂��Ă��܂�

�����悻�̐�����Universal Adversarial Perturbaion�Ɠ��l�ł����A�ۓ����d�ˍ��킹���摜���^�[�Q�b�g�ւƌ�F���銄����60�`70%�ł�

## �g����

### �͂��߂�

�܂��ŏ��ɁA���Ȃ��̎w�肵���C�ӂ̉摜�ɂ��āAInception���f�����g���A���O�w�K�ɂ���č��ꂽTargeted Universal Adversarial Perturbation���d�ˁA���ʌ��ʂ����o�����܂��B

```
python demo_inception.py -i data/test_img.png	
```

������s���Ǝ����I�Ɏ��O�w�K���ꂽInception���f�����_�E�����[�h���Atest_img.png�Ɂukit fox�v���^�[�Q�b�g�Ƃ���Targeted Universal Adversarial Perturbation��Y�����A���ʂ������ʂ̕�����ƂƂ��ɂ��o�͂��܂��B

![kit fox targeted images](data/index_img/target1.png)

�����̐ۓ���"Universal"�ł��邽�ߎ��炪�p�ӂ����ʂ̉摜�ɑ΂��Ă��d�ˍ��킹�邾���ŁA���l�̐������������Ƃ��m�F���Ă��܂��B

100�N���X���^�[�Q�b�g�Ƃ��āA���炩���ߐۓ����v�Z���Ă��܂��B�\�[�X�R�[�h�̏㕔��`target=1`���ilabels.txt���Q�l�ɂ��j1�`100�̍D���ɕύX���邱�Ƃŗe�ՂɃ^�[�Q�b�g�ۓ����d�ˍ��킹�邱�Ƃ��ł��܂��B
�Ⴆ��`target=3`�Ƃ���Ύ��̂悤�Ȍ��ʂƂȂ�܂��B

![kit fox targeted images](data/index_img/target3.png)

�܂�����ȊO�̃N���X�ɂ��Ă̍U���⎩�g�̃��f���ɂ����čs�������ꍇ���̏͂��Q�Ƃ��Ă��������B


###  �����̃��f����Targeted Universal Adversarial Perturbation���v�Z����




## �Q�l����

[1] S. Moosavi-Dezfooli\*, A. Fawzi\*, O. Fawzi, P. Frossard:
[*Universal adversarial perturbations*](http://arxiv.org/pdf/1610.08401), CVPR 2017.

*Targeted ver�̘_���͑��Ƙ_���Ƃ��Ď��M�������ߐl�ɂ������ł���_���ł͂���܂���B
���������Ď�@�����J�����_���͑��݂��܂���B�\�[�X�R�[�h���炨�C�������@���Ă��������B