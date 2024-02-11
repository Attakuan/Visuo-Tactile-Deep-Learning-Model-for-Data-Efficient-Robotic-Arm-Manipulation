

# Visuo-Tactile Deep Learning Model for Data Efficient Robotic Arm Manipulation

Baselines forked from CoRL 2022 Paper: [Visuo-Tactile Transformers for Manipulation](https://arxiv.org/abs/2210.00121) <br />

In this project, we present a novel model for fusing Visuo-Tactile data for robot manipulation task. We propose: <br />
```
Convolutional Layer for visual data stream.
LSTM for tactile data stream
Attention layer for fusing the both streams.
```


Baselines for fusing Visuo-Tactile data:<br />
```
  Visuo-Tactile Transformer (VTT)
  Product-of-Experts (PoE)
  Concatenation (Concat)
  ```
  Requirements:<br />
```
  torch==1.9.0
  tqdm==4.48.2
  pybullet==3.1.8
  gym==0.17.2
  matplotlib==3.4.3
  numpy==1.21.2
  pandas==1.1.2
  ```
  Minitouch Installation:
  ```
  cd Minitouch
  pip install -e .
  ```
  Available Tasks:
  ```
  Pushing-v0
  Opening-v0
  Picking-v0
  Inserting-v0
  ```
  
  Example of Running Code:
  ```
  python train.py --encoder="VTT" --seed=0 --task_name="Pushing-v0"
 ```

Read Results with read_pickle.py<br />

For detailed information check Report.pdf <br />

# Credits<br />
Orignal Codes:
- Yizhou Chen, Andrea Sipos, Mark Van der Merwe, Nima Fazeli
Original Forked Code:
- https://github.com/yich7045/Visuo-Tactile-Transformers-for-Manipulation
