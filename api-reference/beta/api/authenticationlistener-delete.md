---
title: "Delete authenticationListener"
description: "Deletes an authenticationListener from an event supported by an authenticationEventsPolicy."
author: "jkdouglas"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Remove authenticationListener

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.

## Permissions

Choose the permission marked as least privileged for this API. Use a higher privileged permission only if your app requires it. For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "authenticationlistener_delete" } -->
[!INCLUDE [permissions-table](../includes/permissions/authenticationlistener-delete-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
