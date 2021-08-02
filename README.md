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

# Related Works

<p align="center">
    <img src="./figures/fig_related.jpg"/> <br />
    <em> 
    Figure 2: Summary of widely used salient object detection (SOD) datasets and our SHD360. GT = ground truth. ER Image = equirectangular image. Attr. = attributes. obj. = object-level GT. ins. = instance-level GT. Please note that all the datasets listed above provide pixel-wise annotations.
    </em>
</p>


------

# DataSet: SHD360

<p align="center">
    <img src="./figures/fig_categories.jpg"/> <br />
    <em> 
    Figure 3: Statistics of the proposed SHD360. (a)/(b) The quantity of object-/instance-level per-pixel ground-truth masks of each of the scene categories. (c) Hierarchical labels including two super-classes (indoor/outdoor) and 41 scene categories. Attributes statistics including (d) and (e) which represent correlation and frequency of proposed attributes, respectively. (f) Descriptions of the six proposed attributes associated with each of the scene categories.
    </em>
</p>

<p align="center">
    <img src="./figures/fig_attributes.jpg"/> <br />
    <em> 
    Figure 4: Examples of instance-level pixel-wise labels and challenging attributes (please refer to Figure 3 (f) for details) of our SHD360. 
    </em>
</p>

------

# 360° Geometry-adapted S-measure

<p align="center">
    <img src="./figures/fig_metric.jpg"/> <br />
    <em> 
    Figure 5: A comparison between traditional S-measure and proposed 360° geometry-adapted S-measure. The former/latter compute region similarities based on ER blocks/cube maps, respectively. ’+X’,’-X’,’+Y’,’-Y’,’+Z’ and ’-Z’ denote cube maps covering a FoV of 90°×90°, observed from the right, left, up, down, front and back by a 360° camera.
    </em>
</p>

------

# Benchmark

## Overall Results

<p align="center">
    <img src="./figures/fig_qua.jpg"/> <br />
    <em> 
    Figure 6: Performance comparison of 8/2 SOTA SOD/VSOD methods and one 360° SOD method over the three testing sets of our SHD360. S = S-measure (α=0.5), S360 = 360° geometry-adapted S-measure, Fβ = mean F-measure (β2=0.3), Eφ = mean E-measure, M = mean absolute error. ↑/↓ denotes a larger/smaller value is better. The three best results of each column are in red, blue and green, respectively.
    </em>
</p>


## Atrributes-based Results

<p align="center">
    <img src="./figures/fig_qua_attr.jpg"/> <br />
    <em> 
    Figure 7: Attributes-based performance comparison of 11 baselines over our SHD360. ↑/↓ denotes a larger/smaller value is better. Three best results of each row are in red, blue and green, respectively.
    </em>
</p>

------

# Downloads

The object-/instance-level ground truth (with default split) and edge maps can be downloaded from [Baidu] or [Google](https://drive.google.com/file/d/1TII7lQhVPf9tZIUve8FCWsfwFWVxv0N7/view?usp=sharing).

------

# Contact 

Please feel free to drop an e-mail to yi.zhang1@insa-rennes.fr for questions or further discussion.

------

# Citation

    @article{zhang2021shd360,
      title={SHD360: A Benchmark Dataset for Salient Human Detection in 360° Videos},
      author={Zhang, Yi and Zhang, Lu and Zhang, Jing and Wang, Kang and Hamidouche, Wassim and Deforges, Olivier},
      journal={arXiv preprint arXiv:2105.11578},
      year={2021}
    }

