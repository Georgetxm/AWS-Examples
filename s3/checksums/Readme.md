
## Create a new s3 Bucket

```md
aws s3 mb s3://checksums-examples-xm-199
```

## Create a file that we will do a checksum on

```md
echo "Hello Mars" > myfile.txt
```

## Get a checksum of the file

md5sum myfile.txt

# 8ed2d86f12620cdba4c976ff6651637f  myfile.txt

## Upload file to s3

```md
aws s3 cp myfile.txt s3://checksums-examples-xm-199
aws s3api head-object --bucket checksums-examples-xm-199 --key myfile.txt
```

## Upload file with different checksum algo

```md

```
