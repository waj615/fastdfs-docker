# FastDFS Docker

Usage:
```
docker run -dti --network=host --name tracker -v /var/fdfs/tracker:/var/fdfs waj615/fastdfs tracker

docker run -dti --network=host --name storage0 -e TRACKER_SERVER=fastdfs-tracker:22122 -e -v /var/fdfs/storage0:/var/fdfs waj615/fastdfs storage

docker run -dti --network=host --name storage1 -e TRACKER_SERVER=fastdfs-tracker:22122 -e -v /var/fdfs/storage1:/var/fdfs waj615/fastdfs storage

docker run -dti --network=host --name storage2 -e TRACKER_SERVER=fastdfs-tracker:22122 -e GROUP_NAME=group2 -e PORT=22222 -v /var/fdfs/storage2:/var/fdfs waj615/fastdfs storage
```
