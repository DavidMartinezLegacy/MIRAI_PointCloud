# MIRAI_PointCloud
A repository for learning Open3D
真实物体表面的离散采样
```shell
conda create -n open3denv python=3.6
conda activate open3denv
conda install -c open3d-admin open3d==0.8.0.0
```
[Dataset](http://graphics.stanford.edu/data/3Dscanrep/)
```
import open3d as o3d
import wget
url = 'https://raw.githubusercontent.com/PointCloudLibrary/pcl/master/test/bunny.pcd'
#filename = wget.download(url)
pcd = o3d.io.read_point_cloud("bunny.pcd")
print(pcd)
```
