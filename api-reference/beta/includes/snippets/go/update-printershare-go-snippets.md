---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)

requestBody := graphmodels.NewPrinterShare()
displayName := "ShareName"
requestBody.SetDisplayName(&displayName) 
allowAllUsers := true
requestBody.SetAllowAllUsers(&allowAllUsers) 
additionalData := map[string]interface{}{
	"odataBind" : "https://graph.microsoft.com/beta/print/printers/{id}", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Print().SharesById("printerShare-id").Patch(context.Background(), requestBody, nil)


```