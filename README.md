# 可视化检测结果

![可视化结果图](image-2.png)

大尺寸图象的推理结果说明，例Region_736565184：
```
image size: 38463x25295
[TensorRT] Deserialization required 65720 microseconds.
[TensorRT] Total per-runner device persistent memory is 0
[TensorRT] Total per-runner host persistent memory is 469520
[TensorRT] Allocated activation device memory of size 245861376
[TensorRT] CUDA lazy loading is enabled.
推理耗时统计: avg=41.5397 ms, min=5.35895 ms, max=452.472 ms
原始 patch 总数: 2688
跳过空白或全黑 patch 数: 1138
实际推理 patch 数: 1550
总检测目标数: 1857136
NMS去重后剩余目标数: 1856679
MultiPoint GeoJSON written to: output/points_multi.geojson
 总推理时间: 60637.6 ms
阳性细胞数: 680716
阴性细胞数: 1175963
阳性比例: 36.6631%
阴性比例: 63.3369%
最大常驻内存（Max RSS）: 6070432 KB
GPU总显存: 16379 MB
GPU剩余显存: 14895 MB
GPU已用显存: 1484 MB
```
![可视化结果图](Region_736565184_compressed.jpg)


# 实习工作也做过免疫组化 HER-2细胞检测
部分数据示例：

![可视化结果图](image.png)
模型预测全片的结果【局部结果展示】：

![可视化结果图](1.png)

结合癌区分割模型+细胞检测模型，进行免疫组化HER-2的阳性以及阴性率的计算分析
![可视化结果图](2.png)
![可视化结果图](3.png)
