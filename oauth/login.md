# Login

{% api-method method="post" host="https://accounts.launcher-website-prod07.ol.epicgames.com" path="/login/doLauncherLogin" %}
{% api-method-summary %}
Login
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="X-XSRF-TOKEN" type="string" required=true %}
XSRF-TOKEN
{% endapi-method-parameter %}

{% api-method-parameter name="Authentication" type="string" required=true %}
Token type + Authentication token
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="fromForm" type="string" required=true %}
`yes`
{% endapi-method-parameter %}

{% api-method-parameter name="authType" type="string" required=true %}
`null`
{% endapi-method-parameter %}

{% api-method-parameter name="linkExtAuth" type="string" required=true %}
`null`
{% endapi-method-parameter %}

{% api-method-parameter name="client\_id" type="string" required=true %}
client\_id
{% endapi-method-parameter %}

{% api-method-parameter name="redirectUrl" type="string" required=true %}
https://accounts.launcher-website-prod07.ol.epicgames.com/login/showPleaseWait?client\_id=`clientId`&rememberEmail=false
{% endapi-method-parameter %}

{% api-method-parameter name="epic\_username" type="string" required=true %}
Email of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
Password of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="rememberMe" type="string" required=true %}
`NO`
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="post" host="https://accounts.launcher-website-prod07.ol.epicgames.com" path="/register/doLauncherRegister" %}
{% api-method-summary %}
Register
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Token type + Authentication token
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-body-parameters %}
{% api-method-parameter name="redirectUrl" type="string" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="country" type="string" required=true %}
Country of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}
FirstName of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="lastName" type="string" required=true %}
LastName of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="displayName" type="string" required=true %}
DisplayName of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}
Email of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
Password of the Account
{% endapi-method-parameter %}

{% api-method-parameter name="g-recaptcha-response" type="string" required=true %}

{% endapi-method-parameter %}

{% api-method-parameter name="termsAgree" type="string" required=true %}
`yes`
{% endapi-method-parameter %}

{% api-method-parameter name="register" type="string" required=true %}
`sign in`
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



