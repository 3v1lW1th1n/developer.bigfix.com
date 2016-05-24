---
title: Create Role
---

This command will POST the file `role.xml` to the server to create a new role.

[Sample Role XML File](./role.xml)

# python
```python
import requests
with open('role.xml') as xml:
	r = requests.post('https://server:port/api/roles', auth=('user', 'password'), data=xml)
	print(r.text)
```

# Input
## role.xml
```xml
<?xml version="1.0" encoding="UTF-8"?>
<BESAPI xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="BESAPI.xsd">
        <Role Resource="https://localhost:52311/api/role/id">
                <Name>name</Name>
                <ID>id</ID>
                <MasterOperator>0</MasterOperator>
                <CustomContent>1</CustomContent>
                <ShowOtherActions>1</ShowOtherActions>
                <CanCreateActions>1</CanCreateActions>
                <PostActionBehaviorPrivilege>AllowRestartAndShutdown</PostActionBehaviorPrivilege>
                <ActionScriptCommandsPrivilege>AllowRestartAndShutdown</ActionScriptCommandsPrivilege>
                <CanSendMultipleRefresh>1</CanSendMultipleRefresh>
                <CanLock>1</CanLock>
                <UnmanagedAssetPrivilege>ShowNone</UnmanagedAssetPrivilege>
                <InterfaceLogins>
                        <Console>true</Console>
                        <WebUI>true</WebUI>
                        <API>true</API>
                </InterfaceLogins>
        </Role>
</BESAPI>
```