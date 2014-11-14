# hr-time-js

Simple human-readable timestamps

## Usage

`new HRTime(Date then, [Object options])` returns a human-readable timestamp.

### Options

`options` can include the following keys:

+ __`Date now`__

    Date to calculate time difference from.

    _Default_: `new Date()`
    

+ __`Boolean roundDown`__

    Whether or not to round time differences down.
    
    _Default_: `false`

### Example usage and output

```javascript
new HRTime(new Date("13 Nov 2014 20:05 GMT+0800"), {
    now: new Date("13 Nov 2014 20:55 GMT+0800"),
    roundDown: true
});
  
// returns
{
    time: 50
    unit: "minute",
}
```