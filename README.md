oc new-build https://github.com/monkalways/sonarqube.git --strategy=docker --name=sonarqube --to=sonarqube:7.9

oc new-app -f sonarqube-postgresql-template.yaml --param=SONARQUBE_VERSION=7.9
