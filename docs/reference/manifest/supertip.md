---
title: Supertip element in the manifest file
description: ''
ms.date: 05/07/2019
localization_priority: Normal
---

# Supertip

Defines a rich tooltip (both Title and Description). It is used by both [Button](control.md#button-control) or [Menu](control.md#menu-dropdown-button-controls)  controls.

## Child elements

|  Element |  Required  |  Description  |
|:-----|:-----|:-----|
| [Title](#title) | Yes | The text for the supertip. |
| [Description](#description) | Yes | The description for the supertip.<br>**Note**: (Outlook) Only Windows and Mac clients are supported. |

### Title

Required. The text for the supertip. The  **resid** attribute must be set to the value of the **id** attribute of a **String** element in the **ShortStrings** element in the [Resources](resources.md) element.

### Description

Required. The description for the supertip. The  **resid** attribute must be set to the value of the **id** attribute of a **String** element in the **LongStrings** element in the [Resources](resources.md) element.

> [!NOTE]
> For Outlook, only Windows and Mac clients support the **Description** element.

## Example

```xml
<Supertip>
    <Title resid="funcReadSuperTipTitle" />
    <Description resid="funcReadSuperTipDescription" />
</Supertip>
```
