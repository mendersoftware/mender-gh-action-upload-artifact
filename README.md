# mender-push-artifact

A GitHub action to push your artifacts to a hosted Mender instance.

## Features / Limitations

The action supports uploading all artifact versions (v1, v2, v3) to an arbitrary Mender server.

A "personal access token" are used as authentication mechanism. Please read [the documentation](https://docs.mender.io/server-integration/using-the-apis#personal-access-tokens) on how to create one for your Github Actions pipeline setup.

## Usage

This action require the following inputs:

- `mender_pat`: personal access token on the hosted Mender instance to be used
- `mender_artifact`: path to the Mender Artifact to be uploaded, relative to `GITHUB_WORKSPACE`
- *artifact*: a Mender Artifact file (commonly with `.mender` suffix), placed in the `GITHUB_WORKSPACE` directory hierarchy

The action accepts the following optional inputs:

- `mender_uri`: URI for the Mender server to be used. Default: [hosted.mender.io](https://hosted.mender.io)

## Contributing

We welcome and ask for your contribution. If you would like to contribute to
Mender, please read our guide on how to best get started [contributing code or
documentation](https://github.com/mendersoftware/mender/blob/master/CONTRIBUTING.md).

To start editing right away, open the repository on [Gitpod](https://gitpod.io):

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/TheYoctoJester/mender-push-artifact)

## Connect with us

* Join the [Mender Hub discussion forum](https://hub.mender.io)
* Follow us on [Twitter](https://twitter.com/mender_io). Please
  feel free to tweet us questions.
* Fork us on [Github](https://github.com/mendersoftware)
* Create an issue in the [bugtracker](https://northerntech.atlassian.net/projects/MEN)
* Email us at [contact@mender.io](mailto:contact@mender.io)
* Connect to the [#mender IRC channel on Libera](https://web.libera.chat/?#mender)
