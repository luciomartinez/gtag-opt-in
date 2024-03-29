# [GTag Opt In](https://www.npmjs.com/package/gtag-opt-in) &middot; [![Tests Status](https://github.com/luciomartinez/gtag-opt-in/workflows/Node.js%20CI/badge.svg)](https://github.com/luciomartinez/gtag-opt-in/actions)
> Google Analytics Opt In

> [!WARNING] 
> I'm deprecating this package as it requires more time, than what I can give, to keep it up-to-date so that the dependencies remain secure.
> My recommendation would be to read the source code and implement it in your website instead, as it should be easy enough yet secure.

GTag Opt In is a browser library to opt-in in Google Analytics.
Plus, it configures Analytics to [anonymize IP](https://support.google.com/analytics/answer/2763052).
See _why_ and _when_ to use it by reading the [wiki](https://github.com/luciomartinez/gtag-opt-in/wiki) page. 

## Install

### NPM

    npm install gtag-opt-in

### Yarn    

    yarn install gtag-opt-in
    
### HTML

    <script src="https://www.npmcdn.com/gtag-opt-in"></script>

It imports the library as the `GTagOptIn` global variable.

## Use

### ES6
```
import * as GTagOptIn from 'gtag-opt-in';

GTagOptIn.register('UA-XXXXXXXXX-Y');
GTagOptIn.optin();
GTagOptIn.optout();
```

### HTML
```
<script>
  GTagOptIn.register('UA-XXXXXXXXX-Y');
  GTagOptIn.optin();
  GTagOptIn.optout();
</script>
```

## Documentation
Further documentation can be found at the [wiki](https://github.com/luciomartinez/gtag-opt-in/wiki) page.

## Future
The library destiny is to be replaced with official support once Google Analytics releases the [Consent mode](https://support.google.com/analytics/answer/9976101) feature which is currently under beta.
 
## License
Software licensed under MIT license. See the [LICENSE](/LICENSE) file.
