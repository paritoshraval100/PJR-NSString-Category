PJR-NSString-Category
=====================

It is an NSString Category by which you can perform many NSString operations in your application.

It is very helpful for the beginers or even who are working with objective c.


By using this NSString Category you can perform many NSString operation which you normally need.No need to create any method
or any class.


HOW TO USE:
=====================

import this category in your controller by  #import "NSString+PJR.h" and you can perform all NSString operations given
in this category like

    //Examples of NSString Category
    
    NSString *testStr = @"Hello";
    
    if([testStr isValid]){
        NSLog(@"It is a Valid String");
    }
    
    NSString *blankStr = @"  ";
    if([blankStr isBlank]){
        NSLog(@"It is a blank String");
    }
    
    NSString *noOfWordsStr = @"Number of Words";
    NSLog(@"Number of words are :%d",[noOfWordsStr countNumberOfWords]);
    
    if([noOfWordsStr containsString:@"of"]){
        NSLog(@"YES");
    }
    
    if([noOfWordsStr isBeginsWith:@"N"]){
        NSLog(@"YES");
    }

    if([noOfWordsStr isEndssWith:@"s"]){
        NSLog(@"YES");
    }
    
    NSLog(@"string after replace charcter is :%@",[noOfWordsStr replaceCharcter:@"of" withCharcter:@"offfff"]);
    
    NSLog(@"Get substring :%@",[noOfWordsStr getSubstringFrom:1 to:6]);
    
    NSLog(@"Add string :%@",[noOfWordsStr addString:@" are 3"]);
    
    NSLog(@"Removed string :%@",[noOfWordsStr removeSubString:@"of"]);
    
    NSString *letterStr = @"abcd";
    NSString *numberStr = @"1234";
    NSString *letterNuberStr = @"sdf545";
    
    if([letterStr containsOnlyLetters]){
        NSLog(@"Contanis only letters");
    }

    if([numberStr containsOnlyNumbers]){
        NSLog(@"Contanis only numbers");
    }
    
    if([letterNuberStr containsOnlyNumbersAndLetters]){
        NSLog(@"Contanis letters and numbers");
    }
    
    NSArray *array = [NSArray arrayWithObjects:letterStr,numberStr,letterNuberStr, nil];
    if([numberStr isInThisarray:array]){
        NSLog(@"Yes number string is in this array");
    }
    
    NSLog(@"String from array is :%@",[NSString getStringFromArray:array]);
    
    NSLog(@"Array from String is :%@",[noOfWordsStr getArray]);
    
    NSLog(@"My Application Version number is :%@",[NSString getMyApplicationVersion]);
    
    NSLog(@"My Application name is :%@",[NSString getMyApplicationName]);
    
    if([@"pjr@gmail.com" isValidEmail]){
        NSLog(@"It is valid Email");
    }
    if(![@"21323gf" isVAlidPhoneNumber]){
        NSLog(@"It is not valid Phone number");
    }
    if([@"http://www.google.com" isValidUrl]){
        NSLog(@"It is valid URL");
    }
    
    
    Contact

    Paritosh Raval
    
    
    License
    
    Paritosh Raval


