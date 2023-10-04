---
description: BASE URL --> https://luadeck.vercel.app
---

# API Endpoints & Usage

{% swagger method="post" path="/beautify" baseUrl="https://luadeck.vercel.app" summary="Beautify Endpoint" %}
{% swagger-description %}
Beautifies the given base-64 encoded Lua code\
\
`Any missing header is regarded as false`
{% endswagger-description %}

{% swagger-parameter in="header" name="solvemath" type="string" required="false" %}
Solve Math or not (true/false)
{% endswagger-parameter %}

{% swagger-parameter in="header" name="renamevariables" type="string" %}
Rename Variables or not (true/false)
{% endswagger-parameter %}

{% swagger-parameter in="body" name="body" type="raw text" required="true" %}
Your base-64 encoded code
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Response was returned" %}
Message body will return your code result.
{% endswagger-response %}

{% swagger-response status="413: Payload Too Large" description="Too large payload" %}

{% endswagger-response %}
{% endswagger %}

{% swagger method="post" path="/minify" baseUrl="https://luadeck.vercel.app" summary="Minify Endpoint" %}
{% swagger-description %}
Minifies the given base-64 encoded Lua code\
\
`Any missing header is regarded as false`
{% endswagger-description %}

{% swagger-parameter in="header" name="solvemath" type="string" required="false" %}
Solve Math or not (true/false)
{% endswagger-parameter %}

{% swagger-parameter in="header" name="renamevariables" type="string" %}
Rename Variables or not (true/false)
{% endswagger-parameter %}

{% swagger-parameter in="body" name="body" type="raw text" required="true" %}
Your base-64 encoded code
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Response was returned" %}
Message body will return your code result.
{% endswagger-response %}

{% swagger-response status="413: Payload Too Large" description="Too large payload" %}

{% endswagger-response %}
{% endswagger %}

