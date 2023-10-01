# A Kubernetes HELM Chart for the ERDDAP application

Based on, and extending the work done in dockerizing ERDDAP: [erddap-gold-standard](https://ioos.github.io/erddap-gold-standard/)

## Install this chart

You likely want to make at least a minimum configuration values.yaml from the following:


```
domain:
  enabled: true
  name: your.domain.name

config:
  enabled: true
  variables: |-
    ERDDAP_adminInstitution="your institution"
    ERDDAP_adminEmail="youremail@example.com"
```

Clone this repository to a machine with the helm binary from [helm.sh](https://helm.sh), review the default values, and install.

```
git clone https://github.com/kumulustech/erddap-helm.git
cd erddap-helm
helm install erddap .
```

## Contributing

Fork and submit a pull request.  We follow the code of conduct outlined in our [Code of Conduct](CODEOFCONDUCT.md) file in the root directory of the repository.
