# EasyPrefs
A light weight & elegent NSUserDefaults wrapper

# Perpose
Make NSUserDefaults more easy to use, treat preferences as properties

# Setup
```objc
#import "EasyPrefs.h"

@interface TINPrefs : EasyPrefs

@property (nonatomic, copy) NSString *name;
@property (nonatomic, assign) int age;

@end

#import "TINPrefs.h"

@implementation TINPrefs

EasyPrefsRegisterDefault(name, @"Cyan")
EasyPrefsRegisterDefault(age, @25)

@end
```

# Usage
```objc
[[TINPrefs instance] setName:@"Katrine"];
[[TINPrefs instance] setAge:18];
```

# That's all