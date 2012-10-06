### Objective-C wrapper for XXTEA

#### Usage

    #import "NSString+XXTEA.h"
    
    NSString *plain_text = @"Hello xxtea";
    NSString *key = @"key";
    NSString *encryped = [plain_text encryptXXTEA:@"123"];
    
    NSLog(@"encrypted string is base64 encoded:%@",encryped);
    
    NSString *decryped = [encryped decryptXXTEA:@"123"];
    STAssertEqualObjects(plain_text, decryped,@"xxtea encypt/decrypt");


#### LICENSE
    
Apache 2.0

#### AUTHORS

original c source is from: http://code.google.com/p/xxtea-algorithm/

cocoa wrapper is written by Pan Fan(nightsailer)
