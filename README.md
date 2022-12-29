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

The requests are given in time order and all the privacy-related information was ommitted. 

Each request in the dataset is given in a comma-separated format with 5 columns:
- **Seq** : The sequence number of the request in this dataset, starting from 0.
- **Timestamp**: The time when the request was issued, given in UTC timestamp format.
- **ObjectID**: The unique object ID of the content requested.
- **Size**: The size of the content requested, given in B (Byte).
- **TimeToComplete**: The time spent to complete the content request, given in s (second).


The first five requests are given as example (no column name information was included in the dataset):

| Seq |  Timestamp | ObjectID | Size | TimeToComplete|
| ---- | --- | ---- |  ---- | ----               |
|0|1424534404|102923E4D078CB12660EFBD212AE1471425A3E67|31929800|111|
|1|1424534409|0F60DAD8FE80CA35536E73F18476EAB3A34250A2|833462272|658|
|2|1424534411|FD14FB3FFE8D8E9F4653DF5F2C39C230625B3D74|1048576000|10070|
|3|1424534412|4458435F7CC5249EB00BB6E8CE8DE12CC6B6767C|9217283|98|
|4|1424534413|774157731FD1E113F35208ED904CA9A72E53C8AD|649075360|1892|

### Dataset Download
The dataset is available here: [download link](https://cloud.tsinghua.edu.cn/f/28bf6f262a65430a91f0/?dl=1). 

Note that a few illegal records were erased, for the convenience of the dataset users, and thus some details of the public download version may not perfectly match with what stated [above](#cdn-trace-dataset).
