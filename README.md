# ConstrainedScrollBehavior

An AppBarLayout.ScrollingViewBehavior that adapts scrolling view height based on its content.

This is useful in conjunction with scrolling AppBarLayouts. With the default behavior, the 
AppBarLayout keeps scrolling out of the screen even if the scrolling content is over.
With ConstrainedScrollBehavior, no more offset is applied if the scrolling view is 
completely visible.

See http://stackoverflow.com/q/31117510/4288782 for example.

### Notes

For this to work, you need:
- set this behavior to the scrolling view
- have match_parent as height
- have at least one of the AppBarLayout childs use the flags:

`app:layout_scrollFlags="scroll|exitUntilCollapsed"`
