# VSW
Vehicle search in the Wild: A New Benchmark
## VSW_v1

- This repository contains the VSW dataset for the following paper：[Unsupervised Vehicle search in the Wild: A New Benchmark (ACM MM 2021)](https://dl.acm.org/doi/10.1145/3474085.3475654). 
- Vehicle search is a crucial part of the city's surveillance system. However, existing research does not fully explore end-to-end vehicle search. Instead, VSW aims to advance the task of vehicle search and benefit traffic regulation and criminal investigations.

- Here . This dataset is for research purposes only and therefore not for commercial use.

- If you have any questions about the VSW dataset, please contact zhongx@whut.edu.cn.

- VSW for vehicle search.
- ![](https://github.com/zsl1997/VSW/blob/main/1.png)

## Description
Note that, we publish only part of the data, also for the initial version. It contains 76,387 frames and 475 ids. We split the dataset into a train and a test subset, ensuring no overlapped images or labeled identities between them. The train set contains 38,280 frames and 254 training IDs, the first 99 are cross-camera ids. The test set contains 38,280 frames and 254 training IDs, the first 97 are cross-camera ids. Then for each vehicle in the test set, we randomly select two bounding boxes as query vehicles under each camera.

- This dataset is organized as follows:
```

├── annotations               # Annotation of frames
│   ├── */*.mat                       
├── frames                    # the vehicle frames
│   ├── */*.jpg                        
├── query                     # query set
│   ├── */*.jpg               
├── frame_train.mat           # frames for model training
├── frame_test.mat            # frames for model testing
├── ID_train.mat              # IDs for model training
├── ID_test.mat               # IDs for model testing
├── query_info.txt            # query set

```

### **Citation**
If you find our dataset useful in your research work, please consider citing:

bib:

    @inbook{10.1145/3474085.3475654,
    title = {Unsupervised Vehicle Search in the Wild: A New Benchmark},
    author = {Zhong, Xian and Zhao, Shilei and Wang, Xiao and Jiang, Kui and Liu, Wenxuan and Huang, Wenxin and Wang, Zheng},
    booktitle = {Proceedings of the 29th ACM International Conference on Multimedia},
    year = {2021},
    pages = {5316–5325},
    }

