# Notes

- VM uses inline caching for performance
- VM cache is limited to 1024
- === is way faster than == as it does not execute .valueOf()
- When input data has a ton of different shapes, the VM need to do extra work and this decreases performance
- Dealing with data through the usage of Objects, is much slower than using Arrays
- Accessing more than 1024 properties of an Object (reading all values) will heavily impact performance as the VM will need to go through at data in memory and will not be able to retreive the answers from the cache (inline caching)