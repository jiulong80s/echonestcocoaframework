# Prerequisite #

To be able to use this Framework, you need to get an [Echo Nest](EchoNest.md) API Key.
You can get one by registering with The Echo Nest on the following page.
http://developer.echonest.com/account/register/

Once you have a valid API Key, you'll be able to init an EchoNest object by using the method
```
EchoNest* nest = [[EchoNest alloc] initWithAPIKey:@"yourApiKey"];
```

The API Key you entered will be tested on the server. If valid, you can go on with the other methods, if not, you can enter a new one by using
```
[nest setApiKey:@"newApiKey"];
[nest validateApiKey];
```