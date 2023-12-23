## Exercise Round 11

Check out the notebook (ExerciseRound11.ipynb) for the questions and programming tasks (type your answers to the notebook).<br><br>
See the two-view SfM demo in SfMfrom2viewsDemo.ipynb (pics and other data contained by ./demo/ courtesy of ESAT/PSI Visics K.U.Leuven)

LINUX/UBUNTU

pip install virtualenv

conda create -n cv_course python=3.4 numpy scipy matplotlib scikit-image scikit-learn jupyter opencv-python
source activate cv_course

## Installing pyflann
(when python environment is activated)
$ conda config --add channels conda-forge
$ conda install pyflann
(https://github.com/primetang/pyflann/issues/1)

if there any issues with `index` or `PySide`, checkout
https://pypi.org/project/PySide/#building-pyside-on-a-unix-system-ubuntu-12-04-lts

$ wget https://pypi.python.org/packages/source/P/PySide/PySide-1.2.4.tar.gz
$ tar -xvzf PySide-1.2.4.tar.gz
$ cd PySide-1.2.4
$ python setup.py bdist_wheel --qmake=/usr/bin/qmake-qt4
$ ls dist

there should be a PySide-1.2.4 wheel in ./dist 
-> PySide-1.2.4-cp34-cp34m-linux_x86_64.whl
$ pip install ./PySide-1.2.4-cp34-cp34m-linux_x86_64.whl

Install `index`
$ pip install index