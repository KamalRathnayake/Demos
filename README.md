# Azure Forms Regocognizer Demo
With sample files

## Uploading Training DataSet

`curl -X POST "{FORMS-ANALYZER-ENDPOINT}/formrecognizer/v1.0-preview/custom/train" -H "Content-Type:application/json" -H "Ocp-Apim-Subscription-Key:{SUBSCRIPTION-KEY}" --data-ascii "{ \"source\": \"{CONTAIER-SAS-URL}\"}"`

## Analyzing Document

`curl -X POST "{FORMS-ANALYZER-ENDPOINT}/formrecognizer/v1.0-preview/custom/models/{MODEL-ID}/analyze" -H "Content-Type: multipart/form-data" -F "form=@\"C:\One.pdf\";type=application/pdf" -H "Ocp-Apim-Subscription-Key:{SUBSCRIPTION-KEY}"`
