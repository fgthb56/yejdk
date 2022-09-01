## 一键部署 Gost(ss+mws) 到 heroku  [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2Ffkhjrighyyi%2Fyuidh)

> ```
>    gost.exe -L=:1080 -F=ss+mwss://method:password@appname.herokuapp.com:443
> ```

```js
addEventListener(
    "fetch",event => {
    let url=new URL(event.request.url);
    url.hostname="xxx.herokuapp.com";
    let request=new Request(url,event.request);
    event. respondWith(
      fetch(request)
    )
  }
)
```
