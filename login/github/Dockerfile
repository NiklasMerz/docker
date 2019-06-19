FROM docker:stable

LABEL "name"="Docker Login Action for Github Packages"
LABEL "maintainer"="GitHub Actions <support+actions@github.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.icon"="log-in"
LABEL "com.github.actions.color"="blue"
LABEL "com.github.actions.name"="Github Packages"
LABEL "com.github.actions.description"="This is an Action to log into the docker registry of Github packages."
COPY LICENSE README.md THIRD_PARTY_NOTICE.md /

ENTRYPOINT echo "$GITHUB_TOKEN" | docker login  docker.pkg.github.com --username $DOCKER_USERNAME --password-stdin
