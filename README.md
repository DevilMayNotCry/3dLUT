# Image-Adaptive-3DLUT
Learning Image-adaptive 3D Lookup Tables for High Performance Photo Enhancement in Real-time



## Usage

## Now only for paired training

### For training
#### Paired training
     !pip install torchvision==0.5.0
     
     !pip install torch==1.4.0
     
     cd Image-Adaptive-3DLUT/trilinear_cpp
     
     !python3 setup.py install
     
     !python3 image_adaptive_lut_train_paired.py --input_dir <dir with images> 
                                                 --input_color_space <XYZ - for png, sRGB - for jpg> 
                                                 --n_cpu 2 
                                                 --batch_size 1
                                                 --output_dir <directory for results>
                                                 
#### Input dir structure:
    input_dir - | raw - dir with raw images
                | retouched - dir with retouched images
                | train_input.txt - image names with ext for train
                | test.txt - image names with ext for test
