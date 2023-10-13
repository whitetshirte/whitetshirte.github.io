
## Keybindings

- <kbd>Numrow</kbd> Switch tabs
- <kbd>t</kbd> Open the create task panel
  - <kbd>Enter</kbd> Create a task
  - <kbd>Tab</kbd> Go to next field
- <kbd>s</kbd> Open the search dialog
- <kbd>Esc</kbd> Close the edit/create task panel (when field is focused)
### Tabs

Create new tabs and categories like so:

```js
const CONFIG = new Config({
    // ...
    openLastVisitedTab: false,
    tabs: [
        {
            name: 'boards',
            background_url: 'src/res/banners/bg-1.gif',
            categories: [{
                name: 'fun',
                links: [{
                    url: 'https://youtube.com',
                    name: 'youtube',
                    icon: 'brand-youtube',
                    icon_color: '#996767'
                }]
            }]
        }
    ]
)
```


### Clock




```js
const CONFIG = new Config({
  // ...
  clock: {
    format: 'h:i p',        // 13:30 PM
    // format: 'do B Y - h:i', // 18th January 2021 - 13:30
    // format: 'h:i - m/b/Y',  // 13:30 - 3/Jul/2021
    iconColor: 'grey'
  }
});
```

### Weather temperature



```js
const CONFIG = new Config({
  // ...
  temperature: {
    location: 'New York',
    scale: 'C'
  }
});
```

