swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UnsubscribeFromDataset:
    get:
      summary: Unsubscribe From Dataset
      description: Unsubscribes from receiving notifications when a dataset is modified
        by another device.
      operationId: unsubscribeFromDataset
      x-api-path-slug: actionunsubscribefromdataset-get
      parameters:
      - in: query
        name: DatasetName
        description: The name of the dataset from which to unsubcribe
        type: string
      - in: query
        name: DeviceId
        description: The unique ID generated for this device by Cognito
        type: string
      - in: query
        name: IdentityId
        description: Unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset