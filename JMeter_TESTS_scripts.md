

----------

Jmeter:
token
$.token

**Скрипт** в login

${__setProperty(token,${token})}


**Скрипт** в stepping Thread Group_first_test

String auth_token = props.get("token");
vars.put("token", auth_token);


в Http reqvest:

auth_token значение    ${token}

----------
url: 116.203.27.46 :5002

andpoint: /login

name: Dmitry_Sh

passvord: qwerty