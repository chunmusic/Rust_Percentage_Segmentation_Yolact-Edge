# Rust Percentage Instance Segmentation (Yolact-Edge)

- This repository is created to calculate rust percentage with instance segmentation.

- The model was trained based on Yolact-Edge.

- Yolact-Edge will detect test pieces which contains rust area and non-rust area and calculate rust percentage.

- Please go to this url to download weight file (https://drive.google.com/drive/folders/1dMHNiwz7B7azoJdPoqXwteOaO4Qf5CrY?usp=sharing)

- The project was implemented in World Robot Summit 2020 (WRS) competition.

## How to use

- Please run the following command to run the demo.

```python
python eval.py --trained_model=weights/yolact_edge_199999_800000.pth --score_threshold=0.3 --top_k=100 --video_multiframe=2 --trt_batch_size 2 --video=rust.mp4 --disable_tensorrt
```

## Preview

![Image1](https://raw.githubusercontent.com/chunmusic/Rust_Percentage_Segmentation_Yolact-Edge/master/output.gif)

### Reference

https://github.com/haotian-liu/yolact_edge
