# Gradle SSH Plugin Template [![build](https://github.com/gradle-ssh-plugin/template/actions/workflows/build.yaml/badge.svg)](https://github.com/gradle-ssh-plugin/template/actions/workflows/build.yaml)

A template project with [Gradle SSH Plugin](https://github.com/int128/gradle-ssh-plugin).

## Getting Started

Clone the repository.

```bash
git clone https://github.com/gradle-ssh-plugin/template.git
cd template
```

Edit `build.gradle` and run Gradle.

```bash
./gradlew showPlatformVersion
```

We can dry run the script as follows:

```bash
./gradlew -PdryRun -i showPlatformVersion
```

## Development

### GitHub Codespaces

Start the server.

```console
$ sudo service ssh start
 * Starting OpenBSD Secure Shell server sshd
```

Generate a key pair and `known_hosts`.

```sh
ssh-keygen -t ecdsa -N '' -C '' -f ~/.ssh/id_ecdsa
tee -a ~/.ssh/authorized_keys < ~/.ssh/id_ecdsa.pub
ssh -v -p 2222 -o StrictHostKeyChecking=accept-new localhost true
```

Change the port to 2222.

```groovy
remotes {
    localhost {
        host = 'localhost'
        port = 2222
```
