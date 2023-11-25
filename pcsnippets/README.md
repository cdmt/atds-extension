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

| Shortcode | Value | Result                                  | Caveat    |
| --------- | ----- | --------------------------------------- | --------- |
| `type12`  | 12px  | `<TypeMini as=""></TypeMini>`           | -         |
| `type14`  | 14px  | `<TypePrius as=""></TypePrius>`         | Uppercase |
| `type14`  | 14px  | `<TypeSmart as=""></TypeSmart>`         | -         |
| `type16`  | 16px  | `<TypeFiesta as=""></TypeFiesta>`       | -         |
| `type16`  | 16px  | `<TypePicanto as=""></TypePicanto>`     | Uppercase |
| `type18`  | 18px  | `<TypeBeetle as=""></TypeBeetle>`       | -         |
| `type20`  | 20px  | `<TypeToledo as=""></TypeToledo>`       | -         |
| `type26`  | 26px  | `<TypeInsignia as=""></TypeInsignia>`   | -         |
| `type32`  | 32px  | `<TypePhantom as=""></TypePhantom>`     | -         |
| `type40`  | 40px  | `<TypeDiscovery as=""></TypeDiscovery>` | -         |
| `type96`  | 96px  | `<TypeCherokee as=""></TypeCherokee>`   | -         |
| `type144` | 144px | `<TypeHummer as=""></TypeHummer>`       | -         |

\_\_

## Styling and spacing

If you never know what `getRelatedOneSpacing` means, or how to add in 4, 8, 12, 16, 24px margins and padding. Then all you have to do is type:

`s4` = 4px,
`s8` = 8px
`s24` = 24px
and so on, its just easier than trying to work out what `getRelatedOneSpacing` and it just fills everything in for you.

### List WITHOUT theme wrapper

Use the following shortcode if you DON'T have your Styled Component wrapped within a theme

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

### List WITH theme wrapper

If you DO have your Styled component wrapped within a theme, please use `short` like so: -

| Shortcode | Value | Result                                          |
| --------- | ----- | ----------------------------------------------- |
| `s4short` | 4px   | `${ThemeSelectors.getGroupOneSpacing(theme)}`   |
| `s8short` | 8px   | `${ThemeSelectors.getGroupTwoSpacing(theme)}`   |
| `s12hort` | 12px  | `${ThemeSelectors.getGroupThreeSpacing(theme)}` |
| `s16hort` | 16px  | `$ThemeSelectors.getGroupFourSpacing(theme)}`   |
| `s20hort` | 20px  | `$ThemeSelectors.getGroupFiveSpacing(theme)}`   |
| `s24hort` | 24px  | `$ThemeSelectors.getGroupSixSpacing(theme)}`    |
| `s32hort` | 32px  | `$ThemeSelectors.getRelatedOneSpacing(theme)}`  |
| `s48hort` | 48px  | `$ThemeSelectors.getRelatedTwoSpacing(theme)}`  |
| `s64hort` | 64px  | `$ThemeSelectors.getDistinctOneSpacing(theme)}` |
| `s72hort` | 72px  | `$ThemeSelectors.getDistinctTwoSpacing(theme)}` |

---

# colors

col-b - blue - ${({ theme }) => ThemeSelectors.getBlue(theme)}
col-b-short - blue - ${ThemeSelectors.getBlue(theme)}
col-lb - blue - ${({ theme }) => ThemeSelectors.getLightBlue(theme)}
col-lb-short - dark blue - ${ThemeSelectors.getLightBlue(theme)}
col-db - dark blue - ${({ theme }) => ThemeSelectors.getDarkBlue(theme)}
col-lb-short - blue - ${ThemeSelectors.getDarkBlue(theme)}
col-r - red - ${({ theme }) => ThemeSelectors.getRed(theme)}
col-r-short - red - ${ThemeSelectors.getRed(theme)}
col-lr - light red - ${({ theme }) => ThemeSelectors.getLightRed(theme)}
col-lr-short - light red - ${ThemeSelectors.getLightRed(theme)}
col-dr - dark red - ${({ theme }) => ThemeSelectors.getDarkRed(theme)}
col-dr-short - dark red - ${ThemeSelectors.getDarkRed(theme)}
col-g - green - ${({ theme }) => ThemeSelectors.getGreen(theme)}
col-g-short - green - ${ThemeSelectors.getGreen(theme)}
col-lg - light green - ${({ theme }) => ThemeSelectors.getLightGreen(theme)}
col-g-short - green - ${ThemeSelectors.getLightGreen(theme)}
col-dg - dark green - ${({ theme }) => ThemeSelectors.getDarkGreen(theme)}
col-g-short - dark green - ${ThemeSelectors.getDarkGreen(theme)}
col-y - yellow - ${({ theme }) => ThemeSelectors.getYellow(theme)}
col-y-short - yellow - ${ThemeSelectors.getYellow(theme)}
col-ly - light yellow - ${({ theme }) => ThemeSelectors.getLightYellow(theme)}
col-ly-short - ligh yellow - ${ThemeSelectors.getLightYellow(theme)}
col-dy - dark yellow - ${({ theme }) => ThemeSelectors.getYellow(theme)}
col-dy-short - dark yellow - ${ThemeSelectors.getDarkYellow(theme)}
col-g - grey - ${({ theme }) => ThemeSelectors.getGrey(theme)}
col-g-short - grey - ${ThemeSelectors.getGrey(theme)}
col-lg - light grey - ${({ theme }) => ThemeSelectors.getLightGrey(theme)}
col-lg-short - light grey - ${ThemeSelectors.getLightGrey(theme)}
col-dg - dark grey - ${({ theme }) => ThemeSelectors.getDarkGrey(theme)}
col-dg-short - dark rey - ${ThemeSelectors.getDarkGrey(theme)}
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