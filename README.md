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
|0|1424534404|0x6cc00e85eacfc56c|31929800|111|
|1|1424534409|0xf2e79b2ae42ea5b|833462272|658|
|2|1424534411|0x8b4c8304587a4ad5|1048576000|10070|
|3|1424534412|0x536cf07acc3eeb9d|9217283|98|
|4|1424534413|0xc48b2b9b7b00e2f3|649075360|1892|

### Dataset Download
The dataset is available here: [download link](https://cloud.tsinghua.edu.cn/f/28bf6f262a65430a91f0/?dl=1). 

Note that a few illegal records were erased, for the convenience of the dataset users, and thus some details of the public download version may not perfectly match with what stated [above](#cdn-trace-dataset).
