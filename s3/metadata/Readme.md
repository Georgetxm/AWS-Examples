## Create a bucket

aws s3 mb s3://metadata-xm-199

## Create a new file

echo "Hello World" > hello.txt

## Upload file with metadata

aws s3api put-object --bucket metadata-xm-199 --key=hello.txt --body=hello.txt --metadata Planet=Mars

## Get metadata through head object

aws s3api head-object --bucket metadata-xm-199 --key hello.txt

## Remove item

aws s3 rm s3://metadata-xm-199/hello.txt

## Remvoe bucket

aws s3 rb s3://metadata-xm-199
