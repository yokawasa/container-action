# Sample Docker Container Action

## Quickstart

```
# Build
docker build -t container-action:v1.0 . 

# Test Run
docker run -it container-action:v1.0 
hello 
docker run -it container-action:v1.0 world
hello world
```

Create release branch
```
git checkout -b v1
git add *
git commit -a -m "v1 release"
git push origin v1
```

Now you can consume the action with yml file like this:
```
uses: yokawasa/container-action@v1
with:
  myInput: 'world'
```



## REFERENCES
- [Creating Container Action](https://github.com/actions/toolkit/blob/master/docs/container-action.md)
- [Actions Versioning](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md)
