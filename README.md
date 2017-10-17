# pinblock

ATM PIN Block Service, used by [Electron ATM](https://github.com/timgabets/electron-atm). The module may be used for ATM PIN processing. 

## To use:
```javascript
const PINBlockService = require('pinblock');

var pinblock = new PINBlockService();
pinblock.get('1234', '4000001234562000')
> '041234FEDCBA9DFF'

pinblock.encode_to_atm_format('0123456789ABCDEF')
> '0123456789:;<=>?'

```
