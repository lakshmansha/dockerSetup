# Cordova Build Setup

Status: Completed

> Image for Build the Cordova Mobile Apps.

## Sofware Contains

| Software  | Version  | Source Link  |
|---|---|---|
| NodeJs  | 10.15.0  | **[Click Here](https://nodejs.org/dist/v10.15.0/node-v10.15.0-linux-x64.tar.gz)**  |
| NPM  | Latest | - |
| @NGX-ROCKET/SCRIPTS  | Latest | - |
| Cordova  | Latest  | - |
| GULP  | Latest  | - |
| Bower  | Latest  | - |
|   |   |   |

## Solution Setup Required

> Please Add npm scripts on name **"docker"** with our command to run on docker.

 As below on package.json

```npm
"scripts": {
    ...
    "docker": "cordova build android --device"
    ...
  },

```

## Docker Commands

For Build the Docker Image:

```bash
docker build -t cordova-setup:<tag> -f ./cordova/Dockerfile .

```

For Run the Docker Image:

On PowerShell:

```bash
docker run -it --rm -v ${PWD}:/application cordova-setup:<tag>

```

On CommandLine:

```bash
docker run -it --rm -v %cd%:/application cordova-setup:<tag>

```

## Examples

For Run the Docker Image:

```bash
docker run -it --rm -v "<path>":/application  cordova-setup:<tag>

```
