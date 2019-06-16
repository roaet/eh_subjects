[//]: # (pypi) Uploading packages to pypi
Pypi help

1. New pypi requires that you use twine: `pip install twine`
2. Then make an sdist: `python setup.py sdist`
3. Then upload with twine: `twine upload dist/*`

```
If you have issues making a release version (one without -devblah), do this:
git tag X.Y.Z -m "Some message"

It is important you do not put a v in front of the X.Y.Z!
```

See pypi.org for information on how to make a `.pypirc`
