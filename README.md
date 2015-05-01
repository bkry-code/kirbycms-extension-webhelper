# kirbycms-extension-webhelper
A collection of little helper for usage in Kirby

## Installation

### GIT

Go into the `{kirby_installation}/site/plugins` directory and execute following command.

```bash
$ git clone https://github.com/fanningert/kirbycms-extension-webhelper.git
```

### GIT submodule

Go in the root directory of your git repository and execute following command to add the repository as submodule to your GIT repository.

```bash
$ git submodule add https://github.com/fanningert/kirbycms-extension-webhelper.git ./site/plugins/kirbycms-extension-webhelper
$ git submodule init
$ git submodule update
```

### Manuell

## Update

### GIT

Go into the `{kirby_installation}/site/plugins/kirbycms-extension-webhelper` directory and execute following command.

```bash
$ git pull
```

### GIT submodule

Go in the root directory of your git repository and execute following command to update the submodule of this extension.

```bash
$ git submodule update
```

## Content

### Messages boxes

http://www.jankoatwarpspeed.com/css-message-boxes-for-different-message-types/

Generel the tag exist in two versions.

**Short tag**

```kirbytag
(message_type: text)
```

**Long text tag**

```kirbytag
(message_type)
text
(/message_type)
```

#### Information messages

```kirbytag
(info: This is an important information.)
```

Output
```html
<div class="messagebox messagebox-info">This is an important information.</div>
```

#### Success messages

```kirbytag
(success: Hooooray! This messages says that operation succeeded!!)
```

Output
```html
<div class="messagebox messagebox-success">Hooooray! This messages says that operation succeeded!!</div>
```

#### Warning messages

```kirbytag
(warning: Now this is a warning! One more click and you`ll face the consequences!)
```

Output
```html
<div class="messagebox messagebox-warning">Now this is a warning! One more click and you`ll face the consequences!</div>
```

#### Error messages

```kirbytag
(error: Oooops, this is an error message. You know what that means.)
```

Output
```html
<div class="messagebox messagebox-error">Oooops, this is an error message. You know what that means.</div>
```

#### Validation messages

```kirbytag
(validation: First name is a required field)
```

Output
```html
<div class="messagebox messagebox-validation">First name is a required field</div>
```

### Figure

#### Simple example

```kirbytag
(figure: text)
content
(/figure)
```

Output
```html
<figure>
  content
  <figcaption>text</figcaption>
</figure>
```

#### Caption top

```kirbytag
(figure: text caption_top: true class: test-class)
content
(/figure)
```

Output
```html
<figure class="test-class">
  <figcaption>text</figcaption>
  content
</figure>
```
