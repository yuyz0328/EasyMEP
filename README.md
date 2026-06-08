# EasyMEP

EasyMEP is an online system for maize ear phenotyping. It supports image upload, queued task execution, and result export.

The system currently supports:

- upload of maize ear photographs captured on a customized measurement board
- maize ear mask extraction and estimation of ear length and ear width traits
- kernel recognition on cross-section images and extraction of row-related traits
- kernel recognition on maize ear images and extraction of kernel-count traits
- maize kernel thickness extraction
- download of completed task result files

## Online Demo

[Open EasyMEP](http://zeasystemsbio.hzau.edu.cn/tools/easymep/)

## Sample Images

You can use the following sample images to test the online demo:

![Sample 1](images/sample1.jpg)
![Sample 2](images/sample2.jpg)
![Sample 3](images/sample3.jpg)

## Device Dependency

EasyMEP relies on a fixed-scale imaging setup, referred to as the **MEP Board**, for accurate maize ear trait extraction. The board design supports perspective correction and stable photography. Its main characteristics are:

- a background grid with 1 cm × 1 cm spacing, enabling size calibration from the image
- grooves used to stabilize maize ears and reduce rolling caused by uneven shape
- black-and-white corner markers used for perspective rectification
- a recommended camera-to-board distance of approximately 130 cm to reduce imaging error

![MEP Board Design](images/design.jpg)

![MEP Board](images/mep-board.jpg)

## Notes

- The public demo is intended for lightweight testing with sample images.
- The EasyMEP function is currently deployed on a CPU server, so its processing speed is relatively slow. It will be migrated to a GPU server for service in the future.
- To reduce server load, users should not upload more than 1 GB of images at one time.
- When uploading images, landscape orientation is recommended. Small rotations do not affect EasyMEP corner detection.
- For further information about EasyMEP, please contact `yuyz@webmail.hzau.edu.cn`.
