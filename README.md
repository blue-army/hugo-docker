# hugo-docker

Image contains the required assemblies to generate hugo documentation.

## Run

Mount the base folder into the container and pass in the path to the `config.toml` file.

```sh
docker run --mount type=bind,source="$(pwd)",target=/work -w="/work" nullreference/hugo-docker --buildDrafts
```