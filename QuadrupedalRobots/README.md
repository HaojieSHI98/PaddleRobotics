# ETG-RL

Reinforcement Learning with Evolutionary Trajectory Generator: A General Approach for Quadrupedal Locomotion

## Requirement
```txt
parl >= 1.4.0
torch >= 1.7.0
rlschool >= 1.0.2
```

## Train
```python
python train.py --task_mode stairstair --CPG_path data/origin_CPG/ESStair_origin.npz
```

## Eval
```python
python train.py --task_mode stairstair --eval 1 --load data/model/StairStair_3_itr_960231.pt
```

## BC training
```python
python BCtrain.py --task_mode stairstair --CPG_path data/model/StairStair_3_itr_960231.npz --ref_agent data/model/StairStair_3_itr_960231.pt
```