# 如何配置ak、sk<a name="dayu_06_0075"></a>

在test.c中，通过GetUserAuthInfo函数设置ak，sk。

```
DISStatus GetUserAuthInfo(char *ProjectId, char *akArray, char *skArray, char *xSecurityToken)
{
char *ak = "Provide your Access Key";
char *sk = "Provide your Secret Key";
printfdbgfunc;
strncpy(akArray, ak, strlen(ak));
strncpy(skArray, sk, strlen(sk));
printfdbgoutfunc;
return 0;
}
```

