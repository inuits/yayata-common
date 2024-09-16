# yayata-common

Repository for locally bootstrapping 925r and Yayata.

## Dependencies

- [Git](https://git-scm.com/) - [Installation](https://git-scm.com/download/linux)
- [Taskfile](https://taskfile.dev/) - [Installation](https://taskfile.dev/installation/#install-script)
- [Docker with Compose v2](https://docs.docker.com/compose/) - [Installation](https://docs.docker.com/compose/install/linux/)

## Installation

Create a new directory for all [925r](https://github.com/inuits/925r) and [Yayata](https://github.com/inuits/yayata) repositories to live in:

```
mkdir -p ~/inuits/yayata-application
```

Step inside the newly created directory.

```
cd ~/inuits/yayata-application
```

Clone this repository from [GitHub](https://github.com/inuits/yayata-common):

```
git clone --branch feature/metalarend/local-setup --single-branch https://github.com/inuits/yayata-common.git
```

Step inside the newly pulled directory.

```
cd yayata-common
```

Clone the 925r and Yayata repositories:

```
task clone
```

## Update

Pull the latest changes from the 925r and Yayata repositories:

```
task pull
```

## Usage

Start both 925r and Yayata:

```
task start
```
                     
Open your browser on [http://localhost:8000](http://localhost:8000) for the 925r application.

Open your browser on [http://localhost:8080](http://localhost:8080) for the Yayata application.

The credentials for Yayata can be found in the 925r .env file.

For more details, check the 925r and Yayata README.md files.
