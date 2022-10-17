# StarFront
## CDN Trace Dataset
The real-world CDN trace used in the paper is published here, hoping to stimulate more studies focusing on efficient content distribution in futuristic space-terrestrial integrated networks.

The trace was collected from an nanonymous commercial cloud CDN operator on February 22-28, 2015, containing 3.9 million flow records in total. Some details of the trace include:
| Parameter |  Value | 
| ---- | --- |
|# of Total Requests                 |    3,998,185           |
|# of Total Bytes Requested          |    4137 TB               |
|50th/90th Obj Size                   |   256KB / 1.3 GB        |
|Duration                             |   7 days (February 22-28, 2015)|

### Dataset Format

All the requests are given in time order and all the privacy-related information was ommitted. 

Each request in the dataset is given in a comma-separated format with 4 columns:
- **Seq** : The sequence number of the request in this dataset, starting from 0.
- **Timestamp**: The time when the request was issued, giving in UTC timestamp format.
- **Size**: The size of the content requested, given in B (Byte).
- **TimeToComplete**: The time spent to complete the content request, given in s (second).


The first five requests are given as example (no column name information was given in the dataset):

| Seq |  Timestamp | Size | TimeToComplete|
| ---- | --- | ---- |  ----               |
|0|1424534404|31929800|111|
|1|1424534409|833462272|658|
|2|1424534411|1048576000|10070|
|3|1424534412|9217283|98|
|4|1424534413|649075360|1892|

### Dataset Download
The dataset is available here: [download link](https://cloud.tsinghua.edu.cn/f/78ef1f2a03714640a793/?dl=1). 
