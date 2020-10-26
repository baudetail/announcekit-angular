![](https://announcekit.app/images/logo@2x.png)

The easiest way to use AnnounceKit widgets in your Angular apps (>=4.2.0).

**Visit [https://announcekit.app](https://announcekit.app) to get started with AnnounceKit.**
[CodeSandbox Demo](https://codesandbox.io/s/announcekit-vue20-demo-jcfjf)

[Documentation](https://announcekit.app/docs/angular)

## Installation

```sh
yarn add announcekit-angular
```

## Usage

app.module.ts
```ts
import {AnnouncekitModule} from 'announcekit-angular'

@NgModule({
  declarations: [
    AppComponent,
  ],
  imports: [
    AnnouncekitModule,
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```


app.component.html
```html
    <announcekit [user]="user" [data]="data"  widget="https://announcekit.app/widgets/v2/2TrvK8">
        What's new
    </announcekit>
```

## Props

Common props you may want to specify include:

- **`widget`** - The url of the widget. You can obtain it while creating or editing widget in AnnounceKit Dashboard.
- `widgetStyle` - You can apply CSS rules to modify / tune the position of the widget.
- `floatWidget` - Set true if the widget is a Float widget.
- `embedWidget` - Set true if the widget is a Embed widget.
- `user` - User properties (for user tracking)
- `data` - Segmentation data
- `lang` - Language selector
- `onWidgetOpen` - Called when the widget is opened.
- `onWidgetClose` - Called when the widget is closed.
- `onWidgetUnread` - Called when unread post count of widget has been updated.