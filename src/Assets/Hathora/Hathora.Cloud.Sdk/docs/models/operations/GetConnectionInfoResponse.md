# GetConnectionInfoResponse


## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `ConnectionInfoV2`                                                                                               | [ConnectionInfoV2](../../models/shared/ConnectionInfoV2.md)                                                      | :heavy_minus_sign:                                                                                               | Ok                                                                                                               |
| `ContentType`                                                                                                    | *string*                                                                                                         | :heavy_check_mark:                                                                                               | HTTP response content type for this operation                                                                    |
| `GetConnectionInfo400ApplicationJSONString`                                                                      | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | N/A                                                                                                              |
| `GetConnectionInfo404ApplicationJSONString`                                                                      | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | N/A                                                                                                              |
| `GetConnectionInfo500ApplicationJSONString`                                                                      | *string*                                                                                                         | :heavy_minus_sign:                                                                                               | N/A                                                                                                              |
| `StatusCode`                                                                                                     | *int*                                                                                                            | :heavy_check_mark:                                                                                               | HTTP response status code for this operation                                                                     |
| `RawResponse`                                                                                                    | [UnityWebRequest](https://docs.unity3d.com/2021.3/Documentation/ScriptReference/Networking.UnityWebRequest.html) | :heavy_minus_sign:                                                                                               | Raw HTTP response; suitable for custom response parsing                                                          |