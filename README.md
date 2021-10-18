# Load Container Image Action

Loads a Docker image that was saved by a [Build Container Image action](https://github.com/twin-digital/action-build-container-image) execution in a previous job. After loading, the image will be available via the local Docker socket for verification or usage.

## Usage

```yaml
- uses: @twin-digital/action-load-container-image@v1
  with:
    # Name of the uploaded artifact containing the image.
    # Default: image
    artifact: ''
```

## Outputs

This step has the following outputs:

* `repository`: Repository name for the loaded image.
* `tag`: The first tag associated with the loaded image.
* `tags`: JSON string containing an array of *all* tags for the loaded image.

## License

The contents of this repository are released under the [MIT License](LICENSE).
