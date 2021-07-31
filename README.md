# SHD360: A Benchmark Dataset for Salient Human Detection in 360° Videos

# Introduction

<p align="center">
    <img src="./figures/fig_teaser.jpg"/> <br />
    <em> 
    Figure 1: An illustration of 360° video salient human detection (VSHD). The first row, two random key frames of a 360° panoramic video from our SHD360. The shown 360° video frames are mapped to plane by conducting equirectangular (ER) projection. The middle row: a subject observes 360° content by moving his head to control the field-of-view (FoV) in a range of 360°×180°. The salient human instances with 360° attributes observed in spherical FoVs at specific rotation angles (e.g., θi, θj). The last row: corresponding annotations such as per-pixel instance-level ground truth (GT) and general attributes including MP-multiple persons, DV-distant view and MB-motion blur.
    </em>
</p>

Salient human detection (SHD) in dynamic 360° immersive videos is of great importance for various applications such as robotics, inter-human and human-object interaction in augmented reality. However, 360° video SHD has been seldom discussed in the computer vision community due to a lack of datasets with large-scale omnidirectional videos and rich annotations. To this end, we propose SHD360, the first 360° video SHD dataset which contains various real-life daily scenes. Our SHD360 provides six-level hierarchical annotations for 6,268 key frames uniformly sampled from 37,403 omnidirectional video frames at 4K resolution. Specifically, each collected key frame is labeled with a super-class, a sub-class, associated attributes (e.g., geometrical distortion), bounding boxes and per-pixel object-/instance-level masks. As a result, our SHD360 contains totally 16,238 salient human instances with manually annotated pixel-wise ground truth. Since so far there is no method proposed for 360° image/video SHD, we systematically benchmark 11 representative state-of-the-art salient object detection (SOD) approaches on our SHD360, and explore key issues derived from extensive experimenting results. We hope our proposed dataset and benchmark could serve as a good starting point for advancing human-centric researches towards 360° panoramic data. 

:running: :running: :running: ***KEEP UPDATING***.

------

# Citation

    @article{zhang2021shd360,
      title={SHD360: A Benchmark Dataset for Salient Human Detection in 360° Videos},
      author={Zhang, Yi and Zhang, Lu and Zhang, Jing and Wang, Kang and Hamidouche, Wassim and Deforges, Olivier},
      journal={arXiv preprint arXiv:2105.11578},
      year={2021}
    }

