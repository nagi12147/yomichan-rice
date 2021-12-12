# Yomichan Rice + JMdict Fix
* Minimal Color
* Fix [JMdict](https://foosoft.net/projects/yomichan/#dictionaries) format to be readable in yomichan and anki card

## BEFORE
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/Before-1.png">
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/Before-2.png">
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/Before-3.png">

## AFTER
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/After-1.png">
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/After-2.png">
<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/After-3.png">

## Installation
1. Go to Yomichan Settings > **Appearance** > **Configure custom CSS…** > Copy and Paste the **[Popup.css](https://github.com/nagi12147/yomichan-rice/blob/main/Popup.css)** content to Popup CSS
2. Turn off **Compact glossaries**, *(optionally)* You could follow the settings below to match my rice

<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/settings.png">

1. Scroll down to **Anki** > **Configure Anki card templates…** > Copy and Paste the **[Handlebars.js](https://github.com/nagi12147/yomichan-rice/blob/main/Handlebars.js)** content to Anki Card Templates
2. Open **Configure Anki card format…** > use `{test}` as your JMdict/English Definition for anki cards. *Make sure you ordered JMdict as your first dictionary*

<img width="500" mheight="500" src="https://github.com/nagi12147/yomichan-rice/blob/main/Screenshot/ankicards.png">

3. Open your Anki > `CTRL+SHIFT+N` or **Tools-Manage Note Types** > Select your prefered Note type > **Cards** > **Styling** > Add this following code to your Styling:

```css
/* Yomichan Definition Fix */
ol {
	margin: 0;
	padding: 0;
	list-style-position: inside;
}
```
## Other
Difference between the default yomichan handlebars and this **[here](https://www.diffchecker.com/RFGbVBTx)**.

Rather than using `{glossary}` to export all definition into Anki, the purpose of `{test}` was only for the first ordered dictionary and not the others.

## Resources
* [stegatxins0#7346 Mining Setup](https://rentry.co/mining) (Yomichan setup)
* [AnimeCards](https://animecards.site/ankisetup/) (Anki and the handlebars setup)
* [TheMoeWay/Yomichan Custom CSS](http://learnjapanese.moe/yomicss/) (How to custom yomichan css)
* [FooSoft/yomichan/display.css](https://github.com/FooSoft/yomichan/blob/master/ext/css/display.css) (To check the css)
* [Garic#9392 Custom Yomichan Color](https://docs.google.com/document/d/1zVeG8sLhPj7rLKj4f0gqGr_FtHXVPpBgg4LwCPkKUTk/edit?usp=sharing)
