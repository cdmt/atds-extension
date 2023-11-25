# pcsnippets README

# Type
type12 - 12px - <TypeMini as=""></TypeMini>
type14 - 14px - <TypePrius as=""></TypePrius>
type14 - 14px - <TypeSmart as=""></TypeSmart>
type16 - 16px - <TypeFiesta as=""></TypeFiesta>
type16 - 16px - <TypePicanto as=""></TypePicanto>
type18 - 18px - <TypeBeetle as=""></TypeBeetle>
type20 - 20px - <TypeToledo as=""></TypeToledo>
type26 - 26px - <TypeInsignia as=""></TypeInsignia>
type32 - 32px - <TypePhantom as=""></TypePhantom>
type40 - 40px - <TypeDiscovery as=""></TypeDiscovery>
type40 - 96px - <TypeCherokee as=""></TypeCherokee>
type40 - 144px - <TypeHummer as=""></TypeHummer>

# Spacing
s4 - 4px - ${({ theme }) => ThemeSelectors.getGroupOneSpacing(theme)}
s4short - 4px - ${ThemeSelectors.getGroupOneSpacing(theme)}
s8 - 8px - ${({ theme }) => ThemeSelectors.getGroupTwoSpacing(theme)}
s8short - 8px - ${ThemeSelectors.getGroupTwoSpacing(theme)}
s12 - 12px - ${({ theme }) => ThemeSelectors.getGroupThreeSpacing(theme)}
s12short - 12px - ${ThemeSelectors.getGroupThreeSpacing(theme)}
s16 - 16px - ${({ theme }) => ThemeSelectors.getGroupFourSpacing(theme)}
s16short - 16px - ${ThemeSelectors.getGroupFourSpacing(theme)}
s24 - 24px - ${({ theme }) => ThemeSelectors.getGroupFiveSpacing(theme)}
s24short - 24px - ${ThemeSelectors.getGroupFiveSpacing(theme)}
s32 - 32px - ${({ theme }) => ThemeSelectors.getRelatedOneSpacing(theme)}
s32short - 32px - ${ThemeSelectors.getRelatedOneSpacing(theme)}
s48 - 48px - ${({ theme }) => ThemeSelectors.getRelatedTwoSpacing(theme)}
s48short - 48px - ${ThemeSelectors.getRelatedTwoSpacing(theme)}
s64 - 64px - ${({ theme }) => ThemeSelectors.getDistinctOneSpacing(theme)}
s64short - 64px - ${ThemeSelectors.getDistinctOneSpacing(theme)}
s72 - 72px - ${({ theme }) => ThemeSelectors.getDistinctTwoSpacing(theme)}
s64short - 64px - ${ThemeSelectors.getDistinctTwoSpacing(theme)}

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
col-at-r - red -  ${({ theme }) => ThemeSelectors.getATRed(theme)}
col-at-b-short - blue ${ThemeSelectors.getATRed(theme)}
col-w - white -  ${({ theme }) => ThemeSelectors.getWhite(theme)}
col-w-short - white ${ThemeSelectors.getWhite(theme)}
col-ac - action color -  ${({ theme }) => ThemeSelectors.getActionColor(theme)}
col-ac-short - action color -  ${ThemeSelectors.getActionColor(theme)}
col-aac - action active color -  ${({ theme }) => ThemeSelectors.getActionActiveColor(theme)}
col-aac-short - action color -  ${ThemeSelectors.getActionActiveColor(theme)}
col-ah - action hover color -  ${({ theme }) => ThemeSelectors.getActionHoverColor(theme)}
col-ah-short - action hover color -  ${ThemeSelectors.getActionHoverColor(theme)}
col-v - visited -  ${({ theme }) => ThemeSelectors.getVisitedColor(theme)}
col-v-short - visited -  ${ThemeSelectors.getVisitedColor(theme)}
col-f - focus -  ${({ theme }) => ThemeSelectors.getFocusColor(theme)}
col-f-short - focus -  ${ThemeSelectors.getFocusColor(theme)}
col-g - graphic - ${({ theme }) => ThemeSelectors.getGraphicColor(theme)}
col-g-short - graphic -  ${ThemeSelectors.getGraphicColor(theme)}
col-e - error - ${({ theme }) => ThemeSelectors.getGraphicColor(theme)}
col-e-short - error -  ${ThemeSelectors.getGraphicColor(theme)}
col-s - success - ${({ theme }) => ThemeSelectors.getSuccessColor(theme)}
col-s-short - success -  ${ThemeSelectors.getSuccessColor(theme)}
col-acc - accent - ${({ theme }) => ThemeSelectors.getAccentColor(theme)}
col-acc-short - accent -  ${ThemeSelectors.getAccentColor(theme)}
col-p - placeholder - ${({ theme }) => ThemeSelectors.getPlaceholderColor(theme)}
col-p-short - placeholder -  ${ThemeSelectors.getPlaceholderColor(theme)}
col-t - title - ${({ theme }) => ThemeSelectors.getTitleColor(theme)}
col-t-short - title -  ${ThemeSelectors.getTitleColor(theme)}
col-c - copy - ${({ theme }) => ThemeSelectors.getCopyColor(theme)}
col-c-short - copy -  ${ThemeSelectors.getCopyColor(theme)}
































