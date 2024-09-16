# yayata-common

Repository for locally bootstrapping 925r and Yayata.

## Dependencies

- [Git](https://git-scm.com/)
- [Taskfile](https://taskfile.dev/)
- [Docker with Compose v2](https://docs.docker.com/compose/)

## Installation

Create a new directory for all [925r](https://github.com/inuits/925r) and [Yayata](https://github.com/inuits/yayata) repositories to live in:

```
mkdir -p ~/inuits/yayata-application
```

Step inside that newly created directory.

```
cd ~/inuits/yayata-application
```

Clone this repository from [GitHub](https://github.com/inuits/yayata-common):

```
git clone --branch feature/metalarend/local-setup --single-branch https://github.com/inuits/yayata-common.git
cd yayata-common
```

Step inside that newly pulled directory.

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

Use GoTask to start both 925r and Yayata:

```
task start
```
                     
Open your browser on [http://localhost:8000](http://localhost:8000) for the 925r application.

Open your browser on [http://localhost:8080](http://localhost:8080) for the Yayata application.

The credentials for Yayata can be found in the Yayata .env file.

For more details, check the Yayata or 925r README.md files.
