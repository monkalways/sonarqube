oc new-build https://github.com/monkalways/sonarqube.git --strategy=docker --name=sonarqube --to=sonarqube:8.2

oc new-app -f sonarqube-postgresql-template.yaml --param=SONARQUBE_VERSION=8.2
