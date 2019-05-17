# Targeted Universal adversarial perturbations

This repos extended [Universal Adversarial Perturbation](https://github.com/LTS4/universal) to target attack.

Only Python3.x ver included.

*python*: Python3.x code to generate universal perturbations using [TensorFlow](https://github.com/tensorflow/tensorflow).


# Python

Python code to find a universal perturbation [[1]](http://arxiv.org/pdf/1610.08401), using the [TensorFlow](https://www.tensorflow.org/) library.

## Usage

### Get started

To get started, you can run the demo code to apply a pre-computed universal perturbation for Inception on the image of your choice
```
python demo_inception.py -i data/test_img.png	
```
This will download the pre-trained model, and show the image without and with universal perturbation with the estimated labels.
In this example, the pre-computed targeted universal perturbation in `data/universal.npy` is used. This Perturbation tageted kit fox class.

### Computing a universal perturbation for your model

To compute a universal perturbation for your model, please follow the same struture as in `demo_inception.py`.
In particular, you should use the `universal_perturbation` function (see `universal_pert.py` for details), with the set of training images 
used to compute the perturbation, as well as the feedforward and gradient functions.

## Reference
[1] S. Moosavi-Dezfooli\*, A. Fawzi\*, O. Fawzi, P. Frossard:
[*Universal adversarial perturbations*](http://arxiv.org/pdf/1610.08401), CVPR 2017.


# �^�[�Q�b�g�^�ėp�I�ۓ�(Japanese Docmentation)

���̃��|�W�g����[Universal Adversarial Perturbation](https://github.com/LTS4/universal)���^�[�Q�b�g�^�U���Ɋg���������̂ł��BPython3.x�̃R�[�h�̂݊܂݂܂��B

python3.x:[TensorFlow](https://github.com/tensorflow/tensorflow)���g���������Ă��܂��B

## �g����

### �͂��߂�

�܂��ŏ��ɁA���Ȃ��̎w�肵���C�ӂ̉摜�ɂ��āAInception���f�����g���A���O�w�K�ɂ���č��ꂽTargeted Universal Adversarial Perturbation���d�ˁA���ʌ��ʂ����o�����܂��B

```
python demo_inception.py -i data/test_img.png	
```

������s���Ǝ����I�Ɏ��O�w�K���ꂽInception���f�����_�E�����[�h���Atest_img.png��Targeted Universal Adversarial Perturbation��Y�����A���ʂ������ʂ̕�����ƂƂ��ɂ��o�͂��܂��B

###  �����̃��f����Targeted Universal Adversarial Perturbation���v�Z����