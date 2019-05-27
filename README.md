# Deep Reasoning with Knowledge Graph for Social Relationship Understanding

This repo is modified from the paper: "[Deep Reasoning with Knowledge Graph for Social Relationship Understanding](https://arxiv.org/abs/1807.00504)" (IJCAI 2018) by Zhouxia Wang, Tianshui Chen, Jimmy Ren, Weihao Yu, Hui Cheng, Liang Lin.

## Environment

The code is implemented using the Pytorch library with Python 2.7 and has been tested on a desktop with the system of Ubuntu 16.04 LTS.

## Dataset
[PISC](https://zenodo.org/record/1059155#.WznPu_F97CI) was released by [[Li et al. ICCV 2017](https://arxiv.org/abs/1708.00634)]. It involves two-level relationship, i.e., coarse-level relationships with 3 categories and fine-level relationships with 6 categories.

## Usage
    usage: test.py [-h] [-j N] [-b N] [--print-freq N] [--weights PATH]
               [--scale-size SCALE_SIZE] [--world-size WORLD_SIZE] [-n N]
               [--write-out] [--adjacency-matrix PATH] [--crop-size CROP_SIZE]
               [--result-path PATH]
               DIR DIR DIR

    PyTorch Relationship

    positional arguments:
      DIR                       path to dataset
      DIR                       path to objects (bboxes and categories of objects)
      DIR                       path to test list

    optional arguments:
      -h, --help                show this help message and exit
      -j N, --workers N         number of data loading workers (defult: 4)
      -b N, --batch-size N      mini-batch size (default: 1)
      --print-freq N, -p N      print frequency (default: 10)
      --weights PATH            path to weights (default: none)
      --scale-size SCALE_SIZE   input size
      --world-size WORLD_SIZE   number of distributed processes
      -n N, --num-classes N     number of classes / categories
      --write-out               write scores
      --adjacency-matrix PATH   path to adjacency-matrix of graph
      --crop-size CROP_SIZE     crop size
      --result-path PATH        path for saving result (default: none)




