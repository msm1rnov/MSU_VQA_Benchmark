Video Quality Assessment (VQA) benchmark provides performance of no-reference (pristine signal is not required) and full-reference methods, which are capable of assessing quality of different videos. Unlike images, videos contain temporal information, whose usage can lead to more reliable prediction of quality. That’s why the proposed benchmark includes both VQA and IQA methods, which have been tested on a range of diverse sequences, compressed with different standards, presets and bitrates. To make the research more objective, experiments with methods performance evaluation on some pools of videos separately have been conducted. Finally, we have provided all the results and analysis not only through tables but also using visualizations to simplify the perception of great amount of information. The ranking of some existing methods proposed through this benchmark may help the reader either detect features in top methods to create their own SOTA VQA method or find the best methods for their aims, such as finding the perceptual optimization of RD tradeoffs in video encoding and streaming.

## Benchmark details

You may find detailed description of benchmark as well as our dataset [here](https://videoprocessing.ai/benchmarks/video-quality-metrics.html).

## Results section
| Method | SROCC on Full Dataset |
|:--------------------:|:--------------:|
NR MEON              |  0.516572
FR FOV VIDEO       |          0.542921
NR TLVQM             |        0.571137
NR NIQE Y             |      0.587831
NR VIDEVAL           |        0.733429
FR LPIPS                |    0.805404
FR GREED              |      0.807199
NR KONIQ               |      0.817207
FR VQM Y               |      0.835021
NR SPAQ BL           |        0.838357
NR NIMA                 |              0.849232
NR PAQ-2-PIQ        |         0.849411
NR SPAQ MT-A        |         0.852967
FR PSNR YUV               |     0.854303
NR SPAQ MT-S        |         0.856873
FR TENCENT            |       0.860325
FR DISTS                  |   0.861489
FR SSIM YUV |            0.884728
FR AVQT         |             0.890449
NR VSFA          |            0.899390
FR MS-SSIM Y             |       0.899817
FR VMAF Y (v061_neg) |            0.906949
NR LINEARITY    |             0.914331
FR VMAF YUV NEG |    0.919048
NR MDTVSFA           |        0.921918
FR VMAF Y (v061)          |      0.942068
FR VMAF YUV                |       0.948621

## How to submit
Send us an email to vqa@videoprocessing.ai with the file of .exe extension with your algorithm and instructions to run it from console. When launched from console we expect your file to have following options (or their analogs):

#### For Full-reference metrics: 
* `-ref` — path to reference video
* `-dist` — path to distorted video
* `-output` — path to output of your algorithm
* `-t` — threshold, if it required in your algorithm
 
 #### For No-reference metrics: 
*  `-dist` — path to distorted video
* `-output` — path to output of your algorithm
*  `-t` — threshold, if it required in your algorithm


Feel free to add any addition information about your algorithm. We won’t publish results of your algorithm without your permission.
