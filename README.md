# AsTeRICS Grid
App for creating a flexible grid system that can be used for **Augmentative and Alternative Communication (AAC)**, for **Smart Home control** and as a **webradio** or **YouTube player**.

## Core features
These are the most important features of AsTeRICS Grid:
* **Cross platform**: runs on PC, Smartphone, Tablet, Windows, Linux, Android, iOS
* **No installation** needed, just open https://grid.asterics.eu/ in the browser
* Once loaded, AsTeRICS Grid **runs offline** without internet connection
* Optionally **synchronize configuration** using the cloud (data is end-to-end encrypted)
* Very **flexible grid system**, layouts are completely customizable
* **Text-to-speech** in various languages
* **Internationalization**: create grid sets in multiple languages
* **Various input possibilities** like Clicking, Tapping (on touchscreen), Hovering, Scanning, Keyboard, Buttons, and even more complex ones like Eye-Tracking, Head-Tracking or use of EMG muscle sensors (using the AsTeRICS Framework)
* Integrated search for **open AAC symbols** from https://www.opensymbols.org/
* **Smart Home control** (using the AsTeRICS Framework)
* **Flexible keyboard layouts** with **word prediction** and **self-learning dictionaries**
* **Play webradios** (over 25000) using [radio-browser.info](http://www.radio-browser.info/gui/#!/)
* **Search and play YouTube videos**

## Production environments
There are two versions of AsTeRICS Grid online:
* https://grid.asterics.eu/ current stable release
* https://grid.asterics.eu/latest/ current testing (beta) release, possibly unstable

## Documentation
See [User documentation](docs/documentation_user/README.md) or [AsTeRICS Grid Playlist on YouTube](https://www.youtube.com/playlist?list=PL0UXHkT03dGrIHldlEKR0ZWfNMkShuTNz).

Also see [Developer documentation (not finished, maybe outdated)](docs/documentation_dev/README.md) and the [Collaboration guide](docs/documentation_dev/collaboration.md).

## Run project locally
1. clone the project `git clone git@github.com:asterics/AsTeRICS-Grid.git`
2. install node.js https://nodejs.org/
3. install yarn, see https://yarnpkg.com/
4. go to the directory of the cloned project and run `yarn install`
5. run `npm run start` and open http://localhost:9095

## Npm scripts
After `yarn install` the following commands are available:
1. `npm run start` --> starts a webserver serving the AsTeRICS grid on `http://localhost:9095`, does hot reloading if js-sources change.
1. `npm run start-legacy` --> same as `start` but js sources are transformed to ES5 using babel.
1. `npm run start-no-live` --> same as `start` but hot reloading is disabled.
2. `npm run build` --> builds the js-files in folder `src` to `app/build` folder.
3. `npm run start-superlogin-dev` --> runs [superlogin](https://github.com/colinskow/superlogin) locally and makes it possible to create "online users" within the locally running application. A local [CouchDb](https://couchdb.apache.org/) instance is necessary in order to work.
4. `npm run release` -> releases the current version with a new tag and push it to `gh-pages` branch in order to be served at https://grid.asterics.eu/
5. `npm run release-latest` -> same as `npm run release` but with destination https://grid.asterics.eu/latest/
5. `npm run test` -> runs tests of the project using [Jest](https://jestjs.io/).

## History
The AsTeRICS Grid evolved out of [AsTeRICS Ergo](https://github.com/asterics/AsTeRICS-Ergo), see [AsTeRICS Ergo Master Plan](https://github.com/asterics/AsTeRICS-Ergo/wiki/Master-Plan-AsTeRICS-Ergo) and [AsTeRICS Ergo Architecture](https://github.com/asterics/AsTeRICS-Ergo/wiki/Architecture) and will eventually replace AsTeRICS Ergo.

## Support us
If you want to support the development of AsTeRICS Grid or contribute to the costs for running the server/database for syncronization you're very welcome to donate:

<div>
<a title="Donate with PayPal" href="https://www.paypal.com/donate/?hosted_button_id=38AJJNS427MJ2" target="_blank" style="margin-right:3em">
<img src="https://github.com/asterics/AsTeRICS-Grid/raw/master/app/img/donate-paypal.png" width=300/></a>
<span>&nbsp;&nbsp;&nbsp;</span>
<a title="Donate at opencollective.com" href="https://opencollective.com/asterics-foundation/projects/asterics-grid" target="_blank">
<img src="https://github.com/asterics/AsTeRICS-Grid/raw/master/app/img/donate-open-collective.png" width=300/></a>
</div>

## Acknowledgements and Attribution
Most of the work for AsTeRICS Grid has been accomplished at the [UAS Technikum Wien](https://www.technikum-wien.at/) in course of the R&D-projects *ToRaDes* (MA23 project 18-04) and *WBT* (MA23 project 26-02), which have been supported by the [City of Vienna](https://www.wien.gv.at/kontakte/ma23/index.html),
see: [ToRaDes Project Information](https://embsys.technikum-wien.at/projects/torades/index.php), [Webpage WBT project](https://wbt.wien).

<img src="https://github.com/asterics/AsTeRICS-Grid/assets/2537025/290d809f-1ccf-4362-be68-f07ff0e21878" width="400"/>
<br/><br/>

Other people and organizations we want to thank:
* Thanks to [ARASAAC](https://arasaac.org/) for collaborating and providing their pictogram API
* Thanks to [crowdin.com](https://crowdin.com/project/asterics-grid) for providing a free open source license
* Thanks to [browserstack.com](https://browserstack.com/) for providing us free UI tests on their platform.
* Thanks to Alex Segler for the great Webradio API [radio-browser.info](http://www.radio-browser.info/) which makes it possible to search and play webradios within AsTeRICS Grid
* Thanks to the makers of the API from [opensymbols.org](https://www.opensymbols.org/) which makes it possible to search for open AAC symbols within AsTeRICS Grid
* Thanks to ResponsiveVoice for providing an free non-commercial version, <a href="https://responsivevoice.org">ResponsiveVoice-NonCommercial</a> licensed under <a href="https://creativecommons.org/licenses/by-nc-nd/4.0/"><img title="ResponsiveVoice Text To Speech" src="https://responsivevoice.org/wp-content/uploads/2014/08/95x15.png" alt="95x15" width="95" height="15" /></a>
* Thanks to all the developers of these projects, which are all used by AsTeRICS Grid in production:
    * [core-js](https://github.com/zloirock/core-js)
    * [couch-auth](https://github.com/perfood/couch-auth)
    * [dom-i18n](https://github.com/ruyadorno/dom-i18n)
    * [file-saver](https://www.npmjs.com/package/file-saver)
    * [fontawesome](https://fontawesome.com/)
    * [GridList](https://github.com/hootsuite/grid)
    * [hls.js](https://github.com/video-dev/hls.js/)
    * [html2canvas](https://github.com/niklasvh/html2canvas)
    * [jszip](https://stuk.github.io/jszip/)
    * [jQuery](https://jquery.com/)
    * [jQuery context menu](https://swisnl.github.io/jQuery-contextMenu/)
    * [jQuery UI](https://jqueryui.com/)
    * [loglevel](https://github.com/pimterry/loglevel)
    * [navigo](https://github.com/krasimir/navigo)
    * [n-ary-huffman](https://github.com/lydell/n-ary-huffman)
    * [Object Model](https://objectmodel.js.org/)
    * [PouchDB](https://pouchdb.com/)
    * [predictionary](https://github.com/asterics/predictionary)
    * [Stanford Javascript Crypto Library (SJCL)](https://crypto.stanford.edu/sjcl/)
    * [superlogin-client](https://www.npmjs.com/package/superlogin-client)
    * [Vue.js](https://vuejs.org/)
    * [Workbox](https://github.com/GoogleChrome/workbox)
