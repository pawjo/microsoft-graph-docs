---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewRenewGroupPostRequestBody()
groupId := "ffffffff-ffff-ffff-ffff-ffffffffffff"
requestBody.SetGroupId(&groupId) 

result, err := graphClient.GroupLifecyclePolicies().RenewGroup().Post(context.Background(), requestBody, nil)


```