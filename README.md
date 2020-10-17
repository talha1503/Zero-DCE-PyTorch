# Zero-DCE: Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement
Pytorch implementation of [Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement](https://openaccess.thecvf.com/content_CVPR_2020/papers/Guo_Zero-Reference_Deep_Curve_Estimation_for_Low-Light_Image_Enhancement_CVPR_2020_paper.pdf)

## Model Architecture

<p align="center">
<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/model_architecture.png">
</p>


#### Result

<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/2_input.bmp" width="256" height="256">  <img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/2_output.bmp" width="256" height="256"> <br>
<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/5_input.bmp" width="256" height="256">  <img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/5_output.bmp" width="256" height="256"> <br>
<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/6_input.bmp" width="256" height="256">  <img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/6_output.bmp" width="256" height="256"> <br>
<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/8_input.bmp" width="256" height="256">  <img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/8_output.bmp" width="256" height="256"> <br>
<img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/10_input.bmp" width="256" height="256">  <img src="https://github.com/talha1503/Zero-DCE/blob/master/assets/results/10_output.bmp" width="256" height="256"> <br>


## References
[1] Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement - CVPR 2020 [link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Guo_Zero-Reference_Deep_Curve_Estimation_for_Low-Light_Image_Enhancement_CVPR_2020_paper.pdf)


## Citation
```
    @misc{guo2020zeroreference,
    title={Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement},
    author={Chunle Guo and Chongyi Li and Jichang Guo and Chen Change Loy and Junhui Hou and Sam Kwong and Runmin Cong},
    year={2020},
    eprint={2001.06826},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
```

Note: Some changes were made as compared to the original paper.
<ul>
<li>
Learning rate was kept to 1e-3 instead of 1e-4.
</li>
<li>
Also, in the paper, equation for the curves is given as: LEn(x) = LEn−1(x) + αnLEn−1(x)(1 − LEn−1(x)) , whereas in the author's original implementation, the curve equation is taken as: LEn(x) = LEn−1(x) + αnLEn−1(x)(LEn−1(x) - 1)
</li>
</ul>
