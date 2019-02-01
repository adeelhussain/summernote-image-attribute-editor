# summernote-image-title
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

Adds a button to the image popover to edit title and alt and caption.

### Installation

#### 1. Include JS


Include the following code after Summernote:

```html
<script src="summernote-image-attributes.js"></script>
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
        	figureClass: 'figure',
        	figcaptionClass: 'fiffff',
        	captionText: 'Caption Goes Here.'
        },
        lang: 'en-US',
        popover: {
            image: [
                ['imagesize', ['imageSize100', 'imageSize50', 'imageSize25']],
                ['float', ['floatLeft', 'floatRight', 'floatNone']],
                ['remove', ['removeMedia']],
                ['custom', ['imageAttributes']],
            ],
        },
    });
});
```

(Thanks to [@asiffermann](https://github.com/asiffermann))
(Thanks to [@DiemenDesign](https://github.com/DiemenDesign))