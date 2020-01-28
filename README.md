By Roker2

## libfpservice.so

Need to change to CMP X1, X0 or NOP

CMP X1, X0 = 3F 00 00 EB in HEX
NOP = 1F 20 03 D5 in HEX

Based on comparing Leeco S2 and Xiaomi Redmi 4X blobs

Maybe need to patch Aliplay functions

| Function                 | Patch place | Patch status (patched or not) |
| :----------------------- | :---------- | :---------------------------- |
| android::notifyClient    | 1B3F4       | yes                           |
| android::notifyClient    | 1B3F8       | yes                           |
| android::notifyClient    | 1B3FC       | yes                           |
| android::notifyClient    | 1B400       | yes                           |
| android::notifyClient    | 1B404       | yes                           |
| android::notifyClient    | 1B408       | yes                           |
| android::notifyClient    | 1B40C       | yes                           |
| android::notifyClient    | 1B410       | yes                           |
| android::notifyClient    | 1B414       | yes                           |
| android::notifyClient    | 1B418       | yes                           |
| android::notifyClient    | 1B420       | yes                           |
| android::postData2Client | 1C628       | yes                           |
| android::postData2Client | 1C62C       | yes                           |
| android::postData2Client | 1C630       | yes                           |
| android::postData2Client | 1C634       | yes                           |
| android::postData2Client | 1C638       | yes                           |
| android::postData2Client | 1C63C       | yes                           |
| android::postData2Client | 1C640       | yes                           |
| android::postData2Client | 1C644       | yes                           |
| android::postData2Client | 1C648       | yes                           |
| android::postData2Client | 1C64C       | yes                           |
| android::postData2Client | 1C654       | yes                           |

2 functions, 22 patch places