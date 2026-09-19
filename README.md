# router test project

This is the experimental release project for the generic Bash installer. The Nim source is intentionally small; the release protocol is language-neutral.

The workflow builds the `example` executable for Linux x86_64 baseline and x86-64-v3 targets, computes SHA-256 and byte sizes, generates `install.manifest`, and publishes a tagged GitHub Release.

After publishing `v0.1.0` from a repository named `gabrielcapilla/router`, test the separate experimental website endpoint with:

```bash
curl -sL gabrielcapilla.github.io/experimental | bash -s router
```

The production `/install` endpoint is intentionally not involved in this experiment.
