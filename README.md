# Finetuning-LLMS

## NOTES: 

Full Precision / HAlf Precision : Data - > related to data types how it is stored in memory -> data types : weights and parameters
Callibration -> in mmodel quantization - how we quantized?
Modes of Quantization :  Post training - Quantization Aware Training
Quantization: conversion from higher memory format to lower memory format
Weights are in the form of matrix - > Every value is stored in memory in the form of 32bits

symmetric distribution: evenly distributed 
                        batch symmetric
                        [0-1000]  batch normalization - near 0 centered
                        scale factor ( 1000-0 / 255-0)   any number convert from fp32 to uint8 
                        
asymmetric:

[-20 ... 1000]
[0 .... 255 ]

forcefully assingn value 

-20/4 = 5 - 5 = 0 assigning 0 to -20
