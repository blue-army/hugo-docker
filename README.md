# hugo-docker

Image containing the required assemblies to generate hugo documentation. Just run the container with the appropriate folder mounted, and call the hugo api.

## Run

Mount the base folder into the container and pass in the path to the `config.toml` file.

```sh
docker run --mount type=bind,source="$(pwd)",target=/work -w="/work" nullreference/hugo-docker --buildDrafts
```
