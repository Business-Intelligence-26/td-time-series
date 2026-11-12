
1. I would make a test API request for 90 days and check the dates returned. That would show whether real history was available before deciding to use fake data.

2. I expect CO2 to rise from late summer into autumn because plants absorb less CO2 as their growth slows.

3. Finding no gaps once does not mean every future download will be complete.

4. I would use the rolling mean to follow a gradual weekly trend and exponential smoothing to react faster to a sudden change. I still need to compare this with my actual output after Step 

5. If all four API attempts fail, the workflow stops before analysis and committing. After a successful earlier run, the dashboard keeps showing the old data; on the first failed run, it would still have the placeholder.
