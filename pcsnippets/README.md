# PC Snippets README

Welcome to PC Snippets, this extenion is aimed at helping developers who work with ATDS and styled components. Speeding up dev time by reducing time and effort working out what fonts are equal to what sizes, what paddings to use and more.

---

## Type / Fonts

If you're having problems finding the right Styled component font to use from a Figma Design, then this will help you.

For example, in Figma a heading is set to 40px, however you don't know what font name/type that is equivalent to.

So, all you need to do now is type `t40` and enter

This will output:
`<TypeDiscovery as='p'></TypeDiscovery>`

So, now all you have to do is type in `t` then select your font size which is used in Figma and it will give you the correct font to use. This saves time and effort trying to work out what the right font to use is. It also bridges that gap between design and dev and avoids confusion.

| Shortcode    | Value | Result                                  | Caveat    |
| ------------ | ----- | --------------------------------------- | --------- |
| `t12`        | 12px  | `<TypeMini as=""></TypeMini>`           | -         |
| `t14prius`   | 14px  | `<TypePrius as=""></TypePrius>`         | Uppercase |
| `t14`        | 14px  | `<TypeSmart as=""></TypeSmart>`         | -         |
| `t16`        | 16px  | `<TypeFiesta as=""></TypeFiesta>`       | -         |
| `t16picanto` | 16px  | `<TypePicanto as=""></TypePicanto>`     | Uppercase |
| `t18`        | 18px  | `<TypeBeetle as=""></TypeBeetle>`       | -         |
| `t20`        | 20px  | `<TypeToledo as=""></TypeToledo>`       | -         |
| `t26`        | 26px  | `<TypeInsignia as=""></TypeInsignia>`   | -         |
| `t32`        | 32px  | `<TypePhantom as=""></TypePhantom>`     | -         |
| `t40`        | 40px  | `<TypeDiscovery as=""></TypeDiscovery>` | -         |
| `t96`        | 96px  | `<TypeCherokee as=""></TypeCherokee>`   | -         |
| `t144`       | 144px | `<TypeHummer as=""></TypeHummer>`       | -         |

---

## Styling and spacing

If you never know what `getRelatedOneSpacing` means, or how to add in 4, 8, 12, 16, 24px margins and padding. Then all you have to do is type:

`s4` = 4px,
`s8` = 8px
`s24` = 24px
its just easier than trying to work out what `getRelatedOneSpacing` and it just fills everything in for you.

> **Note:** If you you're using a theme wrapper, use `-short` ie: `s8short` to output the following `$ThemeSelectors.getGroupTwoSpacing(theme)}`

| Shortcode | Value | Result                                                          |
| --------- | ----- | --------------------------------------------------------------- |
| `s4`      | 4px   | `${({ theme }) => ThemeSelectors.getGroupOneSpacing(theme)}`    |
| `s8`      | 8px   | `${({ theme }) => ThemeSelectors.getGroupTwoSpacing(theme)}`    |
| `s12`     | 12px  | `${({ theme }) => ThemeSelectors.getGroupThreeSpacing(theme)}`  |
| `s16`     | 16px  | `${({ theme }) => ThemeSelectors.getGroupFourSpacing(theme)}`   |
| `s20`     | 20px  | `${({ theme }) => ThemeSelectors.getGroupFiveSpacing(theme)}`   |
| `s24`     | 24px  | `${({ theme }) => ThemeSelectors.getGroupSixSpacing(theme)}`    |
| `s32`     | 32px  | `${({ theme }) => ThemeSelectors.getRelatedOneSpacing(theme)}`  |
| `s48`     | 48px  | `${({ theme }) => ThemeSelectors.getRelatedTwoSpacing(theme)}`  |
| `s64`     | 64px  | `${({ theme }) => ThemeSelectors.getDistinctOneSpacing(theme)}` |
| `s72`     | 72px  | `${({ theme }) => ThemeSelectors.getDistinctTwoSpacing(theme)}` |

---

# Colors

> **Note:** If you you're using a theme wrapper, use `-short` ie: `cBlueShort` to output the following `$ThemeSelectors.getBlue(theme)}`

| ShortCode      | Value        | Result                                                   |
| -------------- | ------------ | -------------------------------------------------------- |
| `cBlue`        | blue         | `${({ theme }) => ThemeSelectors.getBlue(theme)}`        |
| `cBlueLight`   | blue light   | `${({ theme }) => ThemeSelectors.getLightBlue(theme)}`   |
| `cBlueDark`    | blue dark    | `${({ theme }) => ThemeSelectors.getDarkBlue(theme)}`    |
| `cRed`         | red          | `${({ theme }) => ThemeSelectors.getRed(theme)}`         |
| `cRedLight`    | red light    | `${({ theme }) => ThemeSelectors.getLightRed(theme)}`    |
| `cRedDark`     | red dark     | `${({ theme }) => ThemeSelectors.getDarkRed(theme)}`     |
| `cGreen`       | green        | `${({ theme }) => ThemeSelectors.getGreen(theme)}`       |
| `cGreenLight`  | green light  | `${({ theme }) => ThemeSelectors.getLightGreen(theme)}`  |
| `cGreenDark`   | green dark   | `${({ theme }) => ThemeSelectors.getDarkGreen(theme)}`   |
| `cYellow`      | yellow       | `${({ theme }) => ThemeSelectors.getYellow(theme)}`      |
| `cYellowLight` | yellow light | `${({ theme }) => ThemeSelectors.getLightYellow(theme)}` |
| `cYellowDark`  | yellow dark  | `${({ theme }) => ThemeSelectors.getDarkYellow(theme)}`  |
| `cGrey`        | grey         | `${({ theme }) => ThemeSelectors.getGrey(theme)}`        |
| `cGreyLight`   | grey light   | `${({ theme }) => ThemeSelectors.getLightGrey(theme)}`   |
| `cGreyDark`    | grey dark    | `${({ theme }) => ThemeSelectors.getDarkGrey(theme)}`    |
| `cWhite`       | white        | `${({ theme }) => ThemeSelectors.getWhite(theme)}`       |

---

## More colour values:

| ShortCode       | Result                                                         |
| --------------- | -------------------------------------------------------------- |
| `cAction`       | `${({ theme }) => ThemeSelectors.getAction(theme)}`            |
| `cActionActive` | `${({ theme }) => ThemeSelectors.getActionActiveColor(theme)}` |
| `cActionHover`  | `${({ theme }) => ThemeSelectors.getActionHoverColor(theme)}`  |
| `cVisited`      | `${({ theme }) => ThemeSelectors.getVisitedColor(theme)}`      |
| `cFocus`        | `${({ theme }) => ThemeSelectors.getFocusColor(theme)}`        |
| `cGraphic`      | `${({ theme }) => ThemeSelectors.getGraphicColor(theme)}`      |
| `cError`        | `${({ theme }) => ThemeSelectors.getErrorColor(theme)}`        |
| `cSuccess`      | `${({ theme }) => ThemeSelectors.getSuccessColor(theme)}`      |
| `cAccent`       | `${({ theme }) => ThemeSelectors.getAccentColor(theme)}`       |
| `cPlaceholder`  | `${({ theme }) => ThemeSelectors.getPlaceholderColor(theme)}`  |
| `cTitle`        | `${({ theme }) => ThemeSelectors.getTitleColor(theme)}`        |
| `cCopy`         | `${({ theme }) => ThemeSelectors.getCopyColor(theme)}`         |

---

## ATDS Components

### Link

`scLink`

```
<Link,
  href=""
  routerLink={false}"
  onInteraction={(e: SyntheticEvent) => {
    e.preventDefault();
    setVisible(true);
  }}",
  attributes={{",
    [dataAttrGUI]: getDataGuiPrefixedValue(\"attr-here\"),
    \"aria-label":""
  }}",
  trackData={{",
    <!-- eventEntity: buildUiInteractionEntity(\"track-here\", \"click\")
  }}>
</Link>"
```

---

### Button

`scButton`

```
<Button
  displayType=""
  text=""
  url={url}
  className=""
  additionalClass=""
  fullWidth={true}"
  data-gui=""
  trackingData={{"
    label:""
    category: TrackingCategory.STANDARD
    action: TrackingAction.CLICK
  }}",
/>"
```

---

### Input

`scInput`

```
<Input
  additionalClass=""
  attributes={{"
    'data-testid': ""
  }}"
  errorText=""
  fieldType=""
  helpText=""
  id=""
  label=""
  name=""
  prefix=""
  suffix=""
  themeType=""
/>
```

---

### Toggleswitch

`scToggleSwitch`

```
 <Selection
  additionalClass=""
  attributes={{",
    placeholder: "",
  }}",
  defaultChecked
  errorText=""
  fieldType=""
  helpText=""
  id=""
  label=""
  name=""
/>"
```

---

### Checkbox

`scCheckbox`

```
<Selection
  additionalClass=""
  attributes={{",
    placeholder: 'Placeholder'",
  }}",
  defaultChecked
  errorText=""
  fieldType=""
  helpText={<>${1:Help text}{' '}<a href=\"${2:url}\">${3:Link text}</a></>}",
  id=""
  label=""
  name=""
/>
```

---

# Troubleshooting

If you are having any issues, please try adding the following into your `settings.json` file for vscode: -

```
    "files.associations": {
        "*.code-snippets": "snippets"
    },
    "editor.acceptSuggestionOnEnter": "on",
    "editor.tabCompletion": "on",
    "editor.formatOnSave": true,
    "editor.snippetSuggestions": "top",
    "editor.suggest.snippetsPreventQuickSuggestions": true,
    "editor.quickSuggestions": {
        "comments": "on",
        "strings": "on",
        "other": "on"
    },
    "[snippets]": {}
```
