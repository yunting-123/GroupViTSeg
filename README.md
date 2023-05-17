# Leveraging Local Features and Attention for Efficient Image Segmentation Using Text and Image Prompts

### Datasets

* PhraseCutPlus`: Referring expression dataset
* `PFEPascalWrapper`: Wrapper class for PFENet's Pascal-5i implementation
* `PascalZeroShot`: Wrapper class for PascalZeroShot
* `COCOWrapper`: Wrapper class for COCO.

### Third Party Dependencies
For some of the datasets third party dependencies are required. Run the following commands in the `third_party` folder.  
```bash
git clone https://github.com/cvlab-yonsei/JoEm
git clone https://github.com/Jia-Research-Lab/PFENet.git
git clone https://github.com/ChenyunWu/PhraseCutDataset.git
git clone https://github.com/juhongm999/hsnet.git
```

### Training and Evaluation

To train use the `training.py` script with experiment file and experiment id parameters. E.g. `python training.py phrasecut.yaml 0` will train the first phrasecut experiment which is defined by the `configuration` and first `individual_configurations` parameters. Model weights will be written in `logs/`.

For evaluation use `score.py`. E.g. `python score.py phrasecut.yaml 0 0` will train the first phrasecut experiment of `test_configuration` and the first configuration in `individual_configurations`.



### 
