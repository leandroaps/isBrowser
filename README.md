# isBrowser
This snippet can be used to determine whether the current runtime environment is a browser. This is helpful for avoiding errors when running front-end modules on the server (Node).
```
const isBrowser = () => ![typeof window, typeof document].includes('undefined');
```
**Usage:**
```
isBrowser(); // true (browser)
isBrowser(); // false (Node)
```
