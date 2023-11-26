# PC Snippets README

Welcome to PC Snippets, this extenion is aimed at helping developers who work with ATDS and styled components. Speeding up dev time by reducing time and effort working out what fonts are equal to what sizes, what paddings to use and more.

## Type / Fonts

If you're having problems finding the right Styled component font to use from a Figma Design, then this will help you.

For example, in Figma a heading is set to 40px, however you don't know what font name/type that is equivalent to.

So, all you need to do now is starting typing the following:
`type16`

This will now output:
`<TypeFiesta as="p">your text here</TypeFiesta>`

So, now all you have to do is type in "type" then select your font size which is used in Figma and it will give you the correct font to use. This saves time and effort trying to work out what the right font to use is. It also bridges that gap between design and dev and avoids confusion.

### List

| Shortcode      | Value | Result                                  | Caveat    |
| ---------------| ----- | --------------------------------------- | --------- |
| `t-12`         | 12px  | `<TypeMini as=""></TypeMini>`           | -         |
| `t-14-prius`   | 14px  | `<TypePrius as=""></TypePrius>`         | Uppercase |
| `t-14`         | 14px  | `<TypeSmart as=""></TypeSmart>`         | -         |
| `t-16`         | 16px  | `<TypeFiesta as=""></TypeFiesta>`       | -         |
| `t-16-picanto` | 16px  | `<TypePicanto as=""></TypePicanto>`     | Uppercase |
| `t-18`         | 18px  | `<TypeBeetle as=""></TypeBeetle>`       | -         |
| `t-20`         | 20px  | `<TypeToledo as=""></TypeToledo>`       | -         |
| `t-26`         | 26px  | `<TypeInsignia as=""></TypeInsignia>`   | -         |
| `t-32`         | 32px  | `<TypePhantom as=""></TypePhantom>`     | -         |
| `t-40`         | 40px  | `<TypeDiscovery as=""></TypeDiscovery>` | -         |
| `t-96`         | 96px  | `<TypeCherokee as=""></TypeCherokee>`   | -         |
| `t-144`        | 144px | `<TypeHummer as=""></TypeHummer>`       | -         |

\_\_

## Styling and spacing

If you never know what `getRelatedOneSpacing` means, or how to add in 4, 8, 12, 16, 24px margins and padding. Then all you have to do is type:

`s-4` = 4px,
`s-8` = 8px
`s-24` = 24px
and so on, its just easier than trying to work out what `getRelatedOneSpacing` and it just fills everything in for you.

### List WITHOUT theme wrapper

Use the following shortcode if you DON'T have your Styled Component wrapped within a theme

| Shortcode | Value | Result                                                          |
| --------- | ----- | --------------------------------------------------------------- |
| `s-4`     | 4px   | `${({ theme }) => ThemeSelectors.getGroupOneSpacing(theme)}`    |
| `s-8`     | 8px   | `${({ theme }) => ThemeSelectors.getGroupTwoSpacing(theme)}`    |
| `s-12`    | 12px  | `${({ theme }) => ThemeSelectors.getGroupThreeSpacing(theme)}`  |
| `s-16`    | 16px  | `${({ theme }) => ThemeSelectors.getGroupFourSpacing(theme)}`   |
| `s-20`    | 20px  | `${({ theme }) => ThemeSelectors.getGroupFiveSpacing(theme)}`   |
| `s-24`    | 24px  | `${({ theme }) => ThemeSelectors.getGroupSixSpacing(theme)}`    |
| `s-32`    | 32px  | `${({ theme }) => ThemeSelectors.getRelatedOneSpacing(theme)}`  |
| `s-48`    | 48px  | `${({ theme }) => ThemeSelectors.getRelatedTwoSpacing(theme)}`  |
| `s-64`    | 64px  | `${({ theme }) => ThemeSelectors.getDistinctOneSpacing(theme)}` |
| `s-72`    | 72px  | `${({ theme }) => ThemeSelectors.getDistinctTwoSpacing(theme)}` |

### List WITH theme wrapper

If you DO have your Styled component wrapped within a theme, please use `short` like so: -

| Shortcode    | Value | Result                                          |
| ------------ | ----- | ----------------------------------------------- |
| `s-4-short`  | 4px   | `${ThemeSelectors.getGroupOneSpacing(theme)}`   |
| `s-8-short`  | 8px   | `${ThemeSelectors.getGroupTwoSpacing(theme)}`   |
| `s-12-short` | 12px  | `${ThemeSelectors.getGroupThreeSpacing(theme)}` |
| `s-16-short` | 16px  | `$ThemeSelectors.getGroupFourSpacing(theme)}`   |
| `s-20-short` | 20px  | `$ThemeSelectors.getGroupFiveSpacing(theme)}`   |
| `s-24-short` | 24px  | `$ThemeSelectors.getGroupSixSpacing(theme)}`    |
| `s-32-short` | 32px  | `$ThemeSelectors.getRelatedOneSpacing(theme)}`  |
| `s-48-short` | 48px  | `$ThemeSelectors.getRelatedTwoSpacing(theme)}`  |
| `s-64-short` | 64px  | `$ThemeSelectors.getDistinctOneSpacing(theme)}` |
| `s-72-short` | 72px  | `$ThemeSelectors.getDistinctTwoSpacing(theme)}` |

---

# colors

| ShortCode        | Value        | Result                                                   |
| ---------------- | ------------ | -------------------------------------------------------- |
| `c-blue`         | blue         | `${({ theme }) => ThemeSelectors.getBlue(theme)}`        |
| `c-blue-light`   | blue light   | `${({ theme }) => ThemeSelectors.getLightBlue(theme)}`   |
| `c-blue-dark`    | blue dark    | `${({ theme }) => ThemeSelectors.getdarkBlue(theme)}`    |
| `c-red`          | red          | `${({ theme }) => ThemeSelectors.getRed(theme)}`         |
| `c-red-light`    | red light    | `${({ theme }) => ThemeSelectors.getLightRed(theme)}`    |
| `c-red-dark`     | red dark     | `${({ theme }) => ThemeSelectors.getDarkRed(theme)}`     |
| `c-green`        | green        | `${({ theme }) => ThemeSelectors.getGreen(theme)}`       |
| `c-green-light`  | green light  | `${({ theme }) => ThemeSelectors.getLightGreen(theme)}`  |
| `c-green-dark`   | green dark   | `${({ theme }) => ThemeSelectors.getDarkGreen(theme)}`   |
| `c-yellow`       | yellow       | `${({ theme }) => ThemeSelectors.getYellow(theme)}`      |
| `c-yellow-light` | yellow light | `${({ theme }) => ThemeSelectors.getLighyYellow(theme)}` |
| `c-yellow-dark`  | yellow dark  | `${({ theme }) => ThemeSelectors.getDarlYellow(theme)}`  |
| `c-grey`         | grey         | `${({ theme }) => ThemeSelectors.getGrey(theme)}`        |
| `c-grey-light`   | grey light   | `${({ theme }) => ThemeSelectors.getLightGrey(theme)}`   |
| `c-grey-dark`    | grey dark    | `${({ theme }) => ThemeSelectors.getDarkGrey(theme)}`    |

col-at-b - blue - ${({ theme }) => ThemeSelectors.getATBlue(theme)}
col-at-b-short - blue ${ThemeSelectors.getATBlue(theme)}
col-at-r - red - ${({ theme }) => ThemeSelectors.getATRed(theme)}
col-at-b-short - blue ${ThemeSelectors.getATRed(theme)}
col-w - white - ${({ theme }) => ThemeSelectors.getWhite(theme)}
col-w-short - white ${ThemeSelectors.getWhite(theme)}
col-ac - action color - ${({ theme }) => ThemeSelectors.getActionColor(theme)}
col-ac-short - action color - ${ThemeSelectors.getActionColor(theme)}
col-aac - action active color - ${({ theme }) => ThemeSelectors.getActionActiveColor(theme)}
col-aac-short - action color - ${ThemeSelectors.getActionActiveColor(theme)}
col-ah - action hover color - ${({ theme }) => ThemeSelectors.getActionHoverColor(theme)}
col-ah-short - action hover color - ${ThemeSelectors.getActionHoverColor(theme)}
col-v - visited - ${({ theme }) => ThemeSelectors.getVisitedColor(theme)}
col-v-short - visited - ${ThemeSelectors.getVisitedColor(theme)}
col-f - focus - ${({ theme }) => ThemeSelectors.getFocusColor(theme)}
col-f-short - focus - ${ThemeSelectors.getFocusColor(theme)}
col-g - graphic - ${({ theme }) => ThemeSelectors.getGraphicColor(theme)}
col-g-short - graphic - ${ThemeSelectors.getGraphicColor(theme)}
col-e - error - ${({ theme }) => ThemeSelectors.getGraphicColor(theme)}
col-e-short - error - ${ThemeSelectors.getGraphicColor(theme)}
col-s - success - ${({ theme }) => ThemeSelectors.getSuccessColor(theme)}
col-s-short - success - ${ThemeSelectors.getSuccessColor(theme)}
col-acc - accent - ${({ theme }) => ThemeSelectors.getAccentColor(theme)}
col-acc-short - accent - ${ThemeSelectors.getAccentColor(theme)}
col-p - placeholder - ${({ theme }) => ThemeSelectors.getPlaceholderColor(theme)}
col-p-short - placeholder - ${ThemeSelectors.getPlaceholderColor(theme)}
col-t - title - ${({ theme }) => ThemeSelectors.getTitleColor(theme)}
col-t-short - title - ${ThemeSelectors.getTitleColor(theme)}
col-c - copy - ${({ theme }) => ThemeSelectors.getCopyColor(theme)}
col-c-short - copy - ${ThemeSelectors.getCopyColor(theme)}
