---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')"
requestBody.SetOdataId(&odataId) 

graphClient.Policies().MobileDeviceManagementPoliciesById("mobilityManagementPolicy-id").IncludedGroups().Ref().Post(context.Background(), requestBody, nil)


```