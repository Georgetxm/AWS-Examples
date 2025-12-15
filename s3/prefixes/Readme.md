
# Create bucket

```sh
aws s3 mb s3://prefixes-fun-xm-199
```

## Create folder (prefixes)

```sh
aws s3api put-object --bucket="prefixes-fun-xm-199" --key="hello/"
```
