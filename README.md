# ng2-font-awesome
Simple, easy to use Angular 2 component to manage Font Awesome icons.

# How to install

**Install Packages**
`npm install --save font-awesome ng2-font-awesome`

**Import the module:**
```typescript
//...
import { FontAwesomeModule } from 'ng2-font-awesome/ng2-font-awesome';
@NgModule({
  //...
  imports: [
    //...
    FontAwesomeModule
  ],
  //...
})
export class AppModule { }
```

**If you're using [Angular CLI](https://github.com/angular/angular-cli), add the font-awesome CSS to `styles` inside the `angular-cli.json`**
```json
"styles": [
    "styles.css",
    "../node_modules/font-awesome/css/font-awesome.css"
],
```
*NOTE: If using SCSS preprocessor just change the `css` for `scss`*

**If you're not using the CLI, import the stylesheet to your `index.html` file**
```html
<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" />
```

# Usage and Options
To use the component you can choose between these 2 selectors: `<ng2-fa></ng2-fa>` or `<fa></fa>`.

Name      | Type               | Options    | Required
---       | ---                | ---        | ---
name      | `String`           | [F-A Icons](http://fontawesome.io/icons/) | Yes
size      | `String`           | `lg, 2x, 3x, 4x, 5x`
fixed     | `Boolean`          | `true | false`
animation |  `String`          | `spin | pulse`
rotate    |  `Number | String` | `90 | 180 | 270` `horizontal | vertical`

*Example Use*
```html
<fa name="cog" animation="spin"></fa>
```

# TODO
- [ ] Create unit tests
- [ ] Add `directive` option
- [ ] Add [Stacked Icons](http://fontawesome.io/examples/#stacked) support
- [ ] Add [List Icons](http://fontawesome.io/examples/#list) support