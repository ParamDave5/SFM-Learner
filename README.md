# Improved SfMLearner

### Model Training
To train the entire pipeline, we provide the following commands:
```commandline
cd new_sfm
python train.py --ssim_weight xxx
```
Here we include our random color data augmentation by default. By setting ssim_weight equal to 0, we can recover the original SFM model.

### Model Testing
To test the depth prediction, run:
```commandline
python test_kitti_depth.py
```

To test the pose prediction, run:
```commandline
python test_kitti_pose.py
```

### Model Evaluation
To evaluate the depth prediction, run:
```commandline
python ./kitti_eval/eval_depth.py
```

To evaluate the pose prediction, run:
```commandline
python ./kitti_eval/eval_pose.py
```
# SFM-Learner
