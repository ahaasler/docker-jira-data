# docker-jira-data

A data-only container ready to be used with [docker-jira](https://github.com/ahaasler/docker-jira "docker-jira repo").

## Usage

1. Create and name the data-only container:

```bash
docker run --name jira-data ahaasler/jira-data
```

2. Use it in the jira container:

```bash
docker run --name jira --volumes-from jira-data -d -p 7990:7990 -p 7999:7999 ahaasler/jira
```

> See [docker-jira](https://github.com/ahaasler/docker-jira "docker-jira repo") for more information on the jira container.

## Thanks

* [Docker](https://www.docker.com/ "Docker") for this amazing container engine.
* [Atlassian](https://www.atlassian.com/ "Atlassian") for making great products. Also for their work on [atlassian-docker](https://bitbucket.org/atlassianlabs/atlassian-docker "atlassian-docker repo") which inspired this.
* [Azul Systems](http://www.azulsystems.com/ "Azul Systems") for their *OpenJDK* docker base image.
* And specially to you and the entire community.

## License

This image is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for the full license text.
