Get the most recent body fat percentage. The percentage value is a number between 0 and 100.

On success, the callback function will be provided with a `bodyFatPercentage` object containing the body fat percentage `value`, and the `startDate` and `endDate` of the sample. *Note: startDate and endDate will be the same as bodyFatPercentage samples are saved at a specific point in time.*

```javascript
AppleHealthKit.getLatestBodyFatPercentage(null, (err: Object, results: Object) => {
  if (err) {
    return;
  }
  console.log(results)
});
```

```javascript
{
	value: 20,
	startDate: '2016-07-08T12:00:00.000-0400',
	endDate: '2016-07-08T12:00:00.000-0400'
}
```