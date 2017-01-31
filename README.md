# s3archive
An easy to use python3 package to archive files on Amazon S3

```python
from s3archive.s3archive import Archive

my_archive = Archive('my-bucket', 's3.csv')

if my_archive.exists('config/is-image-example.txt'):
    for key, file_object in my_archive.find('images/.*?/'):
        print(key)
```
