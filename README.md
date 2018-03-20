# Camera Style Adaptation for Person Re-identification
================================================================

### Prepare

1. Install Pytorch

2. Download dataset


### Train and test

1. IDE
  ```Shell
  # For Market-1501
  python main.py -d market --logs-dir logs/market-ide
  # For Duke
  python main.py -d duke --logs-dir logs/duke-ide
  ```
2. IDE + CamStyle
  ```Shell
  # For Market-1501
  python main.py -d market --logs-dir logs/market-ide-camstyle --camstyle 46
  # For Duke
  python main.py -d duke --logs-dir logs/duke-ide--camstyle --camstyle 46
  ```
  
3. IDE + CamStyle + Random Erasing
  ```Shell
  # For Market-1501
  python main.py -d market --logs-dir logs/market-ide-camstyle-re --camstyle 46 --re 0.5
  # For Duke
  python main.py -d duke --logs-dir logs/duke-ide--camstyle-re --camstyle 46 --re 0.5
  ```

### References

- Our code is conducted based on [open-reid](https://github.com/Cysu/open-reid)


If you find this code useful in your research, please consider citing:

    @inproceedings{zhong2018camera,
    title={Camera Style Adaptation for Person Re-identification},
    author={Zhong, Zhun and Zheng, Liang and Zheng, Zhedong and Li, Shaozi and Yang, Yi},
    booktitle={CVPR},
    year={2018}
    }
    
        
### Contact us

If you have any questions about this code, please do not hesitate to contact us.

[Zhun Zhong](http://zhunzhong.site)
