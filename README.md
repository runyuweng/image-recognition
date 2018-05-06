# ImageRecognition
## Introduce
A program to identify picture verification code.

## Interface
### Request parameters
| name | required | type | Instruction |
|:-------:|:-------------: | :----------:| :----------:|
| url | true | string | image url|

### Return parameters
| name | required | type | Instruction |
|:-------:|:-------------: | :----------:| :----------:|
| code | true | number | status code |
| msg | true | string | status message |
| data | true | json | image recognition result |

### JSON example
```
{
  code: 0,
  msg: 'success',
  data: {
    '污': { x: 100, y: 200 },
    '逢': { x: 100, y: 200 },
    '要': { x: 100, y: 200 },
  }
}
```