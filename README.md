# CLIPER
This Is the Official PyTorch Implementation for Our Paper:
>Towards Bridging the Cross-modal Semantic Gap for Multi-modal Recommendation

## Package
* numpy==1.21.5
* pandas==1.3.5
* python==3.7.11
* scipy==1.7.3
* torch==1.11.0
* pyyaml==6.0
* lmdb

## Usage
1.Prepare the environment: Install the required packages.
```
pip install -r requirements.txt
git clone https://github.com/beichenzbc/Long-CLIP.git
cd Long-CLIP
```
2.Preprocess: Choose the dataset to complete the preprocessing process.
```
python process_data.py
```
3.run the model on the preprocessed data.
```
cd src
python main.py
```

## Supported Models and Datasets
Models: BM3, DRAGON, DualGNN, FREEDOM, GRCN, ItemKNNCBF, LATTICE, LayerGCN, MGCN, MMGCN, MVGAE, SELFCFED_LGN, SLMRec, VBPR. See models' details in src/models. You also can add other recommendation models to src/models.

Datasets: Amazon datasets.

## ATTENTION
To run the model of CLIPER-MMCGN, you need to install the following packages:
```
pip install --no-index torch_scatter -f https://pytorch-geometric.com/whl/torch-1.11.0+cpu.html
pip install --no-index torch_sparse -f https://pytorch-geometric.com/whl/torch-1.11.0+cu102.html
pip install --no-index torch_cluster -f https://pytorch-geometric.com/whl/torch-1.11.0+cu113.html
pip install --no-index torch_spline_conv -f https://pytorch-geometric.com/whl/torch-1.11.0+cu115.html
pip install torch_geometric
```

## ACKNOWLEDGEMENT
Many thanks to enoche for their [MMRec](https://github.com/enoche/MMRec) for multimodal recommendation task.
