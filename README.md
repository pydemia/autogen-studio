# autogen-studio

See: https://github.com/microsoft/autogen/tree/main/samples/apps/autogen-studio


```bash
git clone -n --depth=1 --filter=blob:none  --no-checkout \
  https://github.com/microsoft/autogen && \
  cd autogen &&\
  git sparse-checkout set --no-cone samples/apps/autogen-studio && \
  git checkout && \
  cd autogen-studio

```

```bash
cd autogen/samples/apps/autogen-studio

docker build . -f Dockerfile -t autogen_studio_img --platform=linux/amd64
docker build . -f Dockerfile -t autogen_studio_img --platform=linux/arm64
docker run --rm -p 8081:8081 autogen_studio_img


```

