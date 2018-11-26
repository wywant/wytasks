# 查看缺少的Authorizations
运行t-code SU53
# 查看用户的Authorizations
运行t-code SUIM查看
# 维护对象的Authorizations
运行 t-code SU22
# 查看Authorization Objects
运行SU21
# 问题
## No RFC authorization for function module
### 解决方案（没有经过测试）
让用户有对应的function module的S_RFC权限， 
在SU22中给指定的Function Moduel添加S_RFC权限，这应该会在Function Module层次上添加Authorization,而不需要添加到用户。

### Authorization Object S_RFC 
#### Definition
Authorization check when using RFC to access program modules (such as function groups)

#### Defined Fields
This authorization object contains the following three fields:  

RFC_TYPE: Type of the RFC object that is being protected  

Currently, this field can take the value FUGR (function group).  

RFC_NAME: Name of the RFC object that is being protected  

Currently, this field contains the names of function groups. It can have a maximum of 18 characters. Only 18 characters can be checked.  

ACTVT: Activity  

Currently, this field can take the value 16 (Execute).  
### Example
If you want a user to be able to execute function modules from the group ABCD in the target system, then this user needs the following authorization in the target system:
Activity: 16

Name of the RFC object that is being protected: ABCD

Type of the RFC object that is being protected: FUGR

### References
https://help.sap.com/saphelp_nw70/helpdata/en/60/305140c770cd01e10000000a155106/content.htm?no_cache=true
