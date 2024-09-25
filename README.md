# 05-openshift-rootless-build

Tutorial setup from https://github.com/containers/buildah/blob/main/docs/tutorials/05-openshift-rootless-build.md

To build, run:
```
mkdir output && \
buildah build --layers -v $(pwd)/output:/output:rw -v $(pwd)/test-script.sh:/test-script.sh:ro -t myimage -f Containerfile.test
```
