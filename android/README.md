
# Android Setup

Status: Completed

> Base Image for Android Setup to get required software for the Build.

## Sofware Contains

| Software  | Version  | Source Link  |
|---|---|---|
|  OpenJDK |  8 | **[from cmd](https://openjdk.java.net/install/)** |
| Android Tools  | 25.2.5 (Linux)  | **[Click Here](https://dl.google.com/android/repository/tools_r25.2.5-linux.zip)** |
| Android Build Tools  | 27.0.3  | -  |
| Android Platform Tools  | TBD By Tools  | -  |
| Android API  | 23, 26, 27, 28  | -  |
|   |   |   |

## Docker Commands

For Buid the Docker Image:

```bash
docker build -t android-setup:<tag> -f ./Dockerfile .

```

For Run the Docker Image:

```bash
docker run -it --rm android-setup:<tag>

```

On Docker Run --rm indicate to Remove the Container. If you required that container, please remove the command --rm.

## Examples

For Run the Docker Image:

```bash
docker run -it --rm android-setup:<tag>

```