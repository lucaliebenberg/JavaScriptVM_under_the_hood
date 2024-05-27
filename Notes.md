# Notes

- VM uses inline caching for performance
- VM cache is limited to 1024
- === is way faster than == as it does not execute .valueOf()
- When input data has a ton of different shapes, the VM need to do extra work and this decreases performance
- Dealing with data through the usage of Objects, is much slower than using Arrays
- Accessing more than 1024 properties of an Object (reading all values) will heavily impact performance as the VM will need to go through at data in memory and will not be able to retreive the answers from the cache (inline caching)
- Disabling 'inline' when runing Node, will help have a better understanding of the code execution and performance, but as a result your code will run slower (no usage of inline caching for performance)
- Executing '-0' will return a floating point number, which causes issue with the compiler as it uses integers to index the data location from memory