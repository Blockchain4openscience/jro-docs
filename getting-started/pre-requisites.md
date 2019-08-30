# Pre-Requisites
You should have relevant Hyperledger Composer and Fabric versions installed, 
We follow the hyperledger-composer tutorial on [Developer tutorial for creating a Hyperledger Composer solution](https://hyperledger.github.io/composer/latest/tutorials/developer-tutorial).z

Make sure that you start a fresh Hyperledger Fabric network, that is you must teardown any previous Hyperledger Fabric constainer and delete any old business network card that may exist form previous Fabric enviorments. Guide on installing JRO Business Network Application (BNA) can be found here : https://github.com/Blockchain4openscience/jroBna

## CORS Plugin
For the developement environment to run, You need to install a CORS Plugin on your Browser. This allows cross origin requests to work in the browser. After developement session finishes, Please turn the plugin off for security reasons.
You can choose among the following plugins: 

* [CORS everywhere](https://addons.mozilla.org/es/firefox/addon/cors-everywhere/) for firefox
* [Moesif Origin](https://chrome.google.com/webstore/detail/moesif-origin-cors-change/digfbfaphojjndkpccljibejjbppifbc) for chrome