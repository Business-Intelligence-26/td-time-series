1. I would make a test API request for 90 days and check the dates returned. That would show whether real history was available before deciding to use fake data.

2. I expected CO2 to rise from late summer into autumn because plants absorb less CO2 as their growth slows. 

3. My run found no gaps, but that does not guarantee every download will be complete. I would keep the check because future data or a physical sensor could have missing readings.

4. I would use the rolling mean for the weekly trend and exponential smoothing to notice recent changes. In my PM2.5 results, the rolling mean stayed near 22 while exponential smoothing fell from 24.14 to 18.51 as recent values dropped.

5. If all four API attempts fail, the workflow stops before analysis and committing. After a successful earlier run, the dashboard keeps showing the old data; on the first failed run, it would still have the placeholder.

6. I would only use the PM2.5 projection as a rough guide for the next two days. It rises from 14.89 to 15.66 over seven days even though recent values fell, so I would not trust it to predict another sudden change.

7. The analysis functions use dates and numbers rather than a specific city or pollutant. After switching to Paris and PM2.5, I had to update the CSV field name, but the smoothing and projection calculations stayed the same.
