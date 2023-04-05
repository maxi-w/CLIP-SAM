# CLIP-SAM

Small experiment on combining CLIP with SAM to do open-vocabulary image segmentation.

- [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything)
- [Contrastive Language-Image Pre-Training (CLIP)](https://github.com/openai/CLIP)

The approach is to first identify all the parts of an image using SAM, and then use CLIP to find the ones that best match a specific description.

## Usage

1. Download [weights](https://github.com/facebookresearch/segment-anything#model-checkpoints) and place them in this repos root.

2. Install dependencies:
```python
    pip install torch opencv-python Pillow
    pip install git+https://github.com/openai/CLIP.git
    pip install git+https://github.com/facebookresearch/segment-anything.git
```
3. Run Notebook `main.ipynb`


## Example

Example output for prompt "kiwi"

![Image with segmentation](assets/example-segmented.png)


[Example Image Source](https://unsplash.com/photos/zeFy-oCUhV8?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)