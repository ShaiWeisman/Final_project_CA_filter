# Depth refinement using content aware neural network filters
M.Sc final project under the supervision of Dr.Raja Giryes and P.H.D candidate mr. Shai Elmalem

## Abstract
Depth estimation is an important yet challenging problem in computer vision. Since both stereo
and monocular methods tend to fail in texture less, repetitive and\or caged regions, the final
depth estimation generally suffers from artifacts that affect the quality of the result.
The goal of the current project is to study the use of neural networks for depth maps
improvement using content aware neural network filters. Two main approaches are tested:
Joint-filter network (JF-Net), a CNN which selectively transfer salient structures that are
consistent with both guidance and target images, and Fast Deformable Kernel Network, a DNN
which defines a set of neighbors and the corresponding weights (based on both guidance and
target images ) adaptively for each pixel . Both solutions are testes with several architecture
variants and different loss functions.
After analysing all the different solutions, we achieved a reduction of 20% in the L1 error using
the FDKN adaptive loss network on the validation set. However, improvement on the real-world
images was smaller.
This work presents the potential of content aware filters in error reduction, and hopefully with
additional tools will help to bridge the domain gap between synthetic and real-world datasets.

## Main refrences
this work is based on 3 main papers:

Depth input data:<br/>
H. Haim, S. Elmalem, R. Giryes, A. Bronstein, and E. Marom (2018) Depth Estimation
from a Single Image using Deep Learned Phase Coded Mask. IEEE Transactions on
Computational Imaging, pp. 298 – 310

Content Aware filter:<br/>
Kim, Beomjun, Jean Ponce, and Bumsub Ham. "Deformable Kernel Networks for Joint
Image Filtering." arXiv preprint arXiv:1910.08373 (2019)

Adaptive loss function:<br/>
Barron, Jonathan T. "A general and adaptive robust loss function." Proceedings of the
IEEE Conference on Computer Vision and Pattern Recognition. 2019.
