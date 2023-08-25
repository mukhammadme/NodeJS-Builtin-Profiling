# Example app for Node.JS Profiling

## Start Node.js application in profile mode

```bash
NODE_ENV=production node --prof app.js
```

## Generate profile statistics

```bash
node --prof-process isolate-0xnnnnnnnnnnnn-v8.log > processed.txt
```

## Commands to benchmark

```bash
curl -X GET "http://localhost:3000/newUser?username=matt&password=password"  
ab -v -k -c 20 -n 250 "http://localhost:3000/auth?username=matt&password=password"
```

## References

- [Easy profiling for Node.js Applications](https://nodejs.org/en/docs/guides/simple-profiling)
