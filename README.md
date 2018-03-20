# Camera Style Adaptation for Person Re-identification
================================================================

Code for Camera Style Adaptation for Person Re-identification (CVPR 2018). If you find this code useful in your research, please consider citing:

    @inproceedings{zhong2018camera,
    title={Camera Style Adaptation for Person Re-identification},
    author={Zhong, Zhun and Zheng, Liang and Zheng, Zhedong and Li, Shaozi and Yang, Yi},
    booktitle={CVPR},
    year={2018}
    }

### Prepare

1. Install [Pytorch](http://pytorch.org/)

2. Download dataset

   Please download datasets and put them into 'CamStyle/data/market' and 'CamStyle/data/duke', respectively.
   
   - Market-1501   [[BaiduYun]](https://pan.baidu.com/s/1ntIi2Op) [[GoogleDriver]](https://drive.google.com/file/d/0B8-rUzbwVRk0c054eEozWG9COHM/view)
   
   - DukeMTMC-reID   [[BaiduYun]](https://pan.baidu.com/share/init?surl=kUD80xp) (password: chu1) [[GoogleDriver]](https://drive.google.com/file/d/0B0VOCNYh8HeRdnBPa2ZWaVBYSVk/view)
   

3. Download CamStyle Images
   
   Please download CamStyle images and put them into 'CamStyle/data/market/boungding_box_train_camstyle' and 'CamStyle/data/duke/boungding_box_train_camstyle', respectively.

   - Market-1501-Camstyle   [[BaiduYun]]() [[GoogleDriver]]()
   
   - DukeMTMC-reID-CamStyle   [[BaiduYun]]() [[GoogleDriver]]()


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

-Our code is conducted based on [open-reid](https://github.com/Cysu/open-reid)

    
### Contact me

If you have any questions about this code, please do not hesitate to contact me.

[Zhun Zhong](http://zhunzhong.site)
