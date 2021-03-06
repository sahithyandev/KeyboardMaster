# KeyboardMaster

KeyboardMaster is a small, simple library for handling keyboard shortcuts in Javascript.

The library is very small it's just **2.5 KiB** before minifying and **1.6 KiB** after minifying.  
Visit here to see, [LIVE DEMO](https://sahithyandev.github.io/KeyboardMaster/preview/).

If you find any problems (bugs or errors) while using KeyboardMaster, kindly create an issue explaining what is the problem and how to reproduce it.

<!-- It is around **2kb** minified and gzipped and **4.5kb** minified, has no external dependencies, and has been tested in the following browsers:

- Internet Explorer 6+
- Safari
- Firefox
- Chrome

It has support for `keypress`, `keydown`, and `keyup` events on specific keys, keyboard combinations, or key sequences. -->

## Getting started

**Caution I messed up with the git tags while working on it. I published v1.1 and then deleted. But it is still on jsdelivr. So don't use it, it is a older version**

1.  Include KeyboardMaster on your page before the closing `</body>` tag.   
    You can use the CDN to load the file or you can download it from the CDN and refer it locally.

    ```HTML    
    <!-- KeyboardMaster@v1.1 - latest released version -->
    <script src="https://cdn.jsdelivr.net/gh/sahithyandev/KeyboardMaster@v1.2/lib/index.js"></script>

    <!-- KeyboardMaster@v1.1 - latest, minified released version -->
    <script src="https://cdn.jsdelivr.net/gh/sahithyandev/KeyboardMaster@v1.2/lib/index.min.js"></script>
    ```
<!-- 
    Load latest commit @not-recommended
    <script src="https://cdn.jsdelivr.net/gh/sahithyandev/KeyboardMaster@latest/lib/index.js"></script>

        If it's not released as a version, you can use a commit's build version.
        To do this, you have to replace the `version` with `commit-id`
    <script src="https://cdn.jsdelivr.net/gh/sahithyandev/KeyboardMaster@7efa43d/lib/index.js"></script> -->

2.  Add some keyboard events to listen for

    ```html
    <script>
        document.body.addKeyBindings({
            seperator: ' + ', // If undefined, defaults to this value
            bindings: [
                {
                    keyBinding: 'ctrl + shift + :',
                    action: () => {
                        console.log('ctrl + shift + : pressed');
                    }
                },
                {
                    keyBinding: 'shift + tab',
                    action: () => {
                        console.log('shift + tab pressed');
                    }
                }
            ]
        });
    <script>
    ```

**NOTE**  
You can try KeyboardMaster now. But **I don't recommend you to use KeyboardMaster in production until it gets some popularity. I don't think it will happen.**

<!--
## Why KeyboardMaster?

There are a number of other similar libraries out there so what makes this one different?

-   There are no external dependencies, no framework is required
-   You can programatically trigger key events with the `trigger()` method
- You are not limited to `keydown` events (You can specify `keypress`, `keydown`, or `keyup` or let KeyboardMaster choose for you).
- You can bind key events directly to special keys such as `?` or `*` without having to specify `shift+/` or `shift+8` which are not consistent across all keyboards
- It works with international keyboard layouts
- You can bind Gmail like key sequences in addition to regular keys and key combinations
- It works with the numeric keypad on your keyboard
- The code is well documented/commented -->

## Why KeyboardMaster?

There are a number of other similar libraries out there so what makes this one different?

-   There are no dependencies, No more incompatibility issues.
-   You can bind certain keyboard shortcuts to certain elements.

<!-- ## Developer Note

- KeyboardMaster extends the **HTMLElement** object with some methods. -->

## Documentation

Documentation for this library is being built. Take a look, give feedback.

Visit [DOCUMENTATION.md](./Documentation.md).

## Examples

* [Conway's Game of Life](https://sahithyandev.github.io/conways-game-of-life/)