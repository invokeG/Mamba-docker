# Mamba-docker
<p align="center">
  <img alt="Static Badge" src="https://img.shields.io/badge/mamba_ssm-1.1.1-green">
  <img alt="Static Badge" src="https://img.shields.io/badge/causal_conv1d-1.1.1-lightgreen">
  <img alt="Static Badge" src="https://img.shields.io/badge/pytorch-1.13-blue">
  <img alt="Static Badge" src="https://img.shields.io/badge/cuda-11.7-lightblue">
  <img alt="Static Badge" src="https://img.shields.io/badge/Ubuntu-20.04-orange">
  <br>
</p>

Docker Hub : https://hub.docker.com/repository/docker/kom4cr0/cuda11.7-pytorch1.13-mamba1.1.1/general

## Introduction
Build according to github repo README.

Mamba GitHub link : https://github.com/state-spaces/mamba. 
This docker is also suitable for VMamba.

**This is just a basic environment in Ubuntu20.04, in order to solve the problem of `causal_conv1d & mamba_ssm` installation errors. You may also need to add other packages to run Manba.**

 This docker includes the following basic packages: 
>cuda==11.7 (docker: nvidia/cuda)

>pytorch==1.13

>causal_conv1d==1.1.1

>mamba_ssm==1.1.1

## Pull
This tag is not `<latest or default>` !
```
docker pull kom4cr0/cuda11.7-pytorch1.13-mamba1.1.1:1.1.1 
```

## Test
```
python
>>>import torch
>>>from mamba_ssm import Mamba
```
