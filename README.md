Created in requirement to CSE597 Project. 

Citation: Nam, Jinwoo, Daechul Ahn, Dongyeop Kang, Seong Jong Ha, and Jonghyun Choi. "Zero-shot natural language video localization." In Proceedings of the IEEE/CVF International Conference on Computer Vision, pp. 1470-1479. 2021.

Dataset: https://drive.google.com/file/d/1Vjgm2XA3TYcc4h9IWR5k5efU-bXNir5f/view?usp=sharing
Pre-trained Net: https://drive.google.com/file/d/1M2FX2qkEvyked50LSc9Y5r87GBnpohSX/view?usp=sharing

# Environment
git clone https://github.com/gistvision/PSVL.git
cd PSVL
conda create --name PSVL --file requirements.txt
conda activate PSVL

# Training from scratch
python train.py --model CrossModalityTwostageAttention --config "YOUR CONFIG PATH"


# Evaluation
python inference.py --model CrossModalityTwostageAttention --config "YOUR CONFIG PATH" --pre_trained "YOUR MODEL PATH"



