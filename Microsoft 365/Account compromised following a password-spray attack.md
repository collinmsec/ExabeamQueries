# Account compromised following a password-spray attack
*NOTE: Some of the fields that are being used may be different in your environment depending on parsing.*

<blockquote>

A password spray attack is where multiple identities are attacked using common passwords in a unified brute force manner. The risk detection is triggered when an account's password is valid and has an attempted sign in. This detection signals that the user's password was correctly identified through a password spray attack, not that the attacker was able to access any resources.

</blockquote>


```
product:"Microsoft Entra" AND alert_type:"passwordSpray"
```
Reference: https://learn.microsoft.com/en-us/entra/id-protection/concept-identity-protection-risks#password-spray
