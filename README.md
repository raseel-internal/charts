This is the official repository of Raseel helm charts.

### Maintainer: [hbadri@mda.gov.sa](mailto:hbadri@mda.gov.sa)

### Steps to add a new chart:

* Download the needed chart (if you are dealing with a customization of a sepcific chart like __datapusher__ in out case)
* Edit the chart `values.yaml`
* Build the chart : `helm package .`
* Create the appropriate folder: `newchart`
* Cp the tgz file into the new folder
* In the root folder, run the indexing:
`helm repo index --url https://raseel-internal.github.io/charts .`
