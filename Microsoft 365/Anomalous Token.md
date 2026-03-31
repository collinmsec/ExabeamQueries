# Anomalous Token
*NOTE: Some of the fields that are being used may be different in your environment depending on parsing.*
<blockquote>

This detection indicates abnormal characteristics in the token, such as an unusual lifetime or a token played from an unfamiliar location. This detection covers Session Tokens and Refresh Tokens.

</blockquote>

```
product:"Microsoft Entra" AND alert_type:"anomalousToken"
```
Reference: https://learn.microsoft.com/en-us/entra/id-protection/concept-identity-protection-risks#anomalous-token-user
