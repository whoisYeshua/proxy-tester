## Install

```bash
git clone https://github.com/whatbotisthis/proxy-tester.git
cd proxy-tester
npm install
```


## Configure
Add proxies one per line in format `ip:port:user:pass` to `proxies.txt`

Modify domain, delay, threshold, and timeout settings in `config.json`
```javascript
{
  "delay": 50, // delay in ms between sending requests
  "domain": 'https://www.sixflags.com/',
  "timeout": 50000,
  "thresholds": { // times in ms
    "good": 1000, // less than this is good
    "bad": 5000 // greater than this is bad
  }
};
```


## Run
```bash
npm start
```
