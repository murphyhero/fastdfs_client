# fdfs_client.go

fastdfs go client implement

**1 support** 

upload(UploadByFilename,UploadByBuffer)

download(DownloadToFile,DownloadToBuffer)

delete(DeleteFile)

**2 append is not support(limited by fastdfs server)**

you can implement append with delete origin && upload new again

**3 UploadByFilename realized with sendfile syscall in linux,so UploadByBuffer is depracated**

**4 realized conn_pool,pool_size control by config file**

**5 details see client_test.go,good luck ^_^**

## $ go get github.com/murphyhero/fastdfs_client.git

# Author
murphy_guo@126.com
yue.cheng.ted@gmail.com
