# bj-router
Lightweight Router in vanilla javascript for the BuyerJourneyJS project.

## Sponsors
[<img src="https://www.conference.com.mx/web/image/website/3/logo/Conference?unique=cb769b7">](https://www.conference.com.mx/comercializacion-digital)

## Features
- Multiple routes with path and callback function.
- Single page application routing using hash.
- Parameters.
- Query strings.
- Set name on routes with setName(name) and retrieve the path with pathFor(name, parameters).
- Error 404: Callback function included.
- Error 404: Customizable Callback function.

## Example

```javascript
import { bjRouter } from  "@buyerjourney/router";
import { home, store, blog } from "./app/pages";

App = new bjRouter({ hashSensitive:true});
App.on('/', home);
App.on('#store/{product}', store);
App.on('#blog/{article}', blog);

App.run();
```

## Documentation 
- [BuyerJourneyJS project](https://buyerjourney.ninja/).
- [bj-router](https://buyerjourney.ninja/router).
- [Get started](https://buyerjourney.ninja/get-started).

## License
bj-router is [GPL-3.0-or-later](./LICENSE).