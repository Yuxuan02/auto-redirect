# Auto Redirect
This is a chrome extension that allow you to open pages in current tab instead of new tab on customized domain.

## Install
This extension has not been uploaded to the chrome extension store yet, so you need to clone this repository, build it and load it manually.

```bash
git clone https://github.com/lorenzoc25/auto-redirect && cd auto-redirect
yarn build
```
or if you are using npm
```
npm build
```
The extension will then be built on `./auto-redirect/dist` path.

Then, turn on the chrome developer mode by going to `chrome://extensions/` and toggle the developer mode on the upper-right corner.

After turning on the developer mode, select the 'load unpacked' option on the upper-left corner and load the built version on `./auto-redirect/dist`. You should then be ready to go!

## Usage
After loading the extension, you can find it on the chrome extension section. Clicking on the icon would give you an user interface. Simply type in the domain names and this extension will automatically work on them! 

Note: currently, the extension achieve its functionally by using `url.include('rules')` to detect if it should change new tab to redirect in `url`. Thus, a suggested way to include rules is to type the full domain name like `bilibili.com`.

## Future Plans
- Improve on UI
- Regex matching on rules
- Deleting rules / temporarily disable them (WIP)
- Forbid adding duplicate rules
- Add rules that open pages in new tab instead of redirection (WIP)

## Contributing
To contribute, please fork this repository and open a pull request