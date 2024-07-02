# Installing Binaries from a GitHub Release on Ubuntu

This guide provides steps to download and install our released binaries from the drosera-network/releases (you are here) repo on  GitHub.

## Prerequisites

- `curl` installed (for downloading binaries)
- `tar` installed (for extracting binaries if they are compressed)
- Basic command line knowledge

## General Steps to Install Binaries

1. **Download the Binary**

    Use `curl` to download the binary from the GitHub release page. You can get the web link by copying the link from the Releases page of the release you are trying to install binaries from.

    ```sh
    # Using curl
    curl -L https://web-link-to-release-tarball
    ```
2. **Unarchive the Binary**
    Use tar to unarchive and unzip the file.  The file to untar will depend on the binary you downloaded in the previous step
    ```sh
    tar xzvf name-of-binary.tar.gz
    ```
3. **Installing the Binary**
    Use `chmod` to make the file executable
    ```sh
    chmod +x name-of-binary
    ```

4. **Move the binary to a location in the system PATH**
    Use `mv` or `cp` to mv the binary.  This may require sudo and a privileged user.  If you wish to place the executable binary in a different location, you will need to confirm that the location is part of the `$PATH` variable.
    ```sh
    mv operator /usr/bin/
    ```

### Docs
- Checkout our [Official Docs](https://dev.drosera.io) for configuring and running these binaries on your system.
