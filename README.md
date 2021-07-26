# misc

This repository serves miscellaneous downloads for the [Envoy®](https://www.envoyproxy.io/) project.

Unlike usual repositories, a [release](https://github.com/envoyproxy/misc/releases) here is a
download category. This means releases are unrelated to each other. Rather, they are a bundle of
related artifacts.

For example, a release named "jaegertracing-plugin" would have nothing to do with other releases,
except that these are for Envoy purposes, most typically download links in examples or blogs.

This is not an appropriate place to serve production artifacts or sub-projects. This repository is
to provide an alternative to checking in miscellaneous binaries into source control or relying on
third-party sites.

## Creating a release

1. Install the [GitHub CLI](https://cli.github.com/)
2. Choose an intuitive name for the assets
3. Create the release, uploading the files

Ex. For a download category "jaegertracing-plugin" which has a single file
```bash
gh release create jaegertracing-plugin --notes "jaegertracing-plugin" ./jaegertracing-plugin-centos.tar.gz
```

The above file would be available for direct downloads from the release page, or an expression like this:
```
https://github.com/envoyproxy/misc/releases/download/jaegertracing-plugin/jaegertracing-plugin-centos.tar.gz
```

-----
Envoy® is a registered trademark of The Linux Foundation in the United States and/or other countries
