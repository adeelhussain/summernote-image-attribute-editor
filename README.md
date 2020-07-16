# summernote-image-attributes
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

Adds a button to the image popover to edit title, alt, caption and resize along with managing of Aspect Ratio.

### 1. Installation

* #### Include JS
Include the following code after Summernote:

```html
<script src="summernote-image-attributes.js"></script>
<script src="lang/[language-COUNTRY].js"></script>
```

* #### Using npm
If you are using npm, run this command

```html
npm i summernote-image-attributes-editor --save
```

#### 2. Supported languages

Currently available in:
- English

Contributions are welcomed!

#### 3. Summernote options

Finally, customize the Summernote image popover.

```javascript
$(document).ready(function() {
    $('#summernote').summernote({
        imageAttributes: {
          	icon: '<i class="note-icon-pencil"/>',
        	figureClass: 'figureClass',
        	figcaptionClass: 'captionClass',
        	captionText: 'Caption Goes Here.',
        	manageAspectRatio: true // true = Lock the Image Width/Height, Default to true
        },
        lang: 'en-US',
        popover: {
            image: [
                ['image', ['resizeFull', 'resizeHalf', 'resizeQuarter', 'resizeNone']],,
                ['float', ['floatLeft', 'floatRight', 'floatNone']],
                ['remove', ['removeMedia']],
                ['custom', ['imageAttributes']],
            ],
        },
    });
});
```
#### 4. Demo
- [Demo](https://adeelhussain.github.io/summernote-image-attribute-editor/)


(Thanks to [@asiffermann](https://github.com/asiffermann))
(Thanks to [@DiemenDesign](https://github.com/DiemenDesign))
