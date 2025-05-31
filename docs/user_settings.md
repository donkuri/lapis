# Where do I find any of this ?
Lapis comes with a few variables that alters the way it looks. In order to change any variable, select a Lapis card in the Browser (`Browse`), then click on `Cards` (top-left of the card editor), and navigate to the `Styling` section.  
These variable enable some popular CSS tweaks to the card one might want.
You should get instant feedback when changing a variable on the preview inside Anki, so don't be afraid to try changing them.  
Make sure you **don't forget** a *doublequote* or a *semi-colon* at the end of a line.

# Settings breakdown
### main-picture-position
`"left"` to swap the picture and the vocabulary box.  
Valid values : `"left"`, `"right"`  
Default value : `"left"`

### sentence-furigana
Controls when to display furigana in your sentence  
Valid values : `"hover"`, `"always"`, `"off"`  
Default value : `"hover"`

### sentence-position 
Displays the sentence above or below the definition box.  
Valid values : `"above"`, `"below"`  
Default value : `"above"`

### mobile-sentence-position
Same as above, for mobile.

### mobile-audio-buttons
On mobile, audio play buttons are shown on the button left of the card. If you want a layout similar to desktop you can set this to `"header"`  
Valid values : `"default"`, `"header"`  

### nsfw-blur-contained
The blur effect for NSFW tagged card expands outside the main picture box. You can disable this with this variable  
Valid values : `"on"`, `"off"`  
Default value : `"off"`

### open-misc-info
Expands the misc-info box by default  
Valid values : `"on"`, `"off"`  
Default value : `"off"`

### glossary-separator
Adds a line between different dictionaries in glossaries.  
Valid values : `"on"`, `"off"`  
Default value : `"off"`

Note : The formatting of JMDict has all meanings of a word in its own entry, so they all get separated.

### jitendex-format
Customizes Jitendex dictionary by removing some information  
Valid values : `"full"`, `"minimal"`, space-separated list of `no-tags`, `no-sentence`, `no-forms`, `no-xref`, `no-img`  
Default value : `"full"`  
|   values   | behaviour |
| ---------- | --------- |
| `minimal` | removes **everything** except the meanings. Careful as it will also remove explanations you might want to keep. |
| `no-tags` | removes POS tags. |
| `no-sentence` | removes example sentence. |
| `no-forms` | removes the forms table. |
| `no-xref` | removes cross references to other entries (See also...) |
| `no-img` | removes images |

Therefore, having `--jitendex-foramt: "no-forms no-sentence no-xref";` will hide forms, examples sentences and cross references.

# Is that it ? How can I change xx or yy ?
If you think you need to change something in the layout, and that it would also benefit other users of Lapis. We are open to suggestions, please open an issue.